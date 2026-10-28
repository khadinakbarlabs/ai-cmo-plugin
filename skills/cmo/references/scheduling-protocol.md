# Recurring marketing reviews through the host

Apply [directory boundaries](directory-boundaries.md). A plugin file cannot wake itself or run after a session ends. Use only an actual supported host scheduler requested by the user; no daemon, hook, installer or implicit recurring activity is included.

## Prepare and register

1. Use the business goal, bounded inline job brief and permitted account/data scope supplied for this request. Inspect existing matching jobs through the scheduler's real tool/API, not saved schedule, project or session files.
2. Establish cadence, timezone, reporting window, exact allowed data sources/effects, destination, run/cost bounds, expiry and notification rules. A reporting job does not authorize collection spending, outreach or campaign changes. Missing enforceable scope blocks activation.
3. Prepare a complete inline job brief using the bundled [schedule schema](schedule-schema.json) and [review template](scheduled-review-template.md). An optional saved schedule artifact is output only when requested; it is not an active executor or an input file to reload later.
4. Register using the supported host tool and read back actual job ID, timing, next run and activation. Ambiguous registration remains unknown; reconcile through scheduler readback before creating a duplicate.

## Each requested run

Use only the inline job inputs actually registered and permitted live-provider/scheduler readback. Do not load user-generated/uploaded files, prior context/boards, conversation summaries or session journals. If current task state or metric rows are unavailable through an admitted provider, request the bounded missing information inline or return a gap report; do not silently substitute file access.

Check provider freshness, identity, authority and cost controls at execution. Reconcile same-window running/unknown operations before any new effect; a local record is not an overlap lock. Deliver the explicitly scheduled report and one next decision. Create a handoff only if the job scope requests it; never automatically append session history or learn a personal profile.

Notify only for the agreed report, meaningful change/failure or required decision. Keep unchanged monitoring quiet and avoid replaying missed periods or extra spending without scope. Use the same host's supported edit/pause/cancel tool and verify the result. Removing plugin files does not cancel a registered job.

If no supported scheduler exists, return a complete draft brief and a manual review date. Verify current capabilities in the actual host; compatibility does not establish activation. References: [Claude scheduling](https://code.claude.com/docs/en/scheduled-tasks). No timing, lifetime or delivery guarantee is inferred from this document.
