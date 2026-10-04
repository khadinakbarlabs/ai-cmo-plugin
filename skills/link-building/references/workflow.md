# Link Building working reference

## Output contract

Qualified prospect CSV, tactic/asset match, outreach drafts and tracking sheet.

Record the business/campaign ID, source dates and input scope. Include the useful artifact plus evidence, unavailable fields, decision and next owner. Treat an estimated outcome as a hypothesis until measured.

## Quality checks

- Does the output answer the requested customer/business job?
- Can another person verify the important facts from the retained evidence?
- Are prerequisites and actual tool capabilities distinguished from completed actions?
- Are unknown metrics marked and recommendations tied to a test or evidence?
- Is the next handoff concrete and editable?

## Recovery

For missing tools or accounts, produce the useful draft/import-based result and identify the specific missing capability. For empty data, retain collection scope and explain the absence rather than inventing a finding. For partial results, mark the missing portion and avoid extrapolating to the whole market.

## Prospect CSV

Use prospect_url, source_url, checked_at, tactic, topical_fit, existing_link_status, destination_asset, value_offered, contact_source, contact_confidence, outreach_draft_path, owner, stage, next_followup. Avoid ranking by domain-authority score alone. Verify that a broken link is currently broken and that the replacement satisfies the same user need. An unlinked mention needs contextual fit; a scraped email address does not confer permission to send.

## Covered variants

- Backlink profile and gap analysis
- Link prospect qualification
- Broken link opportunities
- Unlinked brand mentions
- Resource page outreach
- Outreach drafting and follow-up tracking

## Exact owned Actor routes

Use [Apify Research](../../apify-research/SKILL.md) for schemas, cost scope and execution. Each route is optional and runtime-untested; do not substitute an unverified Actor.

- `khadinakbar/website-backlink-checker` (`rCohK9eJbjiovPN6s`): required keys `targets`. [Live-inspected schema](../../apify-research/references/public-schemas/website-backlink-checker.json) and [bounded example](../../apify-research/references/public-inputs/website-backlink-checker.json).
- `khadinakbar/backlink-opportunity-finder` (`n1uR8aWhzOBYhxLJl`): required keys `keywords`. [Live-inspected schema](../../apify-research/references/public-schemas/backlink-opportunity-finder.json) and [bounded example](../../apify-research/references/public-inputs/backlink-opportunity-finder.json).
- `khadinakbar/broken-link-checker` (`a2yeVoO8SdJgVEgbK`): required keys `mode`. [Live-inspected schema](../../apify-research/references/public-schemas/broken-link-checker.json) and [bounded example](../../apify-research/references/public-inputs/broken-link-checker.json).
- `khadinakbar/bulk-website-contact-extractor` (`TwNeQtj5TfaKDkcCK`): required keys `startUrls`. [Live-inspected schema](../../apify-research/references/public-schemas/bulk-website-contact-extractor.json) and [bounded example](../../apify-research/references/public-inputs/bulk-website-contact-extractor.json).
- `khadinakbar/contact-details-scraper` (`xUTDfDQougiuhikSc`): required keys none declared. [Live-inspected schema](../../apify-research/references/public-schemas/contact-details-scraper.json) and [bounded example](../../apify-research/references/public-inputs/contact-details-scraper.json).
