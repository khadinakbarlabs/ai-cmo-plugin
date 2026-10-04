# Feedback without surveillance

This package has no telemetry collector, feedback endpoint or global learning service. Feedback stays in the selected business workspace unless the user explicitly asks to send it to a specified destination through an authorized tool. Do not silently email the publisher or upload conversation history.

## Ask after value

Offer one short optional check after a usable deliverable: "Useful as-is, needs changes, or off-target?" Let the user reply naturally. Do not repeat it within the same session, interrupt urgent work, require a rating, or ask again after a refusal unless the user reopens feedback. Corrections during normal work count as feedback without another survey.

Use [feedback schema](feedback-schema.json) and [example](feedback-example.json) for a concise local record. Include business/session ID, deliverable reference, timestamp, category, verdict, actionable summary, severity, status and resolution. Prefer paraphrased minimum necessary context; no raw transcript, PII, customer contact lists or secrets. Categories: accuracy, strategy-fit, brand-voice, usability, integration, report, missing-workflow, outcome. Severity: low, medium, high. Verdict: useful, needs-changes, off-target, declined.

## Learn and close the loop

- Explicit style/process preference: propose or apply the precise change in context, show it to the user and allow correction.
- Factual error: verify the original evidence, fix all affected assets/recommendations, and record the correction and source.
- Strategy feedback: revise the hypothesis; measure outcomes before calling it a better strategy.
- Integration failure: retain redacted operation evidence and reconcile ambiguous effects before retrying.
- Missing capability: produce a concrete workaround/import path and a scoped improvement proposal.

Triage open items by severity, recurrence and affected deliverables. Link resolution to a real corrected output; a promise is not resolved. Review high-impact feedback before proposing the next campaign. Keep unresolved and declined records honest. Do not silently change files outside scope or label a customer observation as representative market research.

## Local product usefulness report

When requested, summarize first useful task completion, accepted vs revised outputs, unresolved feedback, repeat useful sessions and known time/cost per task from explicit journal/feedback records. State the sample and missing data. Count unique IDs and compatible periods; do not equate absence of feedback with satisfaction or session growth with marketing success. Cross-user aggregates require a separately designed, consented collection product; this plugin cannot infer them.
