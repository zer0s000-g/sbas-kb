---
title: Source - RTCA DO-289
description: Red-flag source note documenting that public catalog signals identify RTCA DO-289 as aircraft-surveillance related, not as an SBAS performance-testing anchor
tags: [source, rtca, do-289, surveillance, ads-b, red-flag, provenance]
source_type: standard
created: 2026-04-23
modified: 2026-05-02
status: red-flag
verification_status: public-catalog-mismatch
---

# Source - RTCA DO-289

## Scope of this note

This note records a provenance correction. Earlier vault scaffolding treated RTCA DO-289 as if it were an SBAS performance-testing or monitoring standard. Public catalog signals reviewed in this cycle instead identify RTCA DO-289 as an aircraft-surveillance-applications standard.

Important boundary:

- This note is not a completed extraction from the RTCA document itself.
- The public-catalog signal is sufficient to flag prior SBAS-specific use as likely mis-scoped.
- Do not use DO-289 as a source anchor for SBAS testing, SBAS monitoring, LPV, protection levels, alert limits, or SBAS service performance unless later direct-source review proves a specific relevant linkage.

## Public-catalog identity signal

| Field | Current public-catalog signal |
|---|---|
| Issuing body | RTCA, Inc. |
| Document | DO-289 |
| Public title signal | Minimum Aviation System Performance Standards (MASPS) for Aircraft Surveillance Applications (ASA) |
| Publication-date signal | 2006-12-13 for the cataloged current item |
| Scope signal | ADS-B / aircraft-surveillance application parameter clarification and surveillance applications |
| SBAS relevance signal | Not identified as an SBAS performance-testing standard in the reviewed public catalog material |

## Provenance correction

Previous in-vault wording described DO-289 as an SBAS performance testing or monitoring source. Treat that mapping as superseded by this red flag until direct source review identifies the intended standard.

Likely downstream action:

- Remove DO-289 from SBAS source-priority lists except as a red-flag / mis-scoped reference.
- Do not route SBAS performance-monitoring claims to DO-289.
- Look for the actual SBAS monitoring source family in ICAO Annex 10, ICAO Doc 9849, service-definition documents, ANSP/service-provider performance reports, and regulator guidance.

## Downstream cleanup targets

- [[SBAS-Standards-Regulation]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[SBAS-Research-MOC]]
- [[SBAS in Civil Aviation MOC]]

## See also

- [[SBAS Standards Source Matrix]]
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-229]]
- [[SBAS Source Backlog]]
- [[SBAS MOC]]
