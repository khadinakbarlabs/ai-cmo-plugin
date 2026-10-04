---
name: technical-seo
description: Audit crawlability, indexability, schema, links and site structure. Use for technical SEO, crawl findings, sitemaps or structured-data checks.
---

# Technical SEO

Apply the [shared operating contract](../cmo/references/operating-contract.md) for evidence, local context and action scope.

## Workflow

1. Define crawl scope and site ownership; use a bounded site crawl or supplied export.
2. Check HTTP status, robots directives, canonical targets, duplicate pages, sitemap consistency and internal navigation.
3. Inspect rendering and structured data against the page content. Do not infer a Search Console indexing status from a successful HTTP response.
4. Separate observed defects from suggestions; include affected URLs, reproducible evidence, severity and likely impact.
5. Prepare fix specifications with a verification method. Edit a website only within the user-authorized scope and verify the affected behavior.

## Deliverable

Technical issue register, evidence and fix/verification specifications.

Use the [working reference](references/workflow.md) for covered variants, output fields and quality checks.

For optional data collection, use [Apify Research](../apify-research/SKILL.md) and its [verified Actor catalog](../apify-research/references/actor-catalog.md). Prefer the exact relevant owned Actor; imports remain useful when a tool is unavailable.
