# Business Empire Execution Backlog

**Status:** active planning and validation backlog; no revenue, customer validation, installation, or production changes are implied by inclusion here.
**Owner:** founder-led; each workstream requires a named human owner before production or customer-facing actions.
**Operating rule:** one core network, one near-term cash engine, and a gated portfolio of adjacent revenue streams. Do not build or launch every line simultaneously.

## North-star architecture

Real World Atlas / Life Lived Network is the core trust, discovery, and participation asset. All adjacent businesses must either (a) generate cash that funds the network, (b) improve verified local supply and customer outcomes, or (c) produce reusable distribution, data quality, workflow, or software assets.

Feedback loop: research → buyer conversations → paid service delivery → verified improvements and local insight → more useful network discovery → qualified actions and participation → transparent monetization → reinvestment in quality, trust, accessibility and product → reusable playbooks/software.

## Portfolio: every income path tracked

| ID | Business line | Initial offer / revenue model | Status | Gate before scaling |
|---|---|---|---|---|
| B1 | Local-business visibility and enquiry service | Fixed-scope audit, prioritized fixes, conversion-path review, before/after report | **First commercial experiment** | 5+ qualified buyer conversations; paid pilot; measured outcome, time, costs and margin |
| B2 | Recurring visibility and conversion care | Monthly monitoring, listing accuracy, site health, reporting and agreed maintenance | Hypothesis | B1 shows measurable value and a recurring job |
| B3 | Real World Atlas verified local profiles | Free accurate baseline listings; optional paid business features | Product strategy / validate | Correction and verification process, user value, clear separation of paid status and trust |
| B4 | Transparent sponsorship and qualified enquiries | Clearly labelled sponsorship or contractually defined qualified referrals | Deferred | User demand, attribution, consent/data rights, lead-quality definition and trust safeguards |
| B5 | Digital products and templates | Audit checklists, reporting packs, onboarding guides, local launch kits | Deferred | Repeated delivery exposes reusable work; at least one real buyer signal |
| B6 | Narrow workflow automation / implementation | One trade-specific workflow such as enquiry routing or quote follow-up | Deferred | Repeated manual workflow, customer authorization, rollback and measurable benefit |
| B7 | Niche micro-SaaS | Profile completeness, enquiry attribution, onboarding/verification or a proven workflow tool | Not build-approved | Repeated independent demand; at least two paid concierge/prototype users before material build |
| B8 | Creator/partner ecosystem | Partner referrals, creator collaborations, local guide contributions | Deferred | Useful audience, explicit agreements, disclosure and repeatable attribution |
| B9 | Content, guides, audio/transcription/translation | Useful local guides and permissioned media services | Optional experiment | Rights/consent, quality review, distribution path and positive delivery economics |
| B10 | Ethical affiliate and referral income | Relevant tools/services with clear disclosure | Deferred | Genuine user fit, transparent disclosure and no ranking manipulation |
| B11 | Permissioned newsletter/community updates | Opt-in local updates and sponsored editions | Deferred | Audience permission, preference center, unsubscribe/suppression and measurable usefulness |
| B12 | Research and data insights | Aggregated, privacy-protective reports or local trend insights | Long-term hypothesis | Lawful data rights, meaningful aggregation, minimum cohort rules and demonstrable buyer value |

Do not describe hypotheses as active revenue streams. No fabricated testimonials, listings, reviews, availability, outcomes or verification badges. Do not resell personal data or make paid placement look like independent recommendation.

## Workstreams and deliverables

### W0 — Governance, repository source of truth, security
1. Compare `life-lived-network`, `life-lived-network2`, and related repos; identify canonical source, deployment target, branch protections, active work and divergence.
2. Read each active repo's `AGENTS.md`, `docs/agents/INVARIANTS.md`, ADRs, product constitution and CI workflow before app changes.
3. Preserve PR-only external collaboration, independent review, no force-push/rewrite of published history, and no autonomous merge to main.
4. Review repository history and secret handling without echoing secret values; privately rotate any confirmed exposed credentials.
5. Establish baseline for build, lint, tests, accessibility, errors, analytics, core journeys, SEO and current revenue.
6. Do not modify generated Supabase integration files, route tree, env files or Supabase config; do not create a second discovery/supply engine.

### W1 — First paid pilot
1. Choose one reachable, non-regulated local-business segment and one specific discovery/enquiry problem.
2. Record 20 dated public pain signals across at least three relevant communities/sites, including counterexamples.
3. Conduct 5–10 buyer conversations; ask about frequency, impact, current workaround, prior spend and decision process.
4. Offer a bounded paid pilot before building SaaS. The £250–£750 range is a test hypothesis, not a validated market rate.
5. Use existing first-party analytics/Search Console where authorized; manual QA plus one audit tool.
6. Report baseline, actions, outcome, cash collected, refunds, delivery hours, API/hosting costs, gross margin, rework and customer feedback.
7. Do not promise rankings, leads or revenue. No bulk unsolicited outreach; review current UK ICO/PECR/UK GDPR obligations before any campaign.

### W2 — Product and network improvements
1. Select one existing user journey from discovery to a meaningful real-world action.
2. Baseline mobile UX, accessibility, empty/error states, trust, analytics and search discoverability.
3. Make a narrowly scoped improvement after architecture review; tests and independent review required.
4. Prioritize accurate local data, correction/report flows, clear availability/qualification semantics and transparent sponsorship.
5. Never let fixtures silently become production data or treat raw provider responses as application truth.

### W3 — Research and content
1. Maintain an evidence ledger: source URL, date, claim, evidence type, counterexample, confidence and next test.
2. Complete the Next New Thing channel review systematically; distinguish full transcripts/descriptions from summaries and log all canonical repo links.
3. Publish only genuinely useful, fact-checked content with source review, rights and human approval.
4. Track qualified actions and corrections, not content volume, stars or pageviews alone.

### W4 — Tooling and agent factory
1. Inventory current built-in capabilities before introducing new infrastructure.
2. For each repo, record canonical URL, license/edition, release/activity, security policy, install scripts, dependencies, permissions, outbound data, provider/API costs, hosting and rollback.
3. Trial only in disposable clones with synthetic data and explicit budgets; compare against a manual baseline.
4. Add agents only for well-defined tasks with inputs, output schema, acceptance criteria, stop conditions, audit trail and human escalation.
5. No autonomous merges, public publishing, spending, bulk outreach, or irreversible customer actions.
6. Maintain one registry with status: idea → researched → security/license reviewed → sandboxed → benchmarked → approved → retired. Inclusion does not equal approval.

### W5 — Commercial operations
1. Keep a lightweight pipeline until volume proves a CRM is needed.
2. Standardize proposal, scope, exclusions, customer approvals, delivery checklist, report, support boundaries, invoicing and feedback.
3. Track cash collected, refunds, direct/API/hosting costs, founder hours, effective hourly return, gross margin, repeat purchase and customer outcomes.
4. Set a weekly continue / adjust / stop decision for each experiment.
5. Add recurring plans only when ongoing value and service capacity are proven.

### W6 — Trust, compliance and finance
1. Separate organic recommendations from sponsored placements; label paid content prominently.
2. Use explicit agreements and documented attribution for referrals; never share personal data without a valid basis and clear expectations.
3. Review UK marketing/privacy rules with current ICO guidance; public contact details are not blanket permission to market.
4. Use data minimization, retention/deletion, access controls, suppression/opt-out handling and incident response.
5. Record income, VAT/tax questions, expenses, refunds and cash runway with appropriate professional advice when needed.
6. Regulated categories require end-to-end qualification safeguards; exclude or caveat unverified qualifications.

## Candidate open-source toolbox — research queue, not installation approval

### First-wave fit
- [WAT SEO pipeline](https://github.com/Carbide-and-Dirt/wat-seo-pipeline): local SEO audit/prospect/report workflow. **Sandbox only** until code, license, API costs, data handling and outreach features are reviewed.
- [OpenSEO](https://github.com/every-app/open-seo): SEO workflow comparison; validate what is actually free and what relies on paid APIs.
- [SiteOne Crawler](https://github.com/janreges/siteone-crawler) **or** [Unlighthouse](https://github.com/harlan-zw/unlighthouse): choose one first based on whether broad crawl findings or performance evidence is the primary need.
- [Last30Days](https://github.com/mvanhorn/last30days-skill): research candidate; benchmark against manual source collection.
- [Gitleaks](https://github.com/gitleaks/gitleaks): report-only secret scan first.
- [Renovate](https://github.com/renovatebot/renovate): dependency PR automation only after CI and ownership review.
- [Playwright](https://github.com/microsoft/playwright) and [axe-core](https://github.com/dequelabs/axe-core): use where existing e2e/accessibility coverage has a demonstrated gap.
- [Umami](https://github.com/umami-software/umami) or [PostHog](https://github.com/PostHog/posthog): compare against existing analytics before adding either.
- [Meilisearch](https://github.com/meilisearch/meilisearch) or [Typesense](https://github.com/typesense/typesense): benchmark-only; do not replace or duplicate canonical supply/discovery engine without ADR and evidence.

### Conditional business operations
- [LaunchDesk](https://github.com/imperator-clawdius/launchdesk): inspiration for offer/lead tracking; early project, optional only.
- [Frappe CRM](https://github.com/frappe/crm) or [Twenty](https://github.com/twentyhq/twenty): select one only if lightweight tracking becomes insufficient.
- [Activepieces](https://github.com/activepieces/activepieces) or [Trigger.dev](https://github.com/triggerdotdev/trigger.dev): choose one only after manual workflow and exception paths are documented.
- [listmonk](https://github.com/knadh/listmonk): only for a permissioned audience and mature unsubscribe/suppression handling.
- [Invoice Ninja](https://github.com/invoiceninja/invoiceninja): evaluate only if existing invoicing cannot meet real needs.
- [Chatwoot](https://github.com/chatwoot/chatwoot): support tooling only when a measurable support burden exists.
- [Typebot](https://github.com/baptisteArno/typebot): forms/intake only after privacy, accessibility and existing product capabilities are reviewed.
- [Creator CRM](https://github.com/alongot/creator-crm): defer; inspect authentication and personal-data handling.
- [Cal.diy](https://github.com/calcom/cal.diy): evaluate only when scheduling is a proven bottleneck; verify license/terms.
- [Autumn](https://github.com/useautumn/autumn): billing/entitlement research only if existing billing architecture warrants it.
- [Mautic](https://github.com/mautic/mautic): defer until marketing operations and permission controls justify a heavier platform.
- [Codebase Memory MCP](https://github.com/DeusData/codebase-memory-mcp): sandbox codebase context evaluation.
- [OpenCut](https://github.com/OpenCut-app/OpenCut), [OpenMontage](https://github.com/calesthio/OpenMontage), [Penpot](https://github.com/penpot/penpot), [Excalidraw](https://github.com/excalidraw/excalidraw): creative tooling only if actual workflow needs it; review licenses, including AGPL where relevant.
- [n8n](https://github.com/n8n-io/n8n): license/use terms review required before any commercial adoption.
- [All-In-One Free SEO Tool](https://github.com/IamRamgarhia/All-In-One-Free-SEO-Tool): early-stage sandbox candidate only; verify claims, dependencies, permissions and automated fixes.

Do not install the whole list. Prefer existing platform features; add one tool at a time only when a measured gap and owner exist.

## 90-day sequencing

### Days 1–7: Establish baseline and choose focus
- Repository/source-of-truth audit, invariants, CI/security baseline.
- One target customer segment and one pilot offer.
- Tool/license review for one SEO candidate and one research workflow.
- Output: source-of-truth memo, baseline dashboard, buyer interview script, pilot scope and risk checklist.

### Days 8–14: Buyer discovery and offer
- 20 sourced pain signals; 5–10 buyer conversations; one written fixed-scope offer.
- No software build unless a buyer workflow genuinely requires a small prototype.
- Output: evidence ledger, objections/pricing notes, proposal template, go/no-go decision.

### Days 15–30: Deliver, measure, improve
- Deliver a paid pilot if sold; if not, document attempts and revise/stop rather than claiming traction.
- Improve one product journey with tests and review.
- Produce one SEO/content experiment with citations and human QA.
- Output: outcome report, unit economics, reviewed PR and experiment retrospective.

### Days 31–60: Repeat only what works
- Repeat pilot to test consistency; test recurring care with satisfied customers only where ongoing value exists.
- Create digital assets from repeated delivery; automate one stable workflow only if savings exceed maintenance burden.
- Add CRM or newsletter tooling only if volume and permissioned audience justify it.

### Days 61–90: Scale with gates
- Scale the service only with repeatable acquisition, positive margin and quality.
- Test transparent profile/sponsorship/enquiry model with trust and attribution controls.
- Prototype micro-SaaS only after repeated independent buyers and paid concierge validation.
- Output: portfolio review, continue/stop decisions, next-quarter budget and product roadmap.

## Weekly scorecard

For each offer: evidence strength; qualified conversations; offers; paid conversions; cash collected; refunds; direct/API/hosting costs; hours; gross margin; verified customer outcome; repeat purchase/retention; support burden; core-network effect (profile completeness, corrections, qualified actions, return usage); compliance/security incidents; next decision and owner.

## Immediate next actions (execution queue)

1. Compare the two app repositories and confirm canonical source before any code edits.
2. Read architecture decisions and CI configuration, then capture a no-secrets health/security baseline.
3. Choose a single local business segment; prepare interview script and fixed-scope offer.
4. Review WAT pipeline license/security/costs in a disposable environment; do not enable outreach.
5. Create the first evidence-led pilot deliverable and a customer-facing sample report using synthetic/example data clearly labeled as such.
6. Start weekly scorecard; record zero results honestly if no sale or outcome occurs.

## Explicit non-claims

No buyer interviews, paid conversions, revenue, production deployments, tool installations, customer outreach, or passing CI runs are claimed by this plan. These are execution targets and hypotheses until independently evidenced.
