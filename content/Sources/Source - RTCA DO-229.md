---
title: Source - RTCA DO-229
description: Source note for RTCA DO-229 as the GPS/SBAS airborne-equipment MOPS anchor, with public RTCA product metadata, regulatory cross-signals, and strict downstream claim boundaries
tags: [source, rtca, do-229, sbas, gps, aviation, airborne-equipment, mops, receiver]
source_type: standard
created: 2026-04-23
modified: 2026-05-02
status: active
verification_status: public-product-and-regulatory-signal-reviewed-not-official-text-extracted
---

# Source - RTCA DO-229

## Scope of this note

This note is the knowledge base's current source-family anchor for **RTCA DO-229**, the Minimum Operational Performance Standards (MOPS) family for GPS/SBAS airborne equipment.

It has been tightened using public RTCA product metadata, public standards-catalog metadata, and regulator/agency cross-signals. It is still **not** a completed extraction from the official RTCA standard text.

Important boundary:

- Public product and catalog metadata can support document identity, revision signals, broad equipment scope, and high-level source-family routing.
- Public regulator/ETSO pages can support the fact that DO-229 is used in equipment approval frameworks and that installation/operation approvals remain separate. Dedicated FAA and EASA approval-source notes now exist as [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]].
- Public metadata cannot safely support detailed numerical requirements, test tolerances, receiver algorithms, alerting thresholds, annunciation behavior, operational minima, or compliance interpretations.
- Use this note to route claims to the correct source family. Do not use it as a substitute for the official RTCA document, FAA/EASA TSO/ETSO text, aircraft installation approval, avionics manuals, operator approval, regulator guidance, AIP/procedure material, or procedure-design criteria.

## Public identity and revision signals

| Field                                        | Current public signal                                                                                                                                                          |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Issuing body                                 | RTCA, Inc.                                                                                                                                                                     |
| Committee signal                             | RTCA SC-159 on public RTCA product pages                                                                                                                                       |
| Document family                              | DO-229                                                                                                                                                                         |
| Current RTCA product signal reviewed         | DO-229F, issued 2020-06-11                                                                                                                                                     |
| DO-229F public title signal                  | MOPS for Global Positioning System/Satellite-Based Augmentation System Airborne Equipment                                                                                      |
| Prior revision signal reviewed               | DO-229E, issued 2016-12-15, superseding DO-229D and incorporating Change 1 per public RTCA product metadata                                                                    |
| Public standards-catalog signal              | DO-229 active/current item; 2020-06-11 publication-date signal; page-count signal of 540 pages in one consulted catalog                                                        |
| Broad scope signal                           | Airborne navigation equipment using GPS augmented by SBAS                                                                                                                      |
| Important frequency boundary                 | Public RTCA/standards-catalog text states DO-229 provides standards for single-frequency airborne navigation equipment; dual-frequency equipment is to be addressed separately |
| U.S. SBAS example in public title/scope text | WAAS as the U.S. SBAS example                                                                                                                                                  |

## Publicly visible scope signal

Public RTCA and standards-catalog descriptions identify DO-229 as a MOPS document for airborne navigation equipment using GPS augmented by SBAS. Public product text for DO-229F states that DO-229 is limited to **single-frequency** airborne navigation equipment and that a separate document is expected for dual-frequency equipment.

For this knowledge base, that supports a narrow but important editorial decision:

```text
DO-229 is the receiver/equipment MOPS source family for GPS/SBAS airborne equipment.
It is not the primary source family for SBAS ground-system certification, service status,
procedure design, state approval, or regional operational availability.
```

## Version-specific public signals

### DO-229F public signal

The RTCA product page for DO-229F identifies it as issued in 2020 and describes the revision as adding requirements tags to support future dual-frequency, multi-constellation MOPS development. That public signal is useful for source routing because it confirms two points:

1. DO-229F is still a single-frequency GPS/SBAS airborne-equipment MOPS anchor.
2. DFMC development is adjacent to, but not itself solved by, DO-229F.

### DO-229E public signal

The RTCA product page for DO-229E identifies it as issued in 2016 and as superseding DO-229D while incorporating Change 1. The same public product text describes changes including new SBAS PRN codes, clarifications, and a new requirement related to preventing use of the Navigation Message Correction Table.

This KB should not convert those public summaries into detailed technical requirements. The public revision signal is sufficient only to warn editors that revision baseline matters.

## Regulatory and approval-context signals

### FAA TSO distinction

The FAA's public Technical Standard Orders page defines a TSO as a minimum performance standard used to evaluate an article. It also states that receiving a TSO Authorization is **not** an approval to install and use the article in an aircraft; separate aircraft airworthiness approval is required for installation.

Editorial implication:

```text
A DO-229/TSO equipment claim is not the same as an aircraft installation approval,
operator approval, procedure authorization, or LPV availability claim.
```

### EASA ETSO cross-signal

Public EASA ETSO material for GPS/SBAS navigation sensors and stand-alone GPS/SBAS navigation equipment references DO-229E Section 2, with modifications in ETSO appendices, as a minimum performance standard basis for certain equipment classes. The extracted EASA source-routing layer is now represented by [[Source - EASA ETSO-C145e and ETSO-C146e]]. The FAA counterpart is represented conservatively by [[Source - FAA TSO-C145e and TSO-C146e]].

Editorial implication:

- DO-229 is visibly used in airborne GPS/SBAS equipment approval frameworks.
- The applicable approval path can depend on jurisdiction, ETSO/TSO revision, equipment class, appendices/modifications, installation basis, and aircraft-level requirements.
- The KB must not collapse DO-229, FAA TSO, EASA ETSO, aircraft installation approval, and operational approval into one claim.

## What this source can currently anchor

Until the official RTCA standard text is extracted and section-mapped, this note can safely anchor only source-family and document-identity statements such as:

- DO-229 belongs to the airborne GPS/SBAS receiver/equipment MOPS source family.
- DO-229 is relevant to GPS/SBAS airborne equipment rather than to SBAS ground-segment certification as a whole.
- DO-229 is a plausible source family to investigate for equipment classes, receiver performance, SBAS-based RNAV equipment, LP/LPV-capable equipment context, integrity-related receiver behavior, and test methods.
- DO-229F public metadata indicates a single-frequency scope and a relationship to future DFMC MOPS development, but it should not be used as a DFMC requirements source.
- FAA/EASA public material confirms that equipment approval frameworks may reference DO-229, but installation and operational approvals remain separate; use [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]] for approval-layer routing.

## What this source must not be used for yet

Do not use this note alone to publish or validate:

- exact LPV minima, decision heights, alert limits, time-to-alert values, accuracy values, continuity values, or availability values;
- detailed protection-level formulas, algorithmic assumptions, test tolerances, or receiver annunciation logic;
- procedure-design requirements for LPV, LP, LNAV/VNAV, RNAV, RNP, or GBAS;
- SBAS ground-system certification, service definition, outage reporting, or operational service status;
- aircraft eligibility, installation approval, operational approval, crew authorization, or operator procedure claims;
- dual-frequency or multi-constellation SBAS equipment requirements;
- claims that a particular aircraft, receiver, operator, runway, procedure, or region is approved for LPV or any other SBAS-supported operation.

## Claim-boundary classification

| Claim type                                                  | Current DO-229 support status                                                                                                       | Documentation action                                                                                                                            |
| ----------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Airborne GPS/SBAS receiver/equipment MOPS                   | Strong public product/catalog support                                                                                               | Link to this note, but keep detailed requirements pending official-text extraction                                                              |
| Equipment classes and approval basis                        | Public regulator/ETSO cross-signals show relevance; FAA/EASA source notes now exist; details remain revision/jurisdiction dependent | Route to DO-229 plus [[Source - FAA TSO-C145e and TSO-C146e]] / [[Source - EASA ETSO-C145e and ETSO-C146e]] before making class-specific claims |
| LP/LPV/LNAV/VNAV equipment capability                       | Broad public support as an equipment-source family; operational meaning still depends on procedure and approval layers              | Use cautious conceptual phrasing and keep values out                                                                                            |
| Receiver integrity, protection-level, and alerting behavior | Plausible DO-229 extraction target                                                                                                  | Do not publish algorithms, thresholds, or annunciation behavior until extracted from official source text                                       |
| SBAS ground-system certification                            | Not the primary DO-229 claim family                                                                                                 | Route to [[Source - ICAO Annex 10 Volume I GNSS SBAS]], service-provider, and regulator sources                                                 |
| Procedure design and minima                                 | DO-229 is not sufficient                                                                                                            | Route to PANS-OPS/PBN, regulator, AIP/procedure chart, and operator sources                                                                     |
| Aircraft installation and operational approval              | DO-229/TSO/ETSO evidence is not sufficient                                                                                          | Route to aircraft certification, installation approval, regulator, and operator sources                                                         |
| Service availability and regional status                    | Not supported by DO-229                                                                                                             | Route to service-definition, NOTAM/status, ANSP/AIP, and provider performance sources                                                           |
| DFMC SBAS equipment                                         | Public product/catalog text warns that DO-229 is single-frequency                                                                   | Treat as out of scope unless a dedicated DFMC MOPS/source note is created                                                                       |

## Downstream documentation rules

When editing downstream pages:

1. Use DO-229 language for airborne equipment and receiver-source routing only.
2. Pair DO-229 with [[Source - FAA TSO-C145e and TSO-C146e]], [[Source - EASA ETSO-C145e and ETSO-C146e]], or another applicable regulator source before making equipment-approval statements.
3. Pair DO-229 with procedure-design, AIP/AIS, and operator/regulator sources before making operational LPV or minima statements.
4. Pair DO-229 with Annex 10 and service-provider sources before making system-level SBAS or signal/service claims.
5. Treat revision identity as material: DO-229D/E/F and regulator-modified appendices may not support identical downstream statements.
6. Keep numerical values out of concept pages unless each value has a visible source, applicability condition, revision/date, and operational context.

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
- [[WAAS]]

## Extraction template for a future official-text cycle

### Bibliographic metadata

- issuing body:
- exact title:
- document number:
- revision / change number:
- publication date:
- official access path / institutional library record:
- applicable FAA TSO / EASA ETSO / other regulator references, including [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]] where relevant:

### Sections to extract cautiously

- equipment classes and intended functions;
- receiver performance requirements;
- SBAS signal and message assumptions;
- LP, LPV, LNAV, LNAV/VNAV, and RNAV-related equipment capability language;
- integrity, alerting, protection-level, and receiver usability language;
- test methods, environmental assumptions, and verification conditions;
- revision-specific exclusions, assumptions, and applicability limits;
- any explicit DFMC boundary or transition material.

### Downstream mapping questions

- Which claims belong in [[SBAS Integrity]]?
- Which claims belong in [[Protection Levels]] and [[Alert Limits]]?
- Which claims belong in [[LPV-Approach-Procedure]]?
- Which claims belong in architecture or terminology pages?
- Which claims require [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]], FAA/EASA/regulator, service-provider, AIP/AIS, or procedure-design sources in addition to DO-229?

## Public sources reviewed

- RTCA Community Hub, DO-229F product page: `https://my.rtca.org/productdetails?id=a1B1R0000092ubbUAA`
- RTCA Community Hub, DO-229E product page: `https://my.rtca.org/NC__Product?id=a1B3600000211rIEAQ`
- GlobalSpec standards catalog page for RTCA DO-229: `https://standards.globalspec.com/std/14281994/rtca-do-229`
- FAA Technical Standard Orders page: `https://www.faa.gov/aircraft/air_cert/design_approvals/tso`
- FAA DRS record for TSO-C145e: `https://drs.faa.gov/browse/excelExternalWindow/EFE54F1E6272A7068625811D0064B679.0001`
- FAA DRS record for TSO-C146e: `https://drs.faa.gov/browse/excelExternalWindow/EFE10BFF3187F9A78625811A005E32A6.0001`
- EASA ETSO-C145e public PDF: `https://www.easa.europa.eu/download/etso/ETSO-C145e_CS-ETSO_13.pdf`
- EASA ETSO-C146e A1 public PDF: `https://www.easa.europa.eu/download/etso/ETSO-C146e_A1.pdf`
- ESA Navipedia SBAS Standards page, used only as secondary orientation: `https://gssc.esa.int/navipedia/index.php/SBAS_Standards`

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - FAA TSO-C145e and TSO-C146e]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS MOC]]
