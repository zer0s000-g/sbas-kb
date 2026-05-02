---
title: Source - RTCA DO-229
description: Source note for RTCA DO-229 as the GPS/SBAS airborne-equipment MOPS anchor, with public-catalog metadata and source-extraction boundaries
tags: [source, rtca, do-229, sbas, aviation, airborne-equipment, mops]
source_type: standard
created: 2026-04-23
modified: 2026-05-02
status: active
verification_status: public-catalog-reviewed-not-source-extracted
---

# Source - RTCA DO-229

## Scope of this note

This note is the knowledge base's current source anchor for RTCA DO-229. It has been tightened using public standards-catalog metadata, but it is still not a completed extraction from the purchased RTCA standard itself.

Important boundary:

- Public catalog metadata can support document identity and broad scope.
- It cannot safely support detailed numerical requirements, test tolerances, alerting thresholds, receiver algorithms, or compliance interpretations.
- Use this note to route claims to the correct source family. Do not use it as a substitute for the RTCA document, FAA TSO material, aircraft installation approval, avionics manuals, operator approval, regulator guidance, or procedure-design criteria.

## Public-catalog identity signal

A public standards-catalog page identifies RTCA DO-229 as:

| Field | Current public-catalog signal |
|---|---|
| Issuing body | RTCA, Inc. |
| Document | DO-229 |
| Public title signal | Minimum Operational Performance Standards (MOPS) for Global Positioning System/Satellite-Based Augmentation System Airborne Equipment |
| Publication-date signal | 2020-06-11 for the cataloged current item |
| Catalog status signal | Active / most current in the consulted catalog |
| Scope signal | Airborne navigation equipment using GPS augmented by SBAS |
| Important single-frequency boundary | Public catalog text states the item provides standards for single-frequency airborne navigation equipment, with dual-frequency equipment to be addressed separately |

The catalog signal also says the document is technically equivalent to a DO-229E item. The exact revision lineage, amendment history, and legally applicable revision must still be checked against the official RTCA source and the applicable regulator/equipment approval basis.

## What this source can currently anchor

Until the actual standard is extracted, this note may support only broad routing statements such as:

- DO-229 belongs to the airborne-equipment / receiver-performance source family.
- DO-229 is relevant to GPS/SBAS airborne equipment rather than to SBAS ground-segment certification as a whole.
- DO-229 is a plausible source family for receiver classes, equipment performance, SBAS-based RNAV equipment, and LPV/LP capability discussions.

## What this source must not be used for yet

Do not use this note alone to publish:

- LPV minima, alert limits, time-to-alert values, accuracy figures, continuity figures, or availability figures;
- procedure-design requirements;
- claims about aircraft eligibility or operational approval;
- claims about dual-frequency / multi-constellation SBAS equipment;
- assertions that a particular aircraft, receiver, operator, or procedure is approved.

## Claim-boundary classification

| Claim type | Current DO-229 support status | Documentation action |
|---|---|---|
| Airborne SBAS receiver/equipment MOPS | Strong broad catalog support | Link to this note, but keep detailed requirements pending source extraction |
| LPV/LP/LNAV/VNAV equipment capability | Broad catalog support; details pending | Use cautious conceptual phrasing |
| SBAS ground-system certification | Not the primary anchor | Route to ICAO Annex 10 / service-provider / regulator sources when available |
| Procedure design and minima | Not sufficient alone | Route to PANS-OPS, AIP/procedure charts, regulator material, and operator approvals |
| Service availability | Not sufficient | Route to service-definition documents and real-time/status sources |
| DFMC SBAS equipment | Public-catalog text warns single-frequency scope | Treat as out of scope unless a newer/source-specific anchor is added |

## Current in-vault references

The vault currently links this source from standards, architecture, terminology, integrity, LPV, MOC, and regional-system pages. Those links are appropriate when they refer to airborne-equipment source family support. They should be tightened where a page needs system-level, procedure-design, or service-provider evidence instead.

## Downstream pages to audit

- [[SBAS-Standards-Regulation]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS-vs-Other-Standards]]
- [[SBAS-vs-Other-Augmentation-Methods]]

## Extraction template for a future direct-source cycle

### Bibliographic metadata

- issuing body:
- exact title:
- document number:
- revision / change number:
- publication date:
- access path / library record:
- applicable regulator references:

### Sections to extract cautiously

- equipment classes and intended functions;
- receiver performance requirements;
- SBAS signal and message assumptions;
- approach-capability classes and annunciation logic;
- alerting, integrity, and protection-level language;
- test methods and environmental assumptions;
- explicit exclusions, assumptions, and revision limits.

### Claims to map downstream

- Which claims belong in [[SBAS Integrity]]?
- Which claims belong in [[LPV-Approach-Procedure]]?
- Which claims belong in architecture or terminology pages?
- Which claims require FAA/EASA/regulator, service-provider, or procedure-design sources in addition to DO-229?

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - ICAO Doc 9849]]
- [[SBAS-Standards-Regulation]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS MOC]]
