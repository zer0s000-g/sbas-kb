---
title: Source - SDCM
description: Institutional source note for the Russian System of Differential Corrections and Monitoring, based on official GLONASS/IAC, ICAO, UNOOSA, and bounded public comparator sources
tags: [source, sdcm, glonass, russia, sbas, service-provider, provenance]
source_type: service-provider-and-system-development-source
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: official-glonass-iac-and-public-icao-unoosa-reviewed-with-operational-boundaries
---

# Source - SDCM

## Scope of this note

This source note records the current authenticated public-source posture for the Russian System of Differential Corrections and Monitoring (SDCM).

Use this note only for:

- SDCM identity as a Russian / GLONASS-related augmentation system;
- GLONASS Information and Analysis Center source posture around GLONASS Open Service Performance Standard material;
- ICAO public working-paper statements that SDCM work was underway and intended as a GLONASS SBAS augmentation path;
- bounded development/status context from UNOOSA-hosted Russian GNSS presentations and public SBAS summaries.

Do not use this note to claim current aviation operational approval, published LPV/APV procedures, service-volume commitments, real-time availability, or current certification status.

## Public sources reviewed

- GLONASS IAC system documents: `https://glonass-iac.ru/en/documents/`
- GLONASS Open Service Performance Standard Edition 2.2 PDF: `https://glonass-iac.ru/upload/docs/stehos/stehos_en.pdf`
- ICAO Assembly A37-WP/195: `https://www.icao.int/sites/default/files/Meetings/AMC/ArchivedAssembly/en/A37/Working%20Papers/wp-191-250/wp195_en.pdf`
- UNOOSA-hosted Russian GNSS / SDCM presentation path reviewed as supplemental public context.
- FAA SBAS Worldwide public factsheet reviewed only as external comparator context.

## Source identity table

| Source                                                        | Public identity signal                                                                                                                                     | Safe role in this KB                                                                                           | Boundary                                                                                    |
| ------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| GLONASS Information and Analysis Center system-documents page | Publishes the GLONASS Open Service Performance Standard and states that GLONASS OS PS is a basis for certification of GLONASS-based systems including SDCM | Official GLONASS-system source posture; confirms SDCM is within the GLONASS-based-system certification context | Does not provide a complete SDCM aviation service declaration or procedure inventory        |
| GLONASS OS PS Edition 2.2 (2020)                              | States that the OS PS is a basis for certification of GLONASS services, SDCM, SPOCD, and aviation user equipment                                           | Official GLONASS performance-standard relationship to SDCM                                                     | OS PS addresses GLONASS open SIS performance; it is not an SDCM service-definition document |
| ICAO Assembly A37-WP/195 (Russian Federation, 2010)           | States that work on SDCM as a GLONASS SBAS was underway and describes intended augmentation of GLONASS, GPS, and future Galileo                            | ICAO-public historical development signal                                                                      | 2010 status; not current operational evidence                                               |
| UNOOSA-hosted Russian GNSS/SDCM presentations                 | Public institutional context for SDCM monitoring facilities and development status                                                                         | Supplemental development/status context                                                                        | Presentation material is not a regulator/AIP service approval source                        |
| FAA SBAS Worldwide public factsheet                           | Lists SDCM as under development and augmenting GPS/GLONASS                                                                                                 | External public comparator signal only                                                                         | Not an SDCM authority and not a Russian service declaration                                 |

## Extracted official/public signals

### GLONASS IAC system-documents signal

The GLONASS Information and Analysis Center identifies the GLONASS Open Service Performance Standard as an official GLONASS system document. The portal states that the standard is developed and sustained by the Information and Analysis Center for Positioning, Navigation and Timing of TsNIIMash, coordinated with and approved by the Russian Ministry of Defense and Roscosmos State Corporation.

The portal explicitly states that GLONASS OS PS supports certification of GLONASS-based systems including SDCM. This is the strongest current official public signal for placing SDCM inside the GLONASS institutional/source family.

### GLONASS OS PS signal

The extracted GLONASS OS PS material states that the standard is a baseline interface between GLONASS and user equipment manufacturers/service developers. It is described as a basis for certification of GLONASS services, SDCM, SPOCD, and aviation user equipment.

Important boundary: the OS PS describes GLONASS open service Signal-in-Space performance and related GLONASS system standards. It does not itself define an aviation SDCM Safety-of-Life service, runway procedures, APV/LPV procedure availability, or operator authorization.

### ICAO A37-WP/195 signal

The ICAO Assembly 37th Session working paper presented by the Russian Federation states that the SDCM was a GLONASS space-based augmentation system under development. It describes intended support for:

- integrity information;
- refined ephemeris-time information;
- corrected measurement data;
- GNSS constellation health status.

It also describes SDCM as augmenting GLONASS, GPS, and Galileo in the future.

Important boundary: this is a 2010 ICAO working-paper development signal. It must not be reused as current status without newer Russian regulator/service-provider evidence.

### Public comparator signal

The FAA SBAS Worldwide public factsheet lists SDCM as under development and as augmenting GPS and GLONASS. This is useful as an external public comparator signal, but it is not an SDCM authority.

## What this source can currently anchor

- SDCM means System of Differential Corrections and Monitoring / System for Differential Correction and Monitoring in the Russian GLONASS augmentation context.
- SDCM belongs to the Russian / GLONASS augmentation source family.
- GLONASS IAC and GLONASS OS PS public material connect SDCM to GLONASS-based-system certification context.
- ICAO public material confirms that SDCM work was underway as a GLONASS SBAS development path and describes intended augmentation information types.
- Public comparator material can describe SDCM conservatively as under-development / development-status unless newer official sources are extracted.

## What this source must not be used for

Do not use this note for:

- current aviation operational service declaration;
- LPV/APV approach availability in Russia or surrounding regions;
- aircraft/operator approval;
- AIP procedure publication;
- current service-volume, availability, integrity, continuity, or time-to-alert commitments;
- claims that SDCM is operationally equivalent to WAAS, EGNOS, MSAS, GAGAN, KASS, BDSBAS, or SouthPAN;
- comparative performance or maturity ranking;
- Annex 10 / DO-229 compliance conclusions beyond direct source text.

## Relationship to other source notes

| Related note                                  | Relationship                                                                                     |
| --------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| [[Source - SBAS Service Providers]]           | Family router for service-provider and system identity claims                                    |
| [[SDCM]]                                      | Downstream system note using this source only within stated boundaries                           |
| [[Source - ICAO Annex 10 Volume I GNSS SBAS]] | ICAO SARPs routing; not an SDCM service declaration                                              |
| [[Source - ICAO Doc 9849]]                    | GNSS implementation guidance routing; not an SDCM status source                                  |
| [[Source - RTCA DO-229]]                      | Airborne equipment MOPS routing; not an SDCM service source                                      |
| [[SBAS Operational Validation Dashboard]]     | Tracks what would be required before SDCM or any other system can support procedure-level claims |

## Future extraction targets

Before upgrading SDCM beyond bounded-development status, extract:

1. current Russian official SDCM service-definition or status pages;
2. Roscosmos / GLONASS IAC / operator material specific to SDCM rather than GLONASS OS generally;
3. Russian aviation regulator or AIP material for any claimed aviation use;
4. current GEO/space-segment and monitoring-network status from official public sources;
5. any ICAO regional or state paper after the historical A37-WP/195 development signal.

## See also

- [[SDCM]]
- [[Source - SBAS Service Providers]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS Source Backlog]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Operational Validation Dashboard]]
