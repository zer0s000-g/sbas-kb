---
title: Source - RTCA DO-229
description: Source note for RTCA DO-229 as the GPS/SBAS airborne-equipment MOPS anchor, with public RTCA product metadata, regulatory cross-signals, and strict downstream claim boundaries
tags: [source, rtca, do-229, sbas, gps, aviation, airborne-equipment, mops, receiver]
source_type: standard
created: 2026-04-23
modified: 2026-05-03
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

|| Field | Current public signal |
|| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
|| Issuing body | RTCA, Inc. |
|| Committee signal | RTCA SC-159 on public RTCA product pages |
|| Document family | DO-229 |
|| Current RTCA product signal reviewed | DO-229F, issued 2020-06-11 |
|| DO-229F public title signal | MOPS for Global Positioning System/Satellite-Based Augmentation System Airborne Equipment |
|| Prior revision signal reviewed | DO-229E, issued 2016-12-15, superseding DO-229D and incorporating Change 1 per public RTCA product metadata |
|| Public standards-catalog signal | DO-229 active/current item; 2020-06-11 publication-date signal; page-count signal of 540 pages in one consulted catalog |
|| Broad scope signal | Airborne navigation equipment using GPS augmented by SBAS |
|| Important frequency boundary | Public RTCA/standards-catalog text states DO-229 provides standards for single-frequency airborne navigation equipment; dual-frequency equipment is to be addressed separately |
|| Relevant ICAO SARPs reference | Annex 10 Volume I Chapter 3, Section 3.5 (SBAS provisions); Section 3.6 (GBAS provisions); Appendix B (GNSS technical specifications) |

## Section and structure signals (from public sources)

Public ICAO SBAS implementation guidance and regulator AIP/Navigation documentation reference the following DO-229 structural elements:

|| Structural element | Signal source | Content signal |
|| -------------------------- | -------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
|| Section 1 | Public RTCA/EASA ETSO cross-references | General requirements applicable to all GPS/SBAS airborne equipment classes |
|| Section 2 | EASA ETSO-C145e/C146e public PDFs | Class Beta, Gamma, Delta equipment minimum performance standards as modified by EASA appendices |
|| Appendix | FAA/ETSO cross-signals | Environmental and test procedure provisions |
|| Equipment Class Beta | EASA ETSO-C145e public PDF | Airborne navigation sensors using GPS augmented by SBAS; functional equipment per EASA class framework |
|| Equipment Class Gamma | EASA/FAA cross-signals | Stand-alone airborne navigation equipment with higher integrity/performance class |
|| Equipment Class Delta | EASA/FAA cross-signals | Highest integrity/performance class for stand-alone GPS/SBAS equipment; Delta-4 associated with LPV operations |
|| DFMC boundary | RTCA SC-159 public meeting summaries | DO-229F adds requirements tags for future DFMC development; DO-229F scope remains single-frequency L1/L5 (not yet DFMC) |
|| PRN expansion context | ICAO APAC SBAS implementation guide | DO-229E added new SBAS PRN codes (120–138 original; expanded to 139–158 in May 2017); receiver compatibility issues |

### SBAS avionics Class 1–4 capability structure

Public AIP and ICAO SBAS implementation guidance documents identify the following operational capability classes used in SBAS airborne equipment context:

|| Avionics class | Capability signal | Operational type |
|| -------------- | ---------------------------------------------------------- | ------------------------ |
|| Class 1 | Oceanic, domestic en-route, terminal, LNAV | Lateral guidance only |
|| Class 2 | Class 1 + LNAV/VNAV | 3D with vertical guidance |
|| Class 3 | Class 2 + LP and LPV | LPV precision approach |
|| Class 4 | Final approach segment only; LP/LPV with fail-down to LNAV | ILS alternative |

Important: These avionics classes describe equipment capability, not operational approval. A Class 3 or Class 4 receiver does not, by itself, mean a specific runway, procedure, operator, or region supports LPV operations. Operational approval requires separate procedure-design, regulator, operator, and AIP chart sources.

### DFMC and future multi-constellation boundary

The RTCA SC-159 public meeting summaries confirm that DO-229F remains a single-frequency L1/L5 GPS/SBAS MOPS. DFMC SBAS requirements are under active development in SC-159 and will be addressed in a separate document. DO-229F requirements tags signal future DFMC integration but are not themselves DFMC requirements. The knowledge base editorial rule is:

```text
DO-229F is the single-frequency GPS/SBAS airborne-equipment MOPS anchor.
DFMC SBAS equipment requires a separate MOPS document or version, not yet published in DO-229F scope.
```

## Publicly visible scope signal

Public RTCA and standards-catalog descriptions identify DO-229 as a MOPS document for airborne navigation equipment using GPS augmented by SBAS. Public product text for DO-229F states that DO-229 is limited to **single-frequency** airborne navigation equipment and that a separate document is expected for dual-frequency equipment.

The ICAO APAC SBAS implementation guidance identifies WAAS as the reference U.S. SBAS example within the DO-229 context. The PRN code expansion (original 120–138; expanded to 139–158 in May 2017) was introduced in DO-229E and affects receiver compatibility with newer GEO satellites.

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

- issuing body: RTCA, Inc.
- exact title: Minimum Operational Performance Standards (MOPS) for Global Positioning System/Satellite-Based Augmentation System Airborne Equipment
- document number: DO-229
- revision / change number: DO-229F (current); DO-229E (prior); DO-229D (superseded)
- publication date: DO-229F issued 2020-06-11; DO-229E issued 2016-12-15
- committee: RTCA SC-159 (GPS)
- official access path: RTCA Community Hub (rtca.org)
- related ICAO SARPs: Annex 10 Volume I Chapter 3, Section 3.5 (SBAS); Section 3.6 (GBAS); Appendix B (GNSS)
- applicable FAA TSO: TSO-C145e (Class Beta sensors), TSO-C146e (Class Delta-4 stand-alone); referenced by [[Source - FAA TSO-C145e and TSO-C146e]]
- applicable EASA ETSO: ETSO-C145e (Class Beta), ETSO-C146e A1 (Class Gamma/Delta CCA); referenced by [[Source - EASA ETSO-C145e and ETSO-C146e]]

### Sections to extract cautiously

**From Section 1 (general requirements — all classes):**

- general MOPS applicability and scope
- definitions and terminology
- minimum performance categories and pass/fail criteria
- environmental and interference conditions

**From Section 2 (equipment-class-specific minimum performance standards):**

- Class Beta equipment requirements (sensors; as referenced in EASA ETSO-C145e)
- Class Gamma equipment requirements (stand-alone, intermediate integrity)
- Class Delta equipment requirements (stand-alone, highest integrity; Delta-4 associated with LPV capability)
- LP/LPV/LNAV/VNAV/LNAV equipment capability language and alert-limit behavior
- protection-level and integrity-related receiver behavior
- SBAS signal reception, message decoding, and ionospheric correction assumptions
- receiver annunciation and alerting logic
- test methods, tolerances, and environmental conditions

**From appendices:**

- environmental test provisions
- antenna requirements (related to DO-228/DO-301 context)
- DFMC transition and boundary material (if present in DO-229F)

**Revision-specific material:**

- DO-229E PRN code expansion (120–138 original; 139–158 expanded) and receiver compatibility implications
- DO-229F requirements tags for future DFMC development (not yet DFMC requirements)
- navigation message correction table restrictions

**Explicit boundaries (do not extract as requirements):**

- DFMC SBAS requirements (out of scope of DO-229F)
- Ground-system certification requirements (Annex 10 / service-provider domain)
- Procedure minima and operational approval claims

### Downstream mapping questions

- Which claims belong in [[SBAS Integrity]]?
- Which claims belong in [[Protection Levels]] and [[Alert Limits]]?
- Which claims belong in [[LPV-Approach-Procedure]]?
- Which claims belong in architecture or terminology pages?
- Which claims require [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]], FAA/EASA/regulator, service-provider, AIP/AIS, or procedure-design sources in addition to DO-229?

## Public sources reviewed

- RTCA Community Hub, DO-229F product page: `https://my.rtca.org/productdetails?id=a1B1R0000092ubbUAA`
- RTCA Community Hub, DO-229E product page: `https://my.rtca.org/NC__Product?id=a1B3600000211rIEAQ`
- RTCA list of available documents (September 2020): `https://www.rtca.org/wp-content/uploads/2020/12/LIST-OF-AVAILABLE-DOCS-AS-OF-SETEMBER-2020-.pdf`
- GlobalSpec standards catalog page for RTCA DO-229: `https://standards.globalspec.com/std/14281994/rtca-do-229`
- FAA Technical Standard Orders page: `https://www.faa.gov/aircraft/air_cert/design_approvals/tso`
- FAA DRS record for TSO-C145e: `https://drs.faa.gov/browse/excelExternalWindow/EFE54F1E6272A7068625811D0064B679.0001`
- FAA DRS record for TSO-C146e: `https://drs.faa.gov/browse/excelExternalWindow/EFE10BFF3187F9A78625811A005E32A6.0001`
- EASA ETSO-C145e public PDF: `https://www.easa.europa.eu/download/etso/ETSO-C145e_CS-ETSO_13.pdf`
- EASA ETSO-C146e A1 public PDF: `https://www.easa.europa.eu/download/etso/ETSO-C146e_A1.pdf`
- ESA Navipedia SBAS Standards page, used only as secondary orientation: `https://gssc.esa.int/navipedia/index.php/SBAS_Standards`
- ICAO APAC GBAS/SBAS ITF7 preliminary draft SBAS implementation guidance document (May 2025 rev3), used as structural signal only: `https://www.icao.int/sites/default/files/APAC/Meetings/2025/2025%20GBASSBAS%20ITF7/3-Working%20Papers/A3-WP05-ATTM-Co-Chairs-Prelimary-Draft-SBAS-Implementation-Guidance-Document.pdf`
- GAGAN ENR 4.3 India AIM page (SBAS avionics class structure): `https://aim-india.aai.aero/eaip-v2-07-2023/eAIP/IN-ENR%204.3-en-GB.html`

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
