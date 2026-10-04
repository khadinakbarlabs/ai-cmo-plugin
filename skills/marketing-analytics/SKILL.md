---
name: marketing-analytics
description: Analyze marketing performance, attribution, cohorts and funnel metrics from first-party data or imports. Use for marketing reporting and tracking checks.
---

# Marketing Analytics

Apply the [shared operating contract](../cmo/references/operating-contract.md) for evidence, local context and action scope.

## Workflow

1. Record provider, account, date range, timezone, attribution window, currency and filters.
2. Validate imports for duplicate rows, inconsistent dimensions and missing values; aggregate compatibly.
3. Calculate CTR as clicks/impressions, CPC as spend/clicks, CPA as spend/attributed conversions and ROAS as attributed revenue/spend; return unknown for missing/zero denominators.
4. Distinguish attributed revenue from incremental revenue; do not merge incompatible attribution models or claim paid ROI without spend/outcome data. ROAS is a revenue multiple, not profit: never call a campaign profitable without contribution margin and relevant acquisition/fulfillment costs.
5. Diagnose changes with segment and baseline comparisons; include alternative explanations, sample sufficiency and confidence. A zero-click snapshot does not establish broken delivery or a platform learning-window rule; propose diagnostics before causal claims or reallocations.
6. Prepare measurement fixes and the next decision, with source files and a reproducible calculation trail.

## Deliverable

Metric table, calculation definitions, findings, unknowns and decision-ready report.

Use the [working reference](references/workflow.md) for covered variants, output fields and quality checks.

For account or production tools, use [CLI Integrations](../cli-integrations/SKILL.md) and its [tool capability guide](../cli-integrations/references/tool-capabilities.md). Do not assume an external CLI is installed or supports the intended action.

## Visual reporting

Follow [reporting protocol](../cmo/references/reporting-protocol.md) for weekly/monthly/campaign reports, verified KPI cards, editable tables and a standalone HTML presentation. Use real outcome definitions, source scope and compatible periods. Unknown data stays unknown; a populated report and an empty template are different deliverables. Include one decision, owner and review date.
