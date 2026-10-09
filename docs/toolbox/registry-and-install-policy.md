# AI Toolbox Registry and Install Policy

## Policy
A public repository or skill is a candidate resource, not an approved dependency. Evaluate it before installation and keep the smallest useful subset. Never execute an unfamiliar install script or grant broad repository, shell, customer-data or production permissions by default.

## Candidate registry
| Resource | Potential use | Required checks before adoption |
|---|---|---|
| [Marketing Skills](https://github.com/coreyhaines31/marketingskills) | SEO, copy, CRO and growth workflows | Verify current license, exact skill files, upstream changes, prompt quality and factuality |
| [Claude Ads](https://github.com/AgriciDaniel/claude-ads) | Advertising account audit assistance | Verify repository identity, license, platform/API permissions, data handling and current compatibility |
| [Dify](https://github.com/langgenius/dify) | Visual LLM workflow/app orchestration | Review deployment/security model, license for intended use, secrets, costs and maintenance burden |
| [Impeccable](https://impeccable.style/) | Design critique and interface quality | Verify current usage/install instructions; use against non-production samples first |
| [AI Hero — Grill Me](https://www.aihero.dev/skills-grill-me) | Challenge assumptions and refine requirements | Review output quality; keep as a critique step, not an approval authority |
| [OpenRig](https://openrig.dev/) | Potential agent orchestration | Verify repository/product status, security model, permissions and measured value before adopting |
| [PPT Master](https://github.com/hugohe3/ppt-master/blob/main/skills/ppt-master/SKILL.md) | Presentation generation | Verify license, required files and output rights |
| [VoiceStudio](https://voicestudio.sh/) | Audio workflows | Verify actual product, terms, voice/recording rights, privacy and unit economics |
| [Agent Reach](https://github.com/Panniantong/Agent-Reach) | Potential agent/reach workflows | Confirm canonical repository URL, maintained state, license and exact capabilities |
| [Brag](https://github.com/latent-spaces/brag) | Potential achievement/work-log support | Confirm canonical repository URL, maintenance, license and fit |
| [IdeaBrowser](https://www.ideabrowser.com) | Idea and market research | Validate claims against primary sources and customer interviews |
| [Late Checkout](https://latecheckout.agency/) | Agency/service business inspiration | Treat as reference material, not a software dependency |

**Status:** candidates only. Nothing in this registry should be read as installed, security-reviewed, licensed for every use, or production-approved. Verify each resource at the upstream source at time of adoption. Links that originally pointed to GitHub `/new/main` UI routes have been normalized to likely repository roots and must be confirmed before use.


| [PostHog](https://github.com/PostHog/posthog) | Product analytics, funnels, feature flags, session replay and experiments | Decide cloud vs self-host; review privacy/cookie consent, event schema, retention, hosting/maintenance and data residency |
| [OpenSEO](https://github.com/every-app/open-seo) | SEO research using external data providers, competitor/keyword/backlink workflows | Verify current repository, data provider costs/terms, API keys, outputs and commercial-use licence |
| [Invoice Ninja](https://github.com/invoiceninja/invoiceninja) | Invoicing and client operations for the service business | Check its source-available/commercial licensing and white-label terms carefully; do not assume all features are unrestricted FOSS |
| [Cal.diy](https://github.com/calcom/cal.diy) | Scheduling and booking flows | Confirm project status, deployment requirements, licensing and fit versus a simple calendar link |
| [Autumn](https://github.com/useautumn/autumn) | Subscription, credit and usage-based billing for a future SaaS | Use only if product billing complexity justifies it; review hosted dependencies, Stripe/data handling, licence and migration path |
| [Typebot](https://github.com/baptisteArno/typebot) | Conversational lead capture, intake and qualification | Review licence, hosting, data processing, integrations and human handoff |
| [Frappe CRM](https://github.com/frappe/crm) | CRM and pipeline management | Compare with existing CRM needs; review stack/deployment burden, licence and integration cost |
| [Mautic](https://github.com/mautic/mautic) | Email marketing automation and lead nurture | Defer until consent, deliverability, suppression/opt-out, security updates and list governance are ready |
| [Chatwoot](https://github.com/chatwoot/chatwoot) | Customer support inbox and multi-channel conversations | Review deployment/maintenance, channel provider costs, access controls, retention and current licence |

## Additional candidates found while researching The Next New Thing AI
| Resource | Potential use | Priority / caution |
|---|---|---|
| [Codebase Memory MCP](https://github.com/DeusData/codebase-memory-mcp) | Local codebase knowledge graph for AI coding agents; potentially reduces repeated repository exploration | **Evaluate early** on a disposable clone. It reads source and writes agent configuration; review scripts, permissions, release provenance and local policy before installation |
| [OpenMontage](https://github.com/calesthio/OpenMontage) | Agent-assisted production of video and marketing assets | **Later experiment** for original campaign assets; AGPL-3.0 requires legal review if modifying/distributing or integrating its code; verify media/voice rights and real per-asset costs |
| [Last30Days](https://github.com/mvanhorn/last30days) | Research recent public discussion/trends across supported sources | **Evaluate early** for market/customer research. Verify source availability, platform terms, credentials, privacy and reproducibility |
| Slowbooks (canonical upstream not yet verified) | Potential AI-assisted bookkeeping and receipt workflow | **Research only** until the canonical repository and accounting controls are verified; never delegate final bookkeeping/tax decisions to an unreviewed agent |
| [OpenCut](https://github.com/OpenCut-app/OpenCut) | Open-source video editing alternative for content production | **Watchlist**; check current maturity and whether headless/agent workflows are stable before adopting |
| [Marketing Skills](https://github.com/coreyhaines31/marketingskills) | SEO, copywriting, CRO and analytics skills for agents | **Evaluate early** on one real, measured landing-page or SEO task; verify current licence and install only needed skills |
| [AI job-search workflow example](https://github.com/MadsLorentzen/ai-job-search) | Reference for structured opportunity discovery and tailored application workflows | **Research only**; private user data must never be committed to a public fork or shared with agents without explicit authorization |

**Stack-selection rule:** prefer existing project capabilities over adding a new platform. In particular, compare PostHog with current analytics; compare Typebot with existing form/chat functionality; compare CRM/support tools before deploying either; do not introduce both Autumn and another billing system without a clear architecture decision. External API/data-provider fees still apply even when a repository is free.

## Review checklist
1. Confirm exact upstream project and recent activity.
2. Read license and determine whether intended commercial use, modification and redistribution are permitted.
3. Inspect install scripts, dependencies, filesystem/network behavior and requested permissions.
4. Determine what data leaves the environment and which provider retains it.
5. Test on synthetic or non-sensitive data in an isolated environment.
6. Record versions/commit, files copied, configuration, owner, cost, limitations and removal procedure.
7. Run regression/security checks and obtain reviewer approval.
8. Pin versions where practical and schedule a review date.
9. Remove unused skills and revoke unused credentials.

## Acceptance test
Adopt only if a bounded test demonstrates improved quality, reduced cycle time or increased business value after accounting for setup, model/API cost, review and maintenance.


## Additional landscape candidates (research only)

These entries are candidates from the holistic landscape review. They are not installed, security-reviewed or production-approved. Use the complete prioritization, acceptance tests and rollout order in [the open-source gems landscape](../research/open-source-gems-landscape.md).

| Resource | Capability | Initial priority | Required adoption check |
|---|---|---|---|
| [Gitleaks](https://github.com/gitleaks/gitleaks) | Secret scanning | P0: evaluate report-only | Scan locally; protect findings; rotate any confirmed exposed credential |
| [Renovate](https://github.com/renovatebot/renovate) | Dependency-update PRs | P0: evaluate one repo | Conservative update config, CI validation, no autonomous merge |
| [Playwright](https://github.com/microsoft/playwright) | Browser end-to-end testing | P0: use existing suite first | Add only missing critical-journey coverage; synthetic/test accounts |
| [axe-core](https://github.com/dequelabs/axe-core) | Automated accessibility checks | P0: targeted audit | Pair automated output with manual keyboard/accessibility review |
| [SiteOne Crawler](https://github.com/janreges/siteone-crawler) | Technical SEO/site crawl | P1: test on owned site | Check scope, rate, crawl output and false positives |
| [Unlighthouse](https://github.com/harlan-zw/unlighthouse) | Site-wide Lighthouse audits | P1: alternative to SiteOne for a different need | Avoid overlapping audits without additional signal |
| [SerpBear](https://github.com/towfiqi/serpbear) | Rank tracking | P1: small query sample | Confirm SERP data provider, cost, geography and data handling |
| [Umami](https://github.com/umami-software/umami) | Lightweight web analytics | P1: only if current analytics are insufficient | Privacy/consent, hosting, retention and migration review |
| [Last30Days skill](https://github.com/mvanhorn/last30days-skill) | Recent public-signal research | P1: compare against manual sample | Verify source access, terms, credentials, reproducibility and costs |
| [Crawl4AI](https://github.com/unclecode/crawl4ai) | Structured web extraction | P1: public pages only | Follow site terms, robots guidance, rate limits and privacy/copyright rules |
| [Meilisearch](https://github.com/meilisearch/meilisearch) | Full-text/hybrid search | P1: benchmark only | Verify Community/Enterprise licence boundaries and benchmark against current search |
| [Trigger.dev](https://github.com/triggerdotdev/trigger.dev) | Durable TypeScript background jobs | P1: one non-critical workflow | Compare hosted/self-hosted costs, licence, retries, logs and approval controls |
| [Activepieces](https://github.com/activepieces/activepieces) | Visual integration automation | P1: alternative to Trigger.dev | MIT community core; verify commercial-edition boundaries and permissions |
| [Codebase Memory MCP](https://github.com/DeusData/codebase-memory-mcp) | Codebase graph/context | P2: disposable clone only | Review install scripts and agent configuration writes |
| [LangGraph](https://github.com/langchain-ai/langgraph) | Stateful agent orchestration | P2: architecture evaluation only | Adopt only if current workflow needs durable state/checkpoints/approval it lacks |
| [OpenTelemetry JS](https://github.com/open-telemetry/opentelemetry-js) | Workflow tracing/metrics | P2: only if observability is fragmented | Keep instrumentation proportional to a real debugging need |
| [Typesense](https://github.com/typesense/typesense) | Search and faceted discovery | P2: compare with Meilisearch, not alongside by default | Review licence, operations, indexing and representative relevance tests |
| [Twenty CRM](https://github.com/twentyhq/twenty) | CRM/pipeline | P2: compare with Frappe CRM | Use synthetic data; check current licence, export and operational burden |
| [Frappe CRM](https://github.com/frappe/crm) | CRM/pipeline alternative | P2: compare with Twenty | Select at most one CRM and only when follow-up is a real bottleneck |
| [listmonk](https://github.com/knadh/listmonk) | Opt-in newsletter infrastructure | P2: defer until audience exists | AGPL-3.0; consent, suppression, deliverability, hosting and provider cost |
| [OpenCut](https://github.com/OpenCut-app/OpenCut) | Video editing | Watchlist | Verify maturity and output workflow before production content use |
| [OpenMontage](https://github.com/calesthio/OpenMontage) | Agent-assisted video creation | Watchlist | AGPL-3.0 review plus media/voice/music rights and cost |

**Do not turn this registry into a shopping list.** First-wave focus is repository hygiene, baseline measurement, one technical SEO audit, one research workflow and one paid customer experiment. For all candidates, check upstream license and latest release at the time of use.


## Business portfolio and local-growth research candidates

These additional repositories are research leads connected to the [business portfolio strategy](../strategy/business-portfolio-feedback-loop.md). They are not approved, installed or production-ready by default.

| Repository | Potential role | Initial decision |
|---|---|---|
| [WAT SEO pipeline](https://github.com/Carbide-and-Dirt/wat-seo-pipeline) | Local competitive audits, prospect research and recurring geo-grid reporting | **A1 trial candidate**: inspect source/license, API costs, budget caps, data handling and outreach steps; one-target dry-run only |
| [LaunchDesk](https://github.com/imperator-clawdius/launchdesk) | Offer hypothesis and lead-stage cockpit | **A2 workflow inspiration**: compare with existing task/experiment docs first; small early project, don't add as dependency without demonstrated time savings |
| [All-In-One Free SEO Tool](https://github.com/IamRamgarhia/All-In-One-Free-SEO-Tool) | Broad local SEO/reporting toolkit | **A3 sandbox-only**: early project; no security policy detected at research time; inspect dependencies, API use and autonomous-fix behavior; no production credentials |
| [Creator CRM](https://github.com/alongot/creator-crm) | Creator/partner relationship tracking | **Defer**: simple shared-password gate and creator contact data require security/auth/privacy review; only relevant if partner pipeline becomes a bottleneck |
| [OpenSEO](https://github.com/every-app/open-seo) | SEO research and workflows | Compare against one independent audit; check current project maturity and all data-provider costs |
| [SiteOne Crawler](https://github.com/janreges/siteone-crawler) | Technical site crawl | Use on owned/authorized sites; compare to Unlighthouse rather than duplicating tools |
| [Unlighthouse](https://github.com/harlan-zw/unlighthouse) | Site-wide Lighthouse/performance audit | Select when its output answers a specific gap not already covered |
| [Twenty CRM](https://github.com/twentyhq/twenty) **or** [Frappe CRM](https://github.com/frappe/crm) | Pipeline and follow-up | Choose one only if a lightweight tracker is no longer sufficient |
| [Activepieces](https://github.com/activepieces/activepieces) **or** [Trigger.dev](https://github.com/triggerdotdev/trigger.dev) | Workflow automation | Choose one only after manual workflow proves repeatable and a bottleneck is measured |

The portfolio strategy contains the complete business use cases, scoring, 14/30/60/90-day gates, UK outreach safeguards and the shared economics scorecard. Do not deploy the WAT pipeline for broad lead collection until legal basis, provider terms, cost ceilings and contact rules have been reviewed. UK ICO guidance states that publicly available contact details do not automatically authorize marketing, and rules differ for corporate subscribers versus sole traders/ordinary partnerships: https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-communications/guidance-on-direct-marketing-using-electronic-mail/
