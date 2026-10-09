# App Architecture Readout — Business Pilot Readiness

**Date:** 9 October 2026  
**Source inspected:** connected Lovable project "Real World Atlas" (project ID b3293d2a-3218-4206-ab04-af8e984023ac) plus GitHub default-branch metadata/files for life-lived-network and life-lived-network2.  
**Status:** preliminary; repository-source-of-truth and backend security decisions remain open. No application feature code was changed by this readout. No tests were run.

## Source-of-truth finding

The connected Lovable project is named Real World Atlas and is the only project returned in the workspace. Both GitHub repos have matching AGENTS.md and docs/agents/INVARIANTS.md content, and their README/package manifests are similar. The life-lived-network repository is larger (GitHub metadata reported size 1484 vs 481), and it has .github/workflows/verify.yml; life-lived-network2 did not have that workflow at the checked path. This suggests life-lived-network is the stronger canonical candidate, but it does **not** prove which repository is connected to the live Lovable project or production deployment.

**Decision required before code edits:** verify the connected GitHub repository in Lovable's GitHub integration and confirm the intended canonical repo. Do not copy, merge, archive or delete either repo based only on size.

## Verified project rules

- AGENTS.md says the app is Lovable-connected, published history must not be rewritten, no autonomous merge to main, and external collaboration uses PRs.
- docs/agents/INVARIANTS.md says no second possibility/matching engine, unknown must not become confirmed, stale capability must not look current, unqualified providers must not appear qualified, private/blocked/reported entities must not leak, fixtures must not silently become production data, and tests must not be weakened.
- Canonical discovery engine is src/lib/supply-engine.ts; Lovable inspection reported 612 lines and findSupply as the main export, with wrapper helpers. ADR docs/adr/001-canonical-supply-engine.md reinforces no second engine.
- life-lived-network CI workflow .github/workflows/verify.yml runs Bun install, lint, Vitest and build. The matching workflow path was not found in life-lived-network2.
- The inspected app has route families for map/home and place pages, ask/offer/help/earn, conversations/profile/auth, trips/journeys, sources/moderation and public sitemaps.
- Two ADR documents appear to use number 003; renumbering needs a deliberate human decision, not an incidental feature PR.

## Business-relevant capabilities and gaps

The app already stores business/service-related listing fields including organisation, provider_note, qualification_note, booking_state, booking_url, service_category, origin and demonstration. Existing consent-based connection request/message flows and moderation/blocking concepts may provide a safer foundation than introducing a parallel lead-capture system.

The connected-project inspection found no obvious in-app analytics calls for analytics, track(, posthog or gtag in src. This is a text search, not a complete instrumentation audit. The inspection did not independently verify database row-level security, backend exposure settings, retention behavior or production data integrity.

Gaps worth validating:
- no confirmed business identity claim/ownership flow;
- no dedicated, privacy-reviewed enquiry-attribution mechanism;
- no settled policy for paid visibility;
- service taxonomy/regulated qualification mapping needs end-to-end review;
- product event/qualified-action baseline is not yet established.

## Safest first product improvement candidate

Add a service-only **“Who provides this / How to enquire”** section to the existing entry sheet using fields already present. Show organization and provider notes as supplied information; label qualifications **“Stated by provider”** unless independently verified. Show missing fields as “Not stated”; retain existing trust chips, demonstration labeling and regulated-category caveats. External booking links should be clearly identified and opened safely. This should not add schema, tracking, payment, ranking changes or a second discovery engine.

Likely files to inspect when implementation is approved:
- src/components/entry-sheet.tsx
- src/lib/services.ts
- src/lib/services.test.ts
- tests covering src/lib/supply-engine.ts

Acceptance criteria:
- only appears for service entries;
- no missing or unknown fact is inferred;
- qualifications are not upgraded to verified;
- regulated-category guardrails remain;
- demonstration entries remain visibly labeled;
- supply engine ordering and filtering do not change;
- keyboard access, clear labels and readable mobile layout;
- relevant unit tests, existing lint, test and build all pass in CI.

## Owner decisions

1. Confirm which GitHub repository is the canonical Lovable-connected source (life-lived-network or life-lived-network2).
2. Confirm backend direction (the app's own plan reports an open A/B/C decision).
3. Confirm whether to implement the service provider/contact transparency block as the first small product PR.
4. Keep any future paid placement out of organic discovery ranking; require a separate reviewed architecture and trust decision.
