# Resources: Make Economic Opportunity Easier to Reach

Challenge brief: [../challenges/03-economic-prosperity.md](../challenges/03-economic-prosperity.md)

## Birmingham sources

- Prosper Birmingham dashboard: https://prosperbham.com/dashboard/
- Birmingham Innovation and Economic Opportunity: https://ieo.birminghamal.gov/
- Birmingham Office of Business Diversity and Opportunity: https://ieo.birminghamal.gov/obdo/
- RPCGB economic development: https://www.rpcgb.org/economicdevelopment
- Jefferson State Fast Track: https://www.jeffersonstate.edu/academics/fast-track/

## National sources

- O*NET database: https://www.onetcenter.org/database.html
- BLS public data API: https://www.bls.gov/developers/
- Census data APIs: https://www.census.gov/data/developers/data-sets.html

## Synthetic dataset

[data/economic-opportunity-profiles.csv](data/economic-opportunity-profiles.csv)

**This dataset is entirely synthetic. It contains six clearly fictional people or business profiles. It does not represent any real resident, worker, or founder, and must not be presented as real, live, or authoritative.**

Columns: `profile_id`, `pathway`, `current_state`, `goal`, `constraint`, `opportunity`, `requirement`, `next_seven_day_action`, `handoff_owner_type`, `requires_human_confirmation`, `is_synthetic`.

## 30-minute quick start

1. Open [data/economic-opportunity-profiles.csv](data/economic-opportunity-profiles.csv) and pick one fictional profile.
2. Choose a primary user (worker, young person, navigator, or founder) matching that profile's `pathway` and the moment "what can I do next?"
3. Using the profile's `constraint`, `opportunity`, and `requirement`, identify one reachable step drawing on the profile's own `next_seven_day_action` as a starting point.
4. Cross-check the opportunity against one Birmingham program page (e.g., Jefferson State Fast Track, Birmingham IEO/OBDO) and one national reference (O*NET for occupation/skill context, or BLS for labor market evidence).
5. Produce a first artifact: a pathway card, a small opportunity matcher, or a human-review checklist showing the `handoff_owner_type`.

## Download or API notes

- The Prosper Birmingham dashboard, Birmingham IEO/OBDO pages, RPCGB economic development page, and Jefferson State Fast Track page are standard web pages; read and cite them directly. No bulk download has been verified for these.
- O*NET provides a downloadable database described at https://www.onetcenter.org/database.html; use the documented download files rather than scraping the site.
- BLS offers a public API described at https://www.bls.gov/developers/; follow its documented series IDs and request format rather than guessing endpoints.
- Census data APIs are described at https://www.census.gov/data/developers/data-sets.html; use the documented dataset and variable names.

## Freshness and limitations

- Links were checked on August 27, 2026.
- O*NET occupation and skill data reflects a periodically updated national reference model, not real-time local job openings. BLS data reflects published historical/statistical series, not a live job board. The most important limitation for this track: none of these sources confirm a specific opening, admission, or eligibility for a specific person; only the linked Birmingham program's own current information can do that, and it should be confirmed directly with the program.

## Licensing and terms

- Follow the terms, attribution, and rate-limit rules published on each Birmingham and national source site. Linking to a source here does not grant any right to redistribute its content or data.
- O*NET data is public but subject to its own attribution requirements; check the O*NET site for current citation guidance. BLS and Census API data are public federal data; still follow published usage terms and any rate limits.
- The synthetic profile CSV may be copied and modified for your event project, but any copy must keep the `is_synthetic` label and must not be presented as a real person or business.

## Prohibited uses

- Do not predict employability, success, or performance for any profile.
- Do not guarantee eligibility, funding, admission, wages, or employment for any pathway.
- Do not present O*NET or BLS statistics as a personalized promise or determination for a specific person.
- Do not present synthetic profiles as real residents, workers, or founders.
