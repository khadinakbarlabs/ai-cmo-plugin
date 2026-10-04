---
name: apify-research
description: Run bounded research with Khadin Akbar’s verified Apify Actors through the external Apify CLI, or collect an existing run. Use for Actor-backed marketing data.
---

# Apify Research

Apply the [shared operating contract](../cmo/references/operating-contract.md) for evidence, local context and action scope.

## Workflow

1. Read the Actor catalog and CLI contract; match the exact Actor ID to the requested job. Do not substitute a similarly named Actor.
2. Inspect the installed CLI help, account identity and live input schema/default build; compare with the dated catalog.
3. Prepare and validate a small input JSON from actual required fields; set supported result limits and a user-authorized cost/timeout envelope.
4. Start a new paid run only within explicit or standing authorization; use the documented CLI API route when charge controls are needed.
5. Retain run/build/input IDs and state, then paginate the dataset and relevant summary records. Distinguish run success from usable research rows.
6. Report partial/error rows and charged meters separately; redact credentials and retain provenance with outputs.

## Deliverable

Verified input, run record, paginated dataset, summary and source-linked findings.

Use the [working reference](references/workflow.md) for covered variants, output fields and quality checks.

Read [Actor catalog](references/actor-catalog.md) and [Apify CLI execution](references/apify-cli.md).
