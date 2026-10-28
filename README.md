# AI CMO: Marketing, Ads & SEO

![AI CMO logo](assets/icon.png)

By [Khadin Akbar](https://github.com/khadinakbarlabs).

AI CMO is an AI marketing assistant for SEO, content marketing, advertising research, lead generation, email and social media campaigns. Turn an inline business brief or pasted marketing table into reviewed copy, campaign plans, keyword opportunities and clear performance reports.

Work adapts to business models, industries, team sizes and buying cycles. Small tasks go directly to a specialist; larger campaigns use a coordinated plan with six specialist roles. This is planning and production support, not a guarantee of rankings, sales, virality or regulatory approval.

## What you can do

- **SEO and keyword research:** organize search intent, content topics, technical SEO findings, local search priorities and link-building opportunities. Keyword volumes and backlink metrics require actual source data.
- **Content and ad copy:** create landing-page copy, articles, newsletter drafts, ad variants, design briefs and creator scripts with source-backed claims.
- **Lead generation and outbound planning:** qualify companies from bounded company rows pasted inline, preserve source IDs and suppression, and prepare reviewed outreach drafts. Contact lookup and sending are separate operations.
- **Campaigns and growth:** plan inbound, outbound, ABM, lifecycle, referral, launch, partnership and field-marketing experiments with business-appropriate conversions.
- **Marketing analytics:** calculate compatible campaign metrics, explain unknowns and produce editable Markdown, CSV or design-only visual reports.

## Try it without connecting an account

1. “Using this brief, write a landing-page headline and two ad variants. Use only the features I supplied.”
2. “Analyze this campaign table: 1,000 impressions, 50 clicks, $100 spend and 5 conversions. Calculate CTR, CPC and CPA, and mark missing metrics unknown.”
3. “Qualify these three companies against this ICP. Preserve CRM IDs and do-not-contact flags; keep missing mandatory fit evidence unknown.”
4. “Plan a 30-day content campaign for this business and write the first two posts.”
5. “Resume this campaign from the task state I paste here. Reuse completed work and report the next action.”

No login or paid Actor sample is required for inline-data analysis, planning or copy. Return a complete result inline, or save a requested task artifact in the user's selected workspace. Do not create personal profiles, save conversations, extract Claude history/memory or query user-generated/uploaded files. File-analysis routes are disabled; paste only the bounded relevant data inline.

## Install from GitHub in Claude Code

```text
/plugin marketplace add khadinakbarlabs/ai-cmo-plugin
/plugin install khadin-ai-cmo@ai-cmo-marketplace
```

Then invoke `/khadin-ai-cmo:cmo` or a focused specialist. The installation ID remains `khadin-ai-cmo`; the public display name is descriptive and does not change existing invocations. GitHub availability is separate from directory approval.

## Anthropic first

The canonical package uses `.claude-plugin/plugin.json`, 39 skills and six native Claude agents. There are zero separate commands, bundled CLIs, MCP servers, hooks, installers or background services. Claude Code can load the package with `--plugin-dir`; other surfaces need their own capability verification. Six role files do not prove that independent agents ran. See [host editions](HOSTS.md).

## Business-model adaptation

Use the [20 business-model profiles](skills/business-model-strategy/references/business-models.md), [custom/hybrid adaptation](skills/business-model-strategy/references/custom-model.md) and [marketing discipline map](skills/cmo/references/marketing-disciplines.md). These guides adapt the funnel and assets; they do not certify sector expertise. Regulated claims need current authoritative evidence and appropriate professional review. Do not make individual healthcare, credit, employment, legal or financial eligibility decisions or target people using sensitive personal traits.

## Tools

Connected tools are optional and user-requested. Use an external user-installed CLI only when the actual host supports it, the destination meets the [directory service-admission gate](skills/cmo/references/directory-boundaries.md), and the exact data/effect/cost scope is authorized. Unsupported or unverified integrations receive a complete draft/import or manual handoff. The package does not install tools or connect accounts.

**Apify research:** [38 publisher-owned Actor routes](ACTORS.md) are catalogued. All public IDs/names were rechecked on 2026-10-28; no Actor was run. Sixteen routes are import-only. Twenty-two require provider-permitted acquisition evidence before launch, plus current schema/build/pricing and spending checks. Public visibility and input acceptance do not establish source-access rights. Do not use login cookies, gated retrieval, CAPTCHA bypass or proxy/identity failover. The creator publishes these Actors; calls can incur charges in the user's Apify account. Do not start paid samples or promote an Actor when pasted authorized rows already solve the task.

**Publishing and copy tools:** retained procedures cover Postiz for an authorized destination/time, Resend for approved recipients/content, WP-CLI for a selected site, and Humanizer PRO for explicitly selected text. Availability, endpoint control/Directory approval, privacy, account authority and runtime behavior must each be verified; these are not bundled or automatically enabled connectors. WordPress may be self-hosted. Humanizer PRO can forward selected text to Rephrasy, consume words and retain provider history. See [provider data disclosures](PRIVACY.md).

**Creative boundary:** AI video, audio, voice, avatars and general image generation are unsupported. The Agent Media launch procedure has been replaced with a creator/editor handoff. Deliver scripts, storyboards and shot lists; permitted design-only visual aids may use an available approved design workflow. Existing user-approved assets can be reviewed or prepared for separately authorized publication.

## Review, continuity and reporting

Use the [task router](skills/cmo/references/task-routing.md), [campaign stages](skills/cmo/references/agentic-workflow.md) and [operation outcomes](skills/cmo/references/operation-contract.md). Keep drafts, uploaded content and verified publication separate. Reconcile unknown paid starts or writes before repeating them. A schema describes the contract; it is not runtime enforcement.

A task can produce requested briefs, task boards, reports, issue corrections and handoffs. Continuation uses state pasted inline, not queries of prior project files. No uploaded/user-file extraction, conversation mining, consumer profiling, automatic preference learning or cross-session behavior modification is provided. Recurring reviews require an actual supported host scheduler, explicit bounded scope and activation readback. A plan or saved file is not an active schedule.

## OpenAI version

A separate portable adapter shares the reviewed skills and restrictions, with OpenAI presentation metadata and six role guides. Native Claude agent wrappers are excluded. No OpenAI/Cursor installation or directory approval follows automatically from source compatibility.

See PRIVACY.md, SECURITY.md, SUPPORT.md, TERMS.md and THIRD-PARTY-NOTICES.md. [Directory review notes](DIRECTORY-REVIEW.md) record current checks and remaining gaps. Original instructions are MIT licensed. The 140 mapped workflow families are instruction variants, not 140 executable tools; breadth research is not proof of measured task improvement.
