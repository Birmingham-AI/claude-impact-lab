# Resources: Improve the Handoff to Homelessness Services

Challenge brief: [../challenges/04-homelessness-handoff.md](../challenges/04-homelessness-handoff.md)

## Birmingham sources

- One Roof: https://www.oneroofonline.org/
- One Roof Coordinated Entry: https://www.oneroofonline.org/coordinated-entry
- City community resources: https://cobcd.com/communityresources/
- United Way 211: https://www.uwca.org/programs/211-call-center/
- Birmingham 2025-2029 Consolidated Plan (linked from the Action Plan page): https://cobcd.com/action-plan/

## National sources

- HUD PIT and HIC data: https://www.huduser.gov/portal/datasets/ahar.html
- HUD Community Planning and Development notices (see CPD-17-01 for coordinated-entry requirements): https://www.hud.gov/hudclips/notices/cpd

## Synthetic dataset

[data/homelessness-handoff-scenarios.csv](data/homelessness-handoff-scenarios.csv)

**This dataset is entirely synthetic. It contains six non-identifying, clearly fictional scenarios without detailed trauma narratives. It does not represent any real person, case, or live shelter/service capacity, and must not be presented as real, live, or authoritative. It does not replace Coordinated Entry.**

Columns: `scenario_id`, `person_context`, `immediate_need`, `public_resource_type`, `information_to_confirm`, `safe_next_step`, `handoff_owner_type`, `follow_up_window`, `capacity_is_not_live`, `is_synthetic`.

## 30-minute quick start

1. Open [data/homelessness-handoff-scenarios.csv](data/homelessness-handoff-scenarios.csv) and pick one fictional scenario.
2. Choose a primary user (the person in the scenario or a frontline responder) and the moment "what happens now?" for that scenario's `immediate_need`.
3. Build a safe handoff summary using the scenario's `public_resource_type`, `information_to_confirm`, and `safe_next_step`.
4. Add source and freshness notes, mark the `capacity_is_not_live` flag clearly, and identify the `handoff_owner_type` responsible for the `follow_up_window`.
5. Produce a first artifact: a handoff card, a resource-confirmation workflow, or a frontline summary that a human can review before acting.

## Download or API notes

- One Roof, One Roof Coordinated Entry, City community resources, United Way 211, and the Consolidated Plan PDF are standard web pages or a downloadable PDF; read and cite them directly. No bulk download or API has been verified for these.
- HUD PIT and HIC data are available as downloadable reports and datasets at https://www.huduser.gov/portal/datasets/ahar.html; use the documented download links rather than assuming an API exists.
- The HUD Coordinated Entry Core Elements document is a guidance PDF, not a data source; use it to understand the workflow, not to pull data.

## Freshness and limitations

- Links were checked on August 27, 2026.
- HUD PIT (Point-in-Time) and HIC (Housing Inventory Count) data are published historical, system-level counts collected on specific dates, not live shelter capacity or availability. The most important limitation for this track: no source here reflects real-time bed or shelter availability, and Coordinated Entry (One Roof) is the actual workflow boundary for placement decisions; this event's artifacts must not replace or bypass it.

## Licensing and terms

- Follow the terms, attribution, and rate-limit rules published on each Birmingham and national source site. Linking to a source here does not grant any right to redistribute its content or data.
- HUD PIT/HIC datasets and the Coordinated Entry Core Elements document are public federal resources; still follow their published usage and citation terms.
- The synthetic scenario CSV may be copied and modified for your event project, but any copy must keep the `is_synthetic` label and the `capacity_is_not_live` flag, and must not be presented as a real person, case, or live capacity.

## Prohibited uses

- Do not use real client data, HMIS records, or any personally identifying information about an actual unhoused person.
- Do not score, rank, or assign vulnerability or risk to any person, real or synthetic.
- Do not claim or imply live shelter or service capacity from HUD PIT/HIC data or from the synthetic dataset.
- Do not automate a consequential placement or eligibility decision; every handoff must show a human confirmation point.
- Do not build anything that replaces or bypasses Coordinated Entry.
