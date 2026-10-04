# Agent Media through an external CLI

Primary sources: https://github.com/gitroomhq/agent-media and published `agent-media-cli` 1.19.0 command source, inspected October 5, 2026. Use the standalone CLI; do not install its MCP plugin as an AI CMO dependency.

```sh
agent-media --help
agent-media login
agent-media skills list --json
agent-media skills run --help
agent-media skills status --help
```

Confirm the profile, current skill input schema, available credits, expected cost and model/rights constraints. `make_ugc` accepts the approved script and identity inputs; validate current fields instead of guessing them. A confirmed paid request can use a request file and a saved idempotency key:

```sh
agent-media skills run make_ugc --input-file ./approved-video.json --idempotency-key <saved-request-key> --json
agent-media skills status <returned-run-id> --composed --json
```

Use composed status only when the response supplies `skill_run_id`; ordinary `run_id` uses its matching status route. This is submission plus bounded status checks. Waiting timeout does not cancel remote execution, and a successful process exit does not prove render success. Inspect terminal status and the actual output video for claims, likeness permission, voice, captions, format and duration. Save the run record before polling; reconcile uncertain writes with the same request key.

Generation consumes provider credits and sends scripts/assets to that provider. Keep tokens out of arguments and reports. Export the finished asset for the separately authorized Postiz publishing flow. When unavailable, deliver the script, storyboard and production specification.
