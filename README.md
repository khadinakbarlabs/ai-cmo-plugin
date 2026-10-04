# Khadin AI CMO

![AI CMO icon](assets/icon.png)

By [Khadin Akbar](https://github.com/khadinakbarlabs).

AI CMO is an instruction-based marketing department for businesses and organizations across models, sectors, stages and sizes: strategy, content, ads, lead generation, inbound, outbound, account-based marketing, growth experiments, SEO, AI, virality, lifecycle, partners, field marketing and measurement.

## Agentic team

CMO coordinates six specialists: market intelligence, search, campaign production, growth analysis, campaign review and CLI execution. Multi-stage campaigns use a resumable task board, scoped handoffs, bounded delegation, review/repair and observed execution receipts. Small tasks use one skill. Read [the team workflow](skills/cmo/references/agentic-workflow.md). No executable runtime, MCP, installer or daemon is added. Native Claude agent wrappers are provider-specific; OpenAI uses shared role guides and actual host delegation or sequential fallback.

## Start

Ask: “Use AI CMO to understand my business at this website and create a 30-day growth plan with the first campaign assets.” Or choose a focused skill such as keyword research, link building, ad research or ad creation.

The package contains 39 focused skills covering 140 mapped workflow families. These are instruction workflows, not 140 separate executable tools. They work with supplied materials and supported host tools; connected execution requires your own accounts and external CLIs. No MCP server, hosted backend, bundled CLI, install hook or background daemon is included.

## Install from GitHub in Claude Code

Add the repository marketplace and install the plugin:

```text
/plugin marketplace add khadinakbarlabs/ai-cmo-plugin
/plugin install khadin-ai-cmo@ai-cmo-marketplace
```

Then invoke `/khadin-ai-cmo:cmo` and describe the business/outcome. GitHub installation is separate from approval in Anthropic's directory. The [GitHub release](https://github.com/khadinakbarlabs/ai-cmo-plugin/releases/tag/v0.4.3) supplies separate Claude and OpenAI ZIPs plus checksums. Use the OpenAI ZIP in the supported host upload/install surface; actual host permissions and CLI availability still apply.

## Anthropic first

This source package targets Claude with `.claude-plugin/plugin.json`. In Claude Code, load the folder with `claude --plugin-dir /path/to/ai-cmo`; invoke `/khadin-ai-cmo:cmo` or describe the task. This path is an example, not a hard-coded installation requirement. Test Cowork's actual CLI access before using connected workflows. Chat can use supported instruction/draft/import workflows; installing skills does not expose your computer's CLI.

## Business-model adaptation

Read the [20 business-model/sector profiles](skills/business-model-strategy/references/business-models.md), [custom and hybrid adaptation](skills/business-model-strategy/references/custom-model.md) and [marketing discipline map](skills/cmo/references/marketing-disciplines.md). B2B/enterprise, SaaS/apps, ecommerce/retail, local/services, manufacturing, creators, nonprofits, franchises and other models get different buyers, funnels, assets and metrics. New or regulated domains need current evidence and requirements; broad planning support does not certify every industry or tool.

## Tools

Apify Research uses verified public khadinakbar Actor contracts through the external Apify CLI. Review the dated Actor catalog, current schema and pricing before a run. Use your own Apify account; no credentials are bundled. Existing-run collection and launching a paid run are separate operations.

Social Publishing uses the external Postiz CLI. Install and authenticate through its current official documentation; discover exact accounts/settings before writing. Optional external CLI guides cover Resend email, WordPress publishing, Humanizer PRO copy revision and Agent Media generation. Other services use capability-gated procedures or useful imports/exports. They are not declared working integrations without actual tool/host evidence.

Store business state in a user-owned `.ai-cmo/` workspace, separate from this installation. Ordinary drafts/research follow your request; paid jobs and external actions respect your configured authorization and limits. No campaign is published just because a brief is complete.

## Evidence and limitations

Sources and current Actor contracts were inspected; connected paid runs and publication are not automatically tested during packaging. Consult the separate build report for executed checks. The 30-project benchmark guided breadth; representative workflow inspection is not an exhaustive semantic-parity claim. The original instructions adapt methods to a CLI-first design rather than bundling upstream MCP services.

## OpenAI version

After Anthropic validation, an isolated OpenAI bundle is generated from the same reviewed skills. Codex CLI execution and ChatGPT host support require separate checks. Do not rename a manifest and assume equivalent execution.

See PRIVACY.md, SECURITY.md, SUPPORT.md, TERMS.md and THIRD-PARTY-NOTICES.md for package boundaries and source attribution.

The component budget is 39 discoverable skills, 6 native Claude agents and 0 separate commands. Specialized inbound, outbound, lead generation, ABM, growth, virality, AI and field workflows are reference guides inside their owners, preserving the 140 mapped workflows. This follows a conservative local release profile rather than a verified platform maximum.

## Context, learning and reporting

AI CMO v0.4.3 includes a [continuous learning loop](skills/cmo/references/learning-loop.md): source-aware business context, explainable next actions, concise session handoffs, optional local feedback and editable visual reports. Ask "What should we do next?", "Continue where we left off", "Show progress" or "Review this every week". Existing skills handle these flows; no extra skill/command inventory is added.

Recurring reviews require a verified host scheduler and concrete scope. The package includes recipes and registration checks, not an executor. Feedback remains in your workspace unless you explicitly request a specific external delivery. The report template has no scripts, tracking or external network assets. See [the user experience guide](skills/cmo/references/user-experience.md). These features are instructions/templates; behavioral effectiveness, unattended execution and a 10× improvement are not established by packaging.

## Publication and support

This repository is the public Claude source. The OpenAI release ZIP carries matching shared skill instructions with provider-specific metadata and icons; it omits native Claude wrappers. External CLIs are installed/authenticated separately by the user. [Support](SUPPORT.md), [privacy policy](PRIVACY.md), [terms](TERMS.md), [release validation](RELEASE-VALIDATION.md) and [release history](CHANGELOG.md) document the package. Directory submission, review and public listing are distinct; consult the live portals for their status. No marketing performance improvement is guaranteed.

## Research access limits

All 38 owned Actor routes remain mapped. Their schemas are supported public-mode projections rather than complete upstream schemas. Sixteen acquisition-unverified routes support authorized imports only; the other 22 require evidence of a provider-permitted access method before launch. Login/session secrets and gated retrieval inputs are excluded. See the Apify research catalog for exact per-route limits.
