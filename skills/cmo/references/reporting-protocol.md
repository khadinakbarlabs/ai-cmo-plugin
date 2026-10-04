# Reports that lead to a decision

Use Marketing Analytics for verified calculations and Performance Review for the recommendation. Read [report schema](report-schema.json), [example](report-example.json), [Markdown report](report-template.md) and [HTML template](report-template.html). Choose a compact snapshot, weekly review, monthly strategy or campaign retrospective based on the task. Match visuals to the actual business funnel, never force a consumer checkout onto procurement/donations/services.

## Minimum report contract

Business/campaign and report IDs; reporting period/timezone; source freshness/scope; actual goal; status; headline result; up to five relevant KPIs; comparable baseline or unavailable; interpretation/confidence; completed assets/tasks; budget/spend/cost where known; unresolved data/review/action blockers; next recommended action and next review. Keep draft/accepted/scheduled/published states separate. Include first useful task and feedback summaries only from explicit records and only when relevant.

Every metric records value or null, unit, observed/estimated/unknown state, definition, source, current period and comparison period if used. Missing is not zero. Each metric declares calculation as direct (exported value), ratio (numerator / denominator) or percentage (100 × numerator / denominator). Fractional rates use unit fraction; scaled percentages use unit percent. Display conversion must match these units. Direct metrics set the required numerator/denominator fields to null. Rates use compatible numerator/denominator, weighted aggregate totals and a nonzero denominator. ROI needs the appropriate margin/cost data; revenue ROAS is not profit. Currency/timezone/attribution mismatches cannot be silently combined. Estimated values are visually labeled and cannot appear as verified headline KPIs. Context facts and customer opinions are not analytics.

## Visual hierarchy

Lead with one conclusion and one recommended decision. Then show KPI cards, a real time series when enough points exist, model-appropriate funnel or stage table, channel comparison with units and denominator scope, completed work and next actions. For small data use a table rather than a decorative chart. Use accessible contrast, labels plus color, tabular numerals, readable text and print-friendly layout. Tables/CSV are the accessible fallback. Use Mermaid for a small process/funnel diagram when it improves understanding; do not invent counts to fill a graphic. Scientific/publication charts require a real plotting tool and an exportable artifact.

## Generate safe editable outputs

Save dated Markdown plus CSV when useful; optionally instantiate the standalone HTML template in the selected report directory. It has no JavaScript, trackers, external fonts/assets or network dependencies. HTML-escape every inserted business/source/feedback text, allow only verified http/https links, and use finite clamped numbers for chart widths. Never paste raw scraped HTML, scripts, style fragments or arbitrary URLs. Replace placeholders before delivery; don't claim a template is a populated report. Review mobile/print readability and check visible figures against source/calculations. If file tools are absent, return a readable inline report and clearly state it is unsaved.

## Cadence and decision quality

A weekly report should end with what changed, what matters, what to do, owner and review date. A monthly report should revisit strategy assumptions, experiment outcomes, capacity and feedback. A quiet period can yield "no material change" with known source scope. Do not promise better performance because a report exists. Share/email externally only within specific user authority and destination; a generated local report does not authorize delivery to a third party.
