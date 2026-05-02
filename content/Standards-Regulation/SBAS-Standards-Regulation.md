---
title: SBAS Standards and Regulation
description: Source-disciplined overview of SBAS standards, regulatory source families, and claim boundaries for institutional knowledge-base use
tags: [standards, regulation, icao, rtca, eurocae, certification, source-discipline]
category: standards
created: 2026-04-19
modified: 2026-05-02
version: 2.0
status: reviewed
verification_status: public-catalog-reviewed-with-open-source-extraction
---

# SBAS Standards and Regulation

## Scope

This page is an institutional orientation to SBAS standards and regulatory source families. It is designed to help readers understand which documents and institutions may support which types of claims.

It is not an operational compliance manual. Do not use this page to determine procedure minima, aircraft eligibility, receiver certification, crew authorization, service availability, or regulatory compliance. Those decisions require the applicable official standards, regulator material, service-provider documentation, aircraft/avionics approval basis, AIP/procedure publications, and operator procedures.

## Current source posture

This standards branch has moved from a draft list of document names to a source-disciplined map. The most important correction is that several earlier document mappings were too broad or apparently incorrect.

Use [[SBAS Standards Source Matrix]] as the current routing table.

## Standards source families

| Source family | Typical claim boundary | Current KB anchor |
|---|---|---|
| ICAO SARPs / technical provisions | Global aviation baseline for aeronautical telecommunications, GNSS, and augmentation requirements | Dedicated Annex 10 source note still needed |
| ICAO implementation guidance | State introduction of GNSS operations, implementation considerations, monitoring/assessment/reporting | [[Source - ICAO Doc 9849]] |
| RTCA / EUROCAE airborne equipment standards | Receiver/equipment performance, equipment classes, test methods, and avionics capability | [[Source - RTCA DO-229]] is the current GPS/SBAS airborne-equipment anchor |
| Procedure-design criteria | Procedure construction, minima design, coding assumptions, obstacle assessment | Dedicated PANS-OPS / procedure-design source notes still needed |
| Regulator / ANSP / AIP sources | State implementation, operational approval, published procedures, and actual availability | Regional and country source notes still being built |
| Service-provider documents | Service definition, coverage, performance, NOTAM/status practices, system-specific operational commitments | Future service-provider source notes needed for each SBAS system |

## Confirmed correction register

| Earlier in-vault mapping | Current correction | Resulting editorial rule |
|---|---|---|
| ICAO Doc 9855 as SBAS technical specification | Public ICAO catalog identifies Doc 9855 as Guidelines on the Use of the Public Internet for Aeronautical Applications | Do not cite Doc 9855 for SBAS technical claims |
| ICAO Doc 9854 as SBAS/GBAS performance testing and monitoring | Public ICAO catalog identifies Doc 9854 as Global Air Traffic Management Operational Concept | Do not cite Doc 9854 for SBAS performance-testing claims |
| RTCA DO-242 as GNSS augmentation/integrity standard | Public catalog identifies DO-242 as ADS-B related | Do not cite DO-242 for SBAS integrity or augmentation-system claims |
| RTCA DO-289 as SBAS performance-testing standard | Public catalog identifies DO-289 as aircraft surveillance applications | Do not cite DO-289 for SBAS monitoring or testing claims |

These corrections are intentionally preserved as red-flag source notes rather than deleted, so future editors can see why older draft references changed.

## Current high-confidence anchors

### RTCA DO-229

[[Source - RTCA DO-229]] is the current public-catalog-reviewed anchor for GPS/SBAS airborne equipment. It can route claims about airborne receiver/equipment source family support, but detailed numerical requirements and compliance interpretations still require direct extraction from the official RTCA standard and applicable regulator material.

### ICAO Doc 9849

[[Source - ICAO Doc 9849]] is the current public-catalog-reviewed anchor for ICAO GNSS implementation guidance. It is useful for state implementation and GNSS/SBAS introduction context, but it must not be used alone as a normative requirements source.

## Claim boundaries by topic

| Topic | What this page may say now | What remains source-pending |
|---|---|---|
| SBAS concept and architecture | SBAS is a GNSS augmentation architecture involving ground monitoring, correction/integrity processing, broadcast, and receiver use | Exact SARPs, message definitions, service commitments, and performance values |
| Airborne SBAS equipment | DO-229 is the correct current source-family anchor for GPS/SBAS airborne-equipment MOPS | Revision-specific requirements, tests, equipment classes, alerting details |
| LPV and approach operations | LPV operational use depends on service, equipment, procedure, approval, and real-time integrity conditions | Minima, eligibility, procedure-design rules, and country/operator approval details |
| Integrity / protection levels / alert limits | The conceptual relationship can be explained safely | Exact definitions, thresholds, and operation-specific values |
| System comparisons | Source posture can be compared | Performance rankings and availability claims require service-provider evidence |

## Immediate institutional source-building needs

1. Dedicated source note for ICAO Annex 10, Volume I GNSS/SBAS material.
2. Direct extraction of [[Source - RTCA DO-229]] for airborne-equipment and integrity-related language.
3. Direct extraction of [[Source - ICAO Doc 9849]] for state GNSS implementation and SBAS monitoring guidance.
4. Procedure-design source notes before further expanding LPV/LNAV/VNAV/RNAV/RNP/GBAS procedure pages.
5. Service-provider source notes for WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, SouthPAN, and other systems before comparative performance tables.

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9849]]
- [[Source - ICAO Doc 9854]]
- [[Source - ICAO Doc 9855]]
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-289]]
- [[SBAS Integrity]]
- [[LPV-Approach-Procedure]]
- [[SBAS MOC]]
