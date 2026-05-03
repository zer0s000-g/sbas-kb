---
title: Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual
description: Institutional source-family anchor for ICAO procedure-design and PBN navigation specification material, with explicit boundaries separating procedure design from equipment, article approval, and operational authorization
tags: [source, icao, pans-ops, doc-8168, doc-9613, pbn, procedure-design, rnav, rnp, lpv, lnav-vnav]
source_type: standard
status: active
verification_status: public-catalog-reviewed-not-source-extracted
---

# Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual

## Scope of this note

This note is the knowledge base's institutional source-family anchor for ICAO procedure-design material that underlies LPV, LNAV/VNAV, RNAV, and RNP concepts.

Procedure-design standards, PBN navigation specifications, and operational-approval frameworks are distinct from:

- airborne-equipment MOPS (handled by [[Source - RTCA DO-229]]);
- article/equipment approval (handled by [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]]);
- service-provider commitment (covered by future service-provider source notes);
- regulator operational-approval, AIP/procedure publication, and crew/operator authorization (covered by regulator/ANSP/AIP material).

This note does **not** provide procedure minima, airport-specific decision heights, approach-chart data, or operational-authorization criteria. Those require the official PANS-OPS volumes, the PBN Manual, national AIPs, and regulator operational-approval material.

Important boundary:

- Public ICAO Store metadata can support document identity, purpose, and edition signals.
- It cannot support numerical obstacle-clearance values, exact minima, procedure-design calculations, or state-specific PBN implementation decisions.
- Use this note for source-family routing and to keep procedure-design claims separate from equipment-MOPS and service-commitment claims.

## Source identity signals (public catalog)

### ICAO Doc 8168 — PANS-OPS Volume II

| Field            | Current public signal                                                                                                                                                                              |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Issuing body     | ICAO                                                                                                                                                                                               |
| Document         | Doc 8168                                                                                                                                                                                           |
| Full title       | Procedures for Air Navigation Services (PANS) — Aircraft Operations — Volume II Construction of Visual & Instrument Flight Procedures                                                              |
| Edition          | 7th Edition, 2020 (with Corrigenda 1 and 2)                                                                                                                                                        |
| Publication type | PANS / Manual                                                                                                                                                                                      |
| Purpose signal   | "Intended for the guidance of procedures specialists and describes the essential areas and obstacle clearance requirements for the achievement of safe, regular instrument flight operations"      |
| Scope signal     | Provides basic guidelines to States, and to operators and organizations producing instrument flight charts, for uniform practices at aerodromes where instrument flight procedures are carried out |

### ICAO Doc 9613 — PBN Manual

| Field             | Current public signal                                                                                                                                                                                            |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Issuing body      | ICAO                                                                                                                                                                                                             |
| Document          | Doc 9613                                                                                                                                                                                                         |
| Full title        | Performance Based Navigation (PBN) Manual                                                                                                                                                                        |
| Edition           | 5th Edition, 2023                                                                                                                                                                                                |
| Publication type  | Manual                                                                                                                                                                                                           |
| Purpose signal    | "Identifies the relationship between RNAV and RNP applications and the advantages and limitations of choosing one or the other as the navigation requirement for an airspace concept"                            |
| Additional signal | "Provides practical guidance to States, ANSPs and airspace users on how to implement RNAV and RNP applications, and how to ensure that the performance requirements are appropriate for the planned application" |
| Important signal  | Encourages using existing navigation specifications where possible to avoid costly new certification requirements for individual airspaces                                                                       |

## What this source-family can currently anchor

Until direct extraction from the official PANS-OPS and PBN Manual texts is performed, this note can support broad routing statements such as:

- ICAO Doc 8168 Volume II is the ICAO procedure-design standard applicable to instrument flight procedures.
- ICAO Doc 9613 is the ICAO manual explaining PBN navigation specifications (RNAV and RNP) and implementation guidance.
- Procedure-design material is distinct from airborne-equipment MOPS and from service-provider commitment.
- LPV, LNAV/VNAV, RNAV, and RNP concepts cannot be fully specified by equipment standards alone; they require procedure-design, service, aircraft, operator, and regulator layers.

## What this source-family must not be used for yet

Do not use this note alone to publish:

- exact obstacle-clearance surfaces or numerical minima;
- specific approach-chart data or airport/runway eligibility;
- any numerical RNAV/RNP/alert-limit threshold asserted as procedurally correct;
- aircraft certification or operational-approval requirements in place of the correct AMC/GM, regulator, or operator material;
- comparative performance tables between SBAS, GBAS, or ILS based solely on catalog metadata.

## Relationship to other source notes in this knowledge base

| Procedure concept | Equipment/routing source                           | Procedure-design source                  | Article-approval source                                                                | Service/regulator layer                                  |
| ----------------- | -------------------------------------------------- | ---------------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| LPV               | [[Source - RTCA DO-229]] (airborne equipment MOPS) | This note (PANS-OPS / PBN Manual family) | [[Source - FAA TSO-C145e and TSO-C146e]] / [[Source - EASA ETSO-C145e and ETSO-C146e]] | Service-provider definition + AIP + operational approval |
| LNAV/VNAV         | [[Source - RTCA DO-229]]                           | This note                                | Same as above                                                                          | Same as above                                            |
| RNAV              | [[Source - RTCA DO-229]]                           | This note                                | Same as above                                                                          | Same as above                                            |
| RNP               | [[Source - RTCA DO-229]]                           | This note                                | Same as above                                                                          | Same as above                                            |

## Downstream pages to connect

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[GBAS-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS-Standards-Regulation]]

## Extraction template for future direct-source cycles

### Bibliographic metadata needed

- [ ] Exact edition, amendment/corrigendum baseline, and effective date
- [ ] Direct-text extraction of Table of Contents for GNSS/SBAS-related sections
- [ ] Direct-text extraction of LPV, APV, LNAV/VNAV, RNAV, and RNP section references
- [ ] Direct-text extraction of alert-limit and protection-level definitions as used in procedure design
- [ ] Direct-text extraction of any monitoring/assessment/reporting provisions
- [ ] Cross-check against [[Source - ICAO Annex 10 Volume I GNSS SBAS]] for SARPs/technical-provisions consistency
- [ ] Cross-check against [[Source - RTCA DO-229]] for equipment-procedure boundary alignment
