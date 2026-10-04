# Recurring marketing reviews using host scheduling

A plugin file cannot execute after a session ends. Use an actually available host scheduling facility or a user-owned external scheduler; do not install a daemon, add hooks, create CI jobs or execute background tasks merely because recurrence is suggested. The six specialist wrappers do not expose scheduler tools; the coordinator discovers and registers through actual host capabilities.

## Proposed cadences

Adapt to data freshness, business cycle and capacity. Examples are drafts, never automatic defaults to enable: weekly priorities plus performance review; monthly strategy/experiment review; a launch-specific check after agreed milestones. Daily alerts are useful only when sufficient changing data and a material failure/decision threshold exist. Do not schedule frequent messages just to increase engagement.

## Register a concrete scope

1. Read current business, outcome, workspace, account/data availability and existing schedule records. Inspect supported scheduler capabilities and existing matching jobs before creating a duplicate.
2. Establish cadence, timezone, next occurrence, data sources, concrete report/output destination, allowed effects, run/cost budget, expiration/review date and notification behavior. Preserve standing authorization; ask for missing essentials together. Read-only performance checks do not authorize campaign writes or paid collection. Unknown run costs need an explicit limit before paid actions.
3. Prepare [schedule.json](schedule-example.json) using [the schema](schedule-schema.json), and [a review brief](scheduled-review-template.md). Bind runtime files to the actual selected workspace; no placeholders or fictional paths may be registered. A proposed recipe remains draft.
4. Register only when the user requests recurrence and the exact scope is understood. Use the platform's real tool/API rather than raw guessed syntax. Read back job ID, timezone, next_run_at, registered state and expiry; keep a redacted receipt. Failed/ambiguous registration is unknown pending reconciliation, never scheduled.
5. Each run loads the latest scoped context/board, reads only authorized data, checks existing same-window runs, creates a dated report and updates the session handoff. Include whether CLI credentials, source freshness and approved costs were available at execution. Deduplicate by business/schedule/window; reconcile a running/unknown prior attempt before starting another operation. Only a verified scheduler/executor can provide an actual overlap lock; a local record alone is not such a lock.
6. If required data is unavailable, return a gap report and manual import path without made-up results. Notify only on agreed review delivery, a meaningful change, material failure or needed decision. Unchanged monitoring stays quiet. Missed periods aggregate into one bounded review; don't replay every missed fire or spend extra without scope.
7. Keep edit/pause/cancel paths through the same host scheduler; verify applied changes. Removing plugin files does not cancel external schedules. Save a continuation handoff if a session ends, but do not claim it will wake itself.

## Provider availability, checked October 5, 2026

Claude Code session scheduling runs while its session is available; recurring tasks expire after seven days and missed intervals are not replayed individually. Durable automation uses a separately configured supported host service. See [official Claude scheduling documentation](https://code.claude.com/docs/en/scheduled-tasks). Verify current tool availability and semantics in the actual host. OpenAI packaging does not supply scheduling; use discovered host automation tools when available, otherwise return the draft plus manual review dates. Exact timing and delivery depend on that scheduler, not this plugin.
