# Keyword Research working reference

## Output contract

Keyword CSV, intent clusters, page map and prioritized briefs.

Record the business/campaign ID, source dates and input scope. Include the useful artifact plus evidence, unavailable fields, decision and next owner. Treat an estimated outcome as a hypothesis until measured.

## Quality checks

- Does the output answer the requested customer/business job?
- Can another person verify the important facts from the retained evidence?
- Are prerequisites and actual tool capabilities distinguished from completed actions?
- Are unknown metrics marked and recommendations tied to a test or evidence?
- Is the next handoff concrete and editable?

## Recovery

For missing tools or accounts, produce the useful draft/import-based result and identify the specific missing capability. For empty data, retain collection scope and explain the absence rather than inventing a finding. For partial results, mark the missing portion and avoid extrapolating to the whole market.

## Keyword table contract

Columns: query, country, language, engine, observed_at, source, intent, cluster, business_relevance, volume, volume_units, CPC, currency, difficulty, metric_definition, target_page, existing_or_new, confidence, proposed_next_step. Empty metric cells mean unknown, not zero. Preserve period/aggregation definitions when joining providers. Use branded/nonbranded and transactional/informational distinctions to explain priority. Two keywords sharing words may need different pages when SERP intent differs.

## Covered variants

- Keyword research
- Search intent classification
- Keyword clustering and page mapping

## Exact owned Actor routes

Use [Apify Research](../../apify-research/SKILL.md) for schemas, cost scope and execution. Each route is optional and runtime-untested; do not substitute an unverified Actor.

- `khadinakbar/dataforseo-keyword-research` (`8RW7Ow9S3hRAnX1ye`): required keys `seedKeywords`. [Live-inspected schema](../../apify-research/references/public-schemas/dataforseo-keyword-research.json) and [bounded example](../../apify-research/references/public-inputs/dataforseo-keyword-research.json).
- `khadinakbar/keyword-search-volume-api` (`B7Wq9VHcVFdfNqNBI`): required keys `keywords`. [Live-inspected schema](../../apify-research/references/public-schemas/keyword-search-volume-api.json) and [bounded example](../../apify-research/references/public-inputs/keyword-search-volume-api.json).
- `khadinakbar/scrape-google-serp` (`z0r97dqhtUQk2AXd8`): required keys none declared. [Live-inspected schema](../../apify-research/references/public-schemas/scrape-google-serp.json) and [bounded example](../../apify-research/references/public-inputs/scrape-google-serp.json).
- `khadinakbar/google-trends-scraper` (`yIPnv2aKGDmRmgoy1`): required keys none declared. [Live-inspected schema](../../apify-research/references/public-schemas/google-trends-scraper.json) and [bounded example](../../apify-research/references/public-inputs/google-trends-scraper.json).
- `khadinakbar/seo-domain-keyword-scraper` (`7XL6DUjjDCqltKeBg`): required keys none declared. [Live-inspected schema](../../apify-research/references/public-schemas/seo-domain-keyword-scraper.json) and [bounded example](../../apify-research/references/public-inputs/seo-domain-keyword-scraper.json).
- `khadinakbar/keyword-rank-tracker` (`ufcrXss0mJzYLRgWW`): required keys `targetDomain`, `keywords`. [Live-inspected schema](../../apify-research/references/public-schemas/keyword-rank-tracker.json) and [bounded example](../../apify-research/references/public-inputs/keyword-rank-tracker.json).
