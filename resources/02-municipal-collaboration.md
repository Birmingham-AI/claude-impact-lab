# Resources: Make Regional Services Easier to Navigate

Challenge brief: [../challenges/02-municipal-collaboration.md](../challenges/02-municipal-collaboration.md)

## Birmingham sources

- Community Foundation regional cooperation: https://www.cfbham.org/driving-regional-cooperation/
- Jefferson County local governments: https://www.jeffcoda.org/Default.asp?ID=748&pg=Local+Government
- Regional Planning Commission data and maps: https://www.rpcgb.org/data-maps-overview
- City of Birmingham transparency resources: https://www.birminghamal.gov/government/mayors-office/transparency
- Personnel Board participating agencies: https://www.pbjcal.org/Agencies

## National sources

- Census TIGERweb: https://tigerweb.geo.census.gov/
- Census TIGERweb REST services: https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_restmapservice.html

## Synthetic dataset

[data/municipal-service-cases.csv](data/municipal-service-cases.csv)

**This dataset is entirely synthetic. It contains six clearly fictional service cases at synthetic locations. It does not represent any real resident, case, or agency determination, and must not be presented as real, live, or authoritative.**

Columns: `case_id`, `service_type`, `synthetic_location`, `jurisdiction_a`, `jurisdiction_b`, `authoritative_source`, `conflict_or_gap`, `recommended_handoff`, `requires_human_confirmation`, `is_synthetic`.

## 30-minute quick start

1. Open [data/municipal-service-cases.csv](data/municipal-service-cases.csv) and pick one fictional case.
2. Choose a primary user (resident or frontline staff) and the moment "who owns this?" for that one `service_type`.
3. Map the handoff for that case: `jurisdiction_a` vs `jurisdiction_b`, the `authoritative_source`, the `conflict_or_gap`, and what remains unknown.
4. Mark the point where `requires_human_confirmation` applies and who should confirm it before any action is taken.
5. Produce a first artifact: a small routing prototype, an ownership matrix across the case's jurisdictions, or a one-page handoff card.

## Download or API notes

- The Community Foundation, Jefferson County, RPCGB, City of Birmingham transparency, and Personnel Board pages are standard web pages; read and cite them directly. No bulk download has been verified for these.
- For Census TIGERweb, use the REST map service documentation at https://tigerweb.geo.census.gov/tigerwebmain/TIGERweb_restmapservice.html to construct queries rather than guessing parameters. Treat TIGERweb layers as geographic reference boundaries, not as an eligibility or service-responsibility API.

## Freshness and limitations

- Links were checked on August 27, 2026.
- The Birmingham and Jefferson County pages describe published organizational structure and policy, not live case status or current queue information.
- TIGERweb provides current Census geographic boundaries but is not a legal or administrative record of which agency is responsible for a service. The most important limitation for this track: geographic boundaries from TIGERweb do not determine legal service responsibility, and a boundary lookup is not the same as an agency's actual jurisdiction determination.

## Licensing and terms

- Follow the terms, attribution, and rate-limit rules published on each Birmingham and national source site. Linking to a source here does not grant any right to redistribute its content or data.
- Census TIGERweb services are public federal data; still check and follow the published usage terms and any request limits.
- The synthetic case CSV may be copied and modified for your event project, but any copy must keep the `is_synthetic` label and must not be presented as a real resident case or agency determination.

## Prohibited uses

- Do not send real tickets, service requests, or referrals to any agency, live or synthetic.
- Do not imply that a municipality, county, or agency has approved, endorsed, or confirmed a routing decision your artifact produces.
- Do not use TIGERweb boundary data alone to make or imply a legal responsibility determination.
- Do not present synthetic cases as real residents, real addresses, or real agency records.
