# Structured operation outcomes

Use this for multi-step imports, collection, external writes or uncertain recovery. A small local edit needs only its result and next action. Use the existing business/campaign task IDs and `.ai-cmo/operations/<operation-id>.json` if persistence is allowed, otherwise return an explicitly unsaved receipt. Do not introduce a second workspace or overwrite another session's state. The [schema](operation-schema.json) and [fictional partial import](operation-example.json) define an agent-readable record; they are guidance, not a shipped runtime or mandatory user questionnaire.

Record plugin version, operation/business/task identity, mode (local/import/live), actual effect, current state, bounded limits, counts, real artifact paths, evidence level, safe error and continuation. Inputs are selected source references or hashes, not raw customer rows. The provider block includes service, generic operation ID (or run ID), non-secret account/target references, requested build for paid research, attempted_at and a sha256 request fingerprint; unknown starts retain this identity even when IDs are null. Live running needs an actual provider ID and execution observation. Completion of an external effect requires provider-readback and an actual operation/run ID; a local draft check cannot certify publishing or sending. Provider IDs belong only to task-scoped records, never generic shared context. No secrets or unfiltered account metadata. Normal output is the result/receipt; diagnostics belong separately and must not pollute machine-readable JSON or expose stack traces.

| State | Meaning / next step |
| --- | --- |
| planned | Request prepared; no execution claimed |
| blocked | Required input/tool/access/authority/state is missing; finish independent local work |
| running | Actual ongoing operation with a provider ID or local execution observation |
| partial | Usable output exists, with explicit missing coverage and a checkpoint |
| completed | Requested artifacts exist and acceptance was checked at the stated level |
| failed | Observed terminal failure, with a safe error and any salvageable artifacts |
| unknown | A possible external effect lacks reliable readback; reconcile before any repeat |

Verification is none, local-check or provider-readback. It describes an observed check, not provider approval, independent editorial truth or user acceptance. Keep provider run status separate in `provider.status`: SUCCEEDED can still yield a partial/failed business result. Do not mark empty output completed when upstream diagnostics indicate unavailable coverage.

Safe errors: RUNTIME_MISSING, PROJECT_MISSING, INPUT_INVALID, ACCESS_DENIED, AUTH_REQUIRED, AUTHORITY_REQUIRED, VERSION_UNSUPPORTED, STATE_CONFLICT, COVERAGE_PARTIAL, PROVIDER_FAILED, OUTCOME_UNKNOWN. Each needs a short redacted diagnostic and a concrete next action. A zero exit code is insufficient evidence; actual files, counts and readback matter.

Paid research requires an effect-specific authority reference plus a positive authorized cost limit independently of raw-row/page/time limits. Verify the provider's current cap semantics, minimum charges and supported request. Unsupported controls block the launch; no uncapped fallback. A saved receipt is historical scope, not renewed authorization.

An unknown write/start must retain any known IDs, fingerprint and attempt window. Use supported readback for the same account/entity and compare the request; do not rely on “latest run” alone. If no unique match can be established, remain unknown and ask for the necessary reconciliation, never start a replacement. If identity fields from a previous external attempt are unavailable, preserve an explicitly incomplete unknown-outcome handoff and request only those missing fields. Do not fabricate IDs, hashes or timestamps, discard the unknown effect, or claim schema-valid persistence; preserve any earlier receipt unchanged. No replay is authorized by inability to reconstruct identity. Read-only retry is bounded and stops on access restrictions. A local receipt ID does not establish provider idempotency.

On resume, reconcile the receipt with current files/provider state and the latest user request. Preserve completed artifacts, review decisions and raw-page checkpoints. If scope changed, create an explicit successor operation instead of silently mutating the prior effect. Never count a schedule proposal as activated; use the existing schedule schema and actual host registration/readback.
