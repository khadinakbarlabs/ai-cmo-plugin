# Postiz CLI execution

Source: https://github.com/gitroomhq/postiz-agent and its skills/postiz/SKILL.md. Contract researched October 5, 2026; verify installed CLI help before use. This package does not install or authenticate Postiz.

Setup when needed: install the official external `postiz` CLI following its current documentation, then use supported login. Prefer a login flow that does not place secrets in commands. Never print POSTIZ_API_KEY or credential files.

Read-only discovery sequence:

```sh
postiz --help
postiz auth:status
postiz integrations:list
postiz integrations:settings <integration-id>
```

Resolve exact account, provider settings, local timezone and desired execution time. Convert to an explicit timestamp with offset/UTC. Keep content in a JSON request file, following the installed `posts:create --help` contract. Authorize media upload as well as publishing; upload through `postiz upload` and use returned provider paths as required by the installed contract. Validate actual settings, file accessibility and destination limits.

Before creation, inspect returned provider rules, field descriptions and any dynamic choices/IDs (boards, playlists, communities or equivalent). Settings outside the integration schema can be discarded; validate against the actual account response. For TikTok publication, use `content_posting_method: "DIRECT_POST"`. `"UPLOAD"` sends media to the TikTok inbox for manual completion and can return success without publishing. Use that inbox route only when explicitly requested, and report manual completion as pending.

The documented create route supports `postiz posts:create --json <request-file>`. Run only for the authorized account/content/time. Retain returned IDs; inspect current post-list/info help and read back state. Where supported, `analytics:platform` and `analytics:post` supply analytics. Treat missing analytics explicitly. Do not assume every integration supports every media type or analytic metric.

There is no package guarantee of idempotency. On timeout or ambiguous creation, inspect existing posts/request IDs before retrying. Scheduled is not published. Error logs may contain content/account details; summarize instead of copying raw logs.
