---
name: marketing-operations
description: Plan marketing operations and AI-assisted research, production and QA workflows. Use for AI marketing, reusable prompts, evaluation, automation planning, tracking or tool health.
---

# Marketing Operations

Apply the [shared operating contract](../cmo/references/operating-contract.md) for evidence, local context and action scope.

## Workflow

1. Inventory accounts/tools and actual capabilities without storing credentials.
2. Define campaign IDs, asset names, UTM rules and conversion events consistently across channels.
3. Check tracking destinations, event semantics and duplicate counting with available evidence.
4. Maintain asset and decision registers and scoped operation records; keep business state outside plugin installation.
5. Provide a health report and handoff for missing permissions, stale exports or unverified integrations.

## Deliverable

Capability matrix, UTM/event plan, asset register and operations health report.

Use the [working reference](references/workflow.md) for covered variants, output fields and quality checks.

For account or production tools, use [CLI Integrations](../cli-integrations/SKILL.md) and its [tool capability guide](../cli-integrations/references/tool-capabilities.md). Do not assume an external CLI is installed or supports the intended action.

## Specialized workflow routes

Choose the relevant guide before performing that task; retain its evidence, authority and acceptance checks.

- [AI Marketing](references/ai-marketing.md): AI workflow brief, reusable prompts, reviewed pilot outputs, provider/data map and evaluation/rollout criteria.

## Recurring reviews and continuity

Use [scheduling protocol](../cmo/references/scheduling-protocol.md) for requested host-based recurring reviews with scoped data, effect/cost limits, timezone, receipts, deduplication, gap reports and pause/cancel. Draft is not registered. Preserve a [session journal](../cmo/references/session-journal-template.md) and actionable feedback queue. The plugin has no background executor or unattended authority.
