---
name: cli-integrations
description: Connect an existing external CLI to a marketing workflow without adding a server to the plugin. Use for tool setup or checking supported integrations.
---

# CLI Integrations

Apply the [shared operating contract](../cmo/references/operating-contract.md) for evidence, local context and action scope.

## Workflow

1. Identify the requested service and required read/write/media/analytics capability.
2. Check executable/version and authoritative installed help; never invent a command or assume an API implies a CLI.
3. Use supported interactive login or environment setup without printing secrets; record non-secret capability status.
4. Prepare request files and test read-only discovery before scoped writes.
5. Honor user authorization and limits; reconcile uncertain writes before retries and read back external state.
6. If no suitable CLI or host access exists, supply an import/export/draft workflow; do not silently add MCP or a hosted backend.

## Deliverable

Tool capability record, verified request plan and useful fallback.

Use the [working reference](references/workflow.md) for covered variants, output fields and quality checks.

For account or production tools, use [CLI Integrations](SKILL.md) and its [tool capability guide](references/tool-capabilities.md). Do not assume an external CLI is installed or supports the intended action.
