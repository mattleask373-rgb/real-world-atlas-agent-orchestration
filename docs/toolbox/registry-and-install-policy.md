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
