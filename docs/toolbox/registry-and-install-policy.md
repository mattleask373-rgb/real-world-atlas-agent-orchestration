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
