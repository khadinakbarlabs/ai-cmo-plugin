---
name: social-publishing
description: Prepare, schedule and verify social posts through the externally installed Postiz CLI. Use when the user asks to publish or schedule specific content.
---

# Social Publishing with Postiz

Apply the [shared operating contract](../cmo/references/operating-contract.md) for evidence, local context and action scope.

## Workflow

1. Read the Postiz CLI reference and inspect the installed help; check authentication without exposing credentials.
2. Discover integrations and provider settings; select the exact destination account and user timezone.
3. Prepare platform-specific content and request files; validate lengths, media paths and required settings.
4. Honor authorization for the concrete post/account/time. Upload approved media through the documented CLI flow before referencing its returned path.
5. Create the post once and retain returned IDs; read back scheduling/publication state.
6. On an uncertain response reconcile provider state before retrying. Do not report scheduled content as published.

## Deliverable

Request file, verified destination/time, external IDs and observed state.

Use the [working reference](references/workflow.md) for covered variants, output fields and quality checks.

Read [Postiz execution](references/postiz-cli.md) before account operations.
