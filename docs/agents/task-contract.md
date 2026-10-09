# Standard Agent Task Contract

Every delegated task must include the following fields.

## Request
- **Task ID / title:**
- **Owner role:**
- **Business or user outcome:**
- **Why now / priority:**
- **Deadline and budget/tool limits:**

## Context
- **Source of truth / repository:**
- **Required docs read:** `AGENTS.md`, invariants, relevant ADRs, product constitution and CI.
- **Relevant files, routes, data and prior decisions:**
- **Evidence and links:**
- **Known assumptions / unknowns:**

## Boundaries
- **In scope:**
- **Out of scope:**
- **Allowed tools and data:**
- **Forbidden actions:**
- **Dependencies / other owners:**
- **Risk level:** low / medium / high.
- **Stop and escalate if:** destructive change, new dependency, schema migration, new permission, unexpected secret/data exposure, cost increase, unclear source of truth, or scope expansion.

## Acceptance criteria
Write observable conditions, not vague goals. Include expected behavior, edge cases, accessibility where relevant, analytics, and how success is measured.

## Verification and handoff
- Tests, lint, build and checks run (with results).
- Files changed and concise rationale.
- Evidence for each acceptance criterion.
- Security, privacy, licensing and factuality considerations.
- Known limitations, risks and rollback path.
- Follow-up tasks and named reviewer.

## Definition of done
- Acceptance criteria are met or failures are explicitly documented.
- Relevant tests are added/updated and run; no weakening of existing tests to force a pass.
- No secrets, unrelated edits or unauthorized data collection.
- Independent review completed for code or public-facing claims.
- Required human approvals are recorded before release.
- Monitoring and rollback are defined for production changes.
