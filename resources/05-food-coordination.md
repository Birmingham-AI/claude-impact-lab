# Resources: Coordinate Birmingham's Food Support Network

Challenge brief: [../challenges/05-food-coordination.md](../challenges/05-food-coordination.md)

## Birmingham sources

- Feeding Alabama food finder: https://feedingal.org/find-food-near-you/
- Feeding Alabama programs: https://feedingal.org/programs/
- Grace Klein Community FeedBHM: https://gracekleincommunity.com/feedbhm/
- Jones Valley Teaching Farm sites: https://jvtf.org/our-sites/
- United Way 211: https://www.uwca.org/programs/211-call-center/

## National sources

- USDA Food Access Research Atlas download: https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data
- USDA Food Environment Atlas: https://www.ers.usda.gov/data-products/food-environment-atlas

## Synthetic dataset

[data/food-supply-demand.csv](data/food-supply-demand.csv)

**This dataset is entirely synthetic. It contains eight clearly fictional supply and demand records at synthetic organizations. Nothing in this dataset is live. It does not represent any real inventory, need, or client, and must not be presented as real, live, or authoritative.**

Columns: `record_id`, `record_type`, `synthetic_organization`, `food_category`, `quantity`, `available_or_needed_by`, `storage_requirement`, `transport_available`, `service_area`, `status`, `confirmation_owner_type`, `is_synthetic`.

## 30-minute quick start

1. Open [data/food-supply-demand.csv](data/food-supply-demand.csv) and pick one fictional supply record (`record_type` = supply) and one fictional demand record (`record_type` = demand).
2. Choose a primary user (food coordinator, resident, or frontline staff) and the moment "where should this go?" for that pair.
3. Identify a possible match by comparing `food_category`, `service_area`, and `available_or_needed_by` for the two records.
4. List the confirmation steps needed before any real transfer: timing, `storage_requirement`, `transport_available`, and the `confirmation_owner_type`.
5. Produce a first artifact: a match board, a transfer checklist, or a referral confirmation workflow.

## Download or API notes

- Feeding Alabama, Grace Klein Community FeedBHM, Jones Valley Teaching Farm, and United Way 211 pages are standard web pages; read and cite them directly. No bulk download or API has been verified for these.
- The USDA Food Access Research Atlas offers a documented download at https://www.ers.usda.gov/data-products/food-access-research-atlas/download-the-data; use the linked data files rather than guessing a file structure.
- The USDA Food Environment Atlas offers its own documented download page at https://www.ers.usda.gov/data-products/food-environment-atlas; use the linked data files there.

## Freshness and limitations

- Links were checked on August 27, 2026.
- The USDA Food Access Research Atlas and Food Environment Atlas provide periodically updated geographic and county/tract-level context measures (such as food access indicators), not live pantry inventory or individual-level need. The most important limitation for this track: neither USDA source reflects current stock, hours, or capacity at any specific pantry or organization; only the synthetic dataset or a direct check with the organization can speak to that, and even the synthetic dataset must never be shown as live.

## Licensing and terms

- Follow the terms, attribution, and rate-limit rules published on each Birmingham and national source site. Linking to a source here does not grant any right to redistribute its content or data.
- USDA Food Access Research Atlas and Food Environment Atlas data are public federal data; still follow their published usage and citation terms.
- The synthetic supply/demand CSV may be copied and modified for your event project, but any copy must keep the `is_synthetic` label and must not be presented as real inventory, real need, or a real client.

## Prohibited uses

- Do not ration or allocate food by an opaque or automated algorithm with no human confirmation step.
- Do not use private client lists or any real individual's need or identity.
- Do not present synthetic supply, demand, or availability records as live or real.
- Do not treat USDA Atlas geographic measures as a substitute for confirming actual current inventory with an organization.
