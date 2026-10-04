# Resend email CLI

Primary contract: https://github.com/resend/resend-cli and its skills/resend-cli references; inspected October 5, 2026. Install the maintained external `resend-cli` package only when needed. Use `resend --help`, `resend login` and `resend doctor`; confirm the chosen profile and verified sender. Keep credentials in its supported store/environment, never command arguments or drafts.

Inspect `resend emails send --help` and `resend emails get --help`. A file-based send route is:

```sh
resend emails send --from 'Approved sender <sender@example.com>' --to 'approved@example.com' --subject 'Approved subject' --html-file ./approved-email.html --dry-run
```

The placeholders are not real destinations. Dry-run validates a payload without sending; inspect its recipient/content output privately. Remove `--dry-run` only for the exact authorized send, subject to installed support. Preserve the returned email ID; use `resend emails get <id>` for status. API acceptance is distinct from delivery.

For newsletters, inspect `resend broadcasts create --help` and `resend broadcasts send --help`; use the verified segment and suppression rules. Dry-run support differs by command. Never convert a request for copy into a send, expose recipient lists in reports, or retry an uncertain send before reconciliation. Produce HTML/plain text when disconnected.
