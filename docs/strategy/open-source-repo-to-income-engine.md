# Open-Source Repository → Agent Capability → Income Engine

## Purpose

Turn useful repositories featured by The Next New Thing AI into a controlled research and delivery pipeline for Real World Atlas / Life Lived Network and the wider AI-assisted service business. The objective is not to install everything: it is to discover capabilities, test one real use case, prove customer value, then productize what works.

**Research status (9 October 2026):** the channel page exposes a large catalogue (the public channel listing showed 339 videos at research time), and searchable transcript/summary pages were available for a subset. This is a working integration of the accessible repo-focused videos and the earlier research list, **not a verified exhaustive extraction of every video's full description**. Descriptions and repository links must be systematically inventoried before this subsection is marked complete. Start with the video catalogue and linked summary pages in `docs/research/next-new-thing-channel-review.md`.

## Operating loop

1. **Discover:** research agent records video title, date, canonical video URL, repository URLs from description, transcript/summary URL, claimed use, and the exact timestamp/quote or source passage supporting the claim.
2. **Resolve:** repository scout opens the upstream GitHub repository, verifies owner/name, licence, latest activity/releases, security notices, install method, data flows, external services and operating costs.
3. **Map to a capability:** classify each candidate as product delivery, engineering/QA, SEO/research, lead acquisition, sales/CRM, support, billing/finance, content/media, or infrastructure.
4. **Rank:** score business relevance, time-to-value, evidence quality, implementation effort, security/privacy risk, licence risk, ongoing cost, and reversibility. Popularity is not a score substitute.
5. **Run one bounded trial:** use a disposable clone or synthetic/non-sensitive data; record baseline, task, output quality, time saved, cost, errors, review burden and removal steps.
6. **Accept or reject:** adopt only if the trial beats the baseline and has an owner, a documented rollback path and a human reviewer. Otherwise record the rejection and reason.
7. **Turn capability into an offer:** use validated workflows to deliver a specific outcome to a defined customer segment. Charge for the outcome and service boundary, not the repository or number of agents.
8. **Measure and repeat:** record qualified leads, paid conversions, revenue collected, delivery hours, direct/API costs, gross margin, repeat use, customer outcome, incidents and support burden.

## Agent roles and output contracts

- **Repository Scout:** one candidate record per repo; no installation or code execution. Must provide canonical URL, licence evidence, maintenance evidence, dependency/install risks and open questions.
- **Video Researcher:** maps video → description link → repo → transcript evidence. Never marks a video reviewed if only a title or third-party summary was seen.
- **Product/Architecture Reviewer:** identifies overlap with existing Life Lived Network functionality and rejects duplicate platforms without a decision record.
- **Trial Engineer:** runs isolated, reversible tests; records commands, commit/version, environment assumptions, results and cleanup.
- **Growth Operator:** maps validated capability to one customer pain, one offer, one acquisition channel and one measurable conversion event.
- **QA/Privacy Reviewer:** checks correctness, privacy, licensing, security, accessibility, consent and customer-data handling independently.
- **Chief of Staff:** maintains the candidate backlog, owners, budgets, review dates and continue/stop decisions.

Every task uses the existing agent task contract. No agent can independently install to production, change credentials, publish public content, send bulk outreach, spend money, issue refunds, or make binding financial/accounting decisions.

## Capability portfolio and income hypotheses

| Capability | Candidate projects / sources | First practical test | Potential income path | Gate before scaling |
|---|---|---|---|---|
| SEO and market evidence | [OpenSEO](https://github.com/every-app/open-seo), [Last30Days](https://github.com/mvanhorn/last30days-skill), [Marketing Skills](https://github.com/coreyhaines31/marketingskills) | One authorized site audit and one customer/problem research brief; independently verify every factual claim | Fixed-scope local visibility audit, SEO/content improvement, recurring reporting only if results justify it | Real data sources, API cost, licence, privacy, factuality and measured client outcome |
| Lead acquisition and conversion | Hyper Agent workflow discussed in [the channel's client-finding episode](https://glasp.co/youtube/pIyqwrZ0x8Y); [Typebot](https://github.com/baptisteArno/typebot) | Manually review a small prospect set; prototype an intake flow with synthetic leads | Paid website/enquiry audit, lead-capture setup, conversion improvement | No mass unsolicited automation; consent, opt-out, relevant targeting and human review |
| Product analytics | [PostHog](https://github.com/PostHog/posthog) | Audit current analytics first; if a real gap exists, instrument one funnel in a test environment | Evidence-backed CRO service and measurable product improvement | Consent/privacy, event quality, retention, hosting and operating cost |
| Delivery and client management | [Frappe CRM](https://github.com/frappe/crm), [Chatwoot](https://github.com/chatwoot/chatwoot), [Cal.diy](https://github.com/calcom/cal.diy) | Map current lead → proposal → delivery → support process before selecting one system | More reliable service delivery and retention; these tools are enablers, not standalone revenue | Choose the smallest set; avoid overlapping CRM/support/booking systems |
| Billing and financial operations | [Invoice Ninja](https://github.com/invoiceninja/invoiceninja), [Autumn](https://github.com/useautumn/autumn), Slowbooks (canonical upstream still to verify) | Compare existing accounting/invoicing needs; test invoice workflow with dummy data only | Collect payment reliably; later usage-based SaaS billing if a validated product exists | Verify commercial terms; reconcile financial records; human approval for accounting, tax and payment actions |
| Content and media | [OpenMontage](https://github.com/calesthio/OpenMontage), [OpenCut](https://github.com/OpenCut-app/OpenCut), [Listmonk](https://github.com/knadh/listmonk) | Produce one original, rights-cleared asset or opt-in email draft, then review manually | Content-led acquisition, newsletter, reusable content kits, optional production service | Rights, licensing, email consent/deliverability, quality and per-asset costs |
| Coding and QA leverage | [Codebase Memory MCP](https://github.com/DeusData/codebase-memory-mcp), [Grill Me](https://www.aihero.dev/skills-grill-me), [Archify](https://github.com/archify/archify) (verify canonical upstream before use), [Worktrunk](https://github.com/max-sixty/worktrunk) (verify current upstream before use) | Known-question benchmark on a disposable clone; a narrow plan → implementation → tests → independent review cycle | Lower delivery cost and faster, more reliable client/product work | Do not weaken tests or bypass PR review; audit code access and agent configuration writes |
| Agent orchestration and memory | Paperclip, Hindsight, Buzz, OpenViking, Semantica, SwitchYard and related projects mentioned in repo roundups; resolve canonical URLs before adding as dependencies | First document the gap in current GitHub + project docs; compare one candidate in isolation | Primarily internal leverage; may later underpin a workflow implementation offer | No new control plane without a measured coordination/context problem; permissions and auditability first |
| Productized knowledge and digital goods | Research notes, reviewed templates, local-business checklists, workflow packs | Interview potential buyers or pre-sell a narrow deliverable before building a catalogue | One-off digital product or add-on to a service engagement | Clear audience, rights to included assets/data, demonstrated willingness to pay |

**Important:** a repository is not itself a business model. Revenue requires a customer, a costly problem, a credible outcome, distribution, delivery quality and positive unit economics.

## Priority order for the first 30 days

1. **Baseline and source of truth:** compare `life-lived-network` and `life-lived-network2`; read repository instructions and map existing analytics, forms, CRM and deploy architecture.
2. **One growth-evidence trial:** test OpenSEO or an equivalent current workflow on a single authorized site; compare results with Search Console/first-party data and log any API costs.
3. **One research trial:** test Last30Days or manual research for one clearly framed customer/market question. Treat third-party platform access and scraped data as a privacy/terms review item.
4. **One engineering trial:** evaluate codebase-memory-MCP or a planning/QA skill on a disposable clone and a known task. Do not write its configuration into the production repository until approved.
5. **One revenue test:** offer a bounded, fixed-scope local-business visibility/enquiry pilot to a small, manually reviewed prospect list. Use truthful, individualized contact and record paid outcomes, time and margin.
6. **Only after the first workflow works:** decide whether a CRM, chat inbox, booking system, invoicing tool or newsletter platform is genuinely missing. Choose at most one per capability area.
7. **Weekly review:** stop tools and offers that fail to improve measured outcomes; expand only the workflows with repeatable value.

## Repo/video inventory acceptance criteria

The channel sweep is complete only when the inventory includes, for every accessible video in scope:
- video title, published date and canonical URL;
- whether a full description was inspected;
- every repository/code link extracted from that description;
- transcript inspected vs third-party summary only vs inaccessible;
- canonical upstream repository, licence, maintenance/security review status;
- capability category, experiment hypothesis, priority and owner;
- disposition: backlog, trial, adopted, rejected or blocked, with reason.

Do not infer that a video contains a repo merely from its title. Do not mark the whole channel reviewed until the accessible video list has been paginated and descriptions have been checked systematically. Private, removed or inaccessible videos must be listed as coverage gaps, not silently omitted.
