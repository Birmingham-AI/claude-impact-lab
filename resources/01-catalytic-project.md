# Resources: Choose Birmingham's Next Big Civic Project

Challenge brief: [../challenges/01-catalytic-project.md](../challenges/01-catalytic-project.md)

## Birmingham sources

- Community Foundation report: https://www.cfbham.org/report-to-the-community-2023/
- Community Foundation monthly update: https://www.cfbham.org/monthlyupdate/
- Birmingham Business Alliance Accelerate 2030: https://www.birminghambusinessalliance.com/accelerate-2030/
- Prosper Birmingham dashboard: https://prosperbham.com/dashboard/

## National sources

- Collective Impact framework: https://collectiveimpactforum.org/what-is-collective-impact/
- USAspending API: https://api.usaspending.gov/

## Synthetic dataset

[data/catalytic-project-candidates.csv](data/catalytic-project-candidates.csv)

**This dataset is entirely synthetic. It contains five clearly fictional candidate projects. It does not represent any real proposal, endorsement, or consensus, and must not be presented as real, live, or authoritative.**

Columns: `candidate_id`, `candidate_name`, `primary_beneficiary`, `proposed_owner`, `evidence_strength`, `estimated_time_horizon`, `key_dependency`, `first_commitment`, `is_synthetic`.

## 30-minute quick start

1. Open [data/catalytic-project-candidates.csv](data/catalytic-project-candidates.csv) and pick three of the five fictional candidates.
2. Choose one civic convener as your primary user and one moment: comparing candidates to decide what to rally behind.
3. Pick three to four comparison factors visible in the CSV (for example `evidence_strength`, `estimated_time_horizon`, `key_dependency`, `primary_beneficiary`) and note why each factor matters.
4. Map each candidate against the five Collective Impact conditions (common agenda, shared measurement, mutually reinforcing activities, continuous communication, backbone support) using the `proposed_owner` and `first_commitment` columns as a starting point.
5. Produce a first artifact: a one-page comparison table, a transparent rubric, or a stakeholder next-step map showing who could act first.

## Download or API notes

- The Community Foundation report and monthly update, Birmingham Business Alliance page, and Prosper Birmingham dashboard are standard web pages; read them directly or save a PDF/screenshot for citation. No bulk download has been verified for these.
- The Collective Impact Forum page is a reference article, not a data source; use it to structure your framework, not to pull data.
- For USAspending, use the documented API described at https://api.usaspending.gov/ rather than guessing endpoints or parameters. If you have not tested a specific call, do not describe it as verified; follow the official API documentation for request format and any rate limits.

## Freshness and limitations

- Links were checked on August 27, 2026.
- The Community Foundation report, Birmingham Business Alliance page, and Prosper Birmingham dashboard describe published plans and historical/system-level information, not live, real-time status.
- USAspending award data reflects federal award geography and does not by itself indicate local consensus, need, or impact in Birmingham. The most important limitation for this track: award or funding data is not evidence of stakeholder agreement, and must not be treated as proof that a project has local support.

## Licensing and terms

- Follow the terms, attribution, and rate-limit rules published on each Birmingham and national source site. Linking to a source here does not grant any right to redistribute its content or data.
- The USAspending API is a public federal data source; still check and follow its published usage terms and any rate limits.
- The synthetic candidate CSV may be copied and modified for your event project, but any copy must keep the `is_synthetic` label and must not be presented as a real proposal or endorsement.

## Prohibited uses

- Do not claim that any candidate has Birmingham-wide consensus or stakeholder agreement that has not been shown in the artifact.
- Do not treat USAspending award geography, dollar amounts, or recipient data as proof of local impact, need, or endorsement.
- Do not present the synthetic candidates as real proposals, real organizations, or real commitments.
- Do not build an opaque score with no visible explanation of factors.
