# Host editions and exposure

Canonical authoring is the Claude package; the OpenAI portable edition shares the skill bodies/resources, with root plugin.json and contained presentation metadata. Public ID: khadin-ai-cmo. External CLIs are independently installed tools. None of these installations grant paid-run, sending, publishing or scheduler authority.

| Host | Supported installation / invocation | Verify |
| --- | --- | --- |
| Claude Code | Add the GitHub marketplace and install khadin-ai-cmo@ai-cmo-marketplace as described in README; /khadin-ai-cmo:cmo or relevant specialist | Run `claude plugin list --json`, check enabled version/path, then open a fresh session and observe a representative skill load |
| Claude Code isolated validation | `claude --plugin-dir /absolute/claude/package` or a supported ZIP | This process loads the selected edition; it does not install/refresh the default account plugin |
| Codex local | A supported repo/personal marketplace points to the portable package; enable the exact plugin-name@marketplace-name | Inspect `codex plugin list --json`, actual installed skill/resource paths, and a fresh supported session. Existing sessions may retain the old discovery list |
| Codex copy-only skills | Copy the complete skills tree into an isolated project's .agents/skills for testing | Retain sibling references and per-skill assets. This verifies a copied skill edition, not native plugin installation |
| Cursor local | Put the complete portable package under ~/.cursor/plugins/local/khadin-ai-cmo with root plugin.json | Reload Window/restart, confirm Customize components and a task. Admin settings can disable local imports; a same-name marketplace install takes precedence |
| Claude/ChatGPT remote surfaces | Supported directory installation/upload | Confirm actual host exposure and tools separately. Web/cloud installs do not expose CLIs on a personal computer |

Keep installed version/path separate from source version. Search only target plugin IDs across relevant marketplace/cache/copied-skill locations before refresh; do not overwrite unrelated marketing plugins or hand-edit managed caches. Synchronize existing installs through supported marketplace updates or replace an owned copied/local edition after checking for user edits and retaining rollback. Preserve public IDs and invocation policies. Do not replace an existing provider review merely to test a local change.

Codex local marketplace paths are relative to the marketplace root, not the .agents/plugins folder. Marketplace discovery is separate from enabled installation. Claude native agent files do not register OpenAI/Cursor agents: those editions use six role guides and sequential fallback unless authorized native delegation actually exists. Required references must remain inside the selected package.

Sources checked 2026-10-05: [Claude skills](https://code.claude.com/docs/en/skills), [OpenAI plugin authoring](https://developers.openai.com/plugins/build/plugins), [Cursor local plugins](https://cursor.com/docs/plugins). Verify the installed CLI help and current documentation at use time; no universal count limit or cross-host evaluation runner is assumed.

## Same-name skills and crowded sessions

A correct local source or marketplace entry does not prove this session selected it. Personal/copied marketing skills can share IDs such as sales-enablement. Record the actual loaded SKILL.md path and source version during a harmless smoke task. If the host reports dropped descriptions or a skills-context overflow, record discovery as impaired; do not infer that your description failed from that run. Test an isolated edition with only relevant skills enabled through the host's supported settings, then compare against the normal session. Per-process overrides must not permanently disable unrelated user skills. A path-pinned or explicit invocation test is distinct from natural selection.

Codex supports path-specific `[[skills.config]]` entries with `enabled = false`; verify current [skill controls](https://developers.openai.com/codex/skills) before using them. Use a fresh session after supported installation/refresh. Do not count a response produced by a different same-name skill as this plugin's behavior.
