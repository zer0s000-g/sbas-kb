---
title: Source - FAA and EASA Procedure-Design and PBN Material
description: Institutional source-family anchor for FAA TERPS / PBN orders and EASA AMC/GM / Easy Access Rules related to instrument procedure design and PBN operations, with explicit boundaries
tags: [source, faa, easa, terps, pbn, procedure-design, order-8260, amc-gm, operational-approval]
source_type: regulator-material
status: active
verification_status: public-catalog-reviewed-not-source-extracted
---

# Source - FAA and EASA Procedure-Design and PBN Material

## Scope of this note

This note is the knowledge base's institutional source-family anchor for FAA and EASA material related to instrument procedure design and PBN operational criteria.

It exists to keep procedure-design, operational-approval, and aircraft-installation claims separated from:

- airborne-equipment MOPS (handled by [[Source - RTCA DO-229]]);
- article/equipment approval (handled by [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]]);
- ICAO PANS-OPS / PBN Manual family (handled by [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]]);
- service-provider commitment (covered by future service-provider source notes).

This note does **not** provide procedure minima, airport-specific decision heights, fleet-equipage rates, operational-approval checklists, or crew-training hour requirements. Those require the official FAA/EASA documents, AIPs, operator manuals, and regulator approvals.

Important boundary:

- Public FAA and EASA catalog metadata can support document identity, purpose, and current-edition signals.
- It cannot support numerical design tolerances, exact minima, or operational-approval decisions.
- Use this note for regulator-level procedure-design routing and to keep national approval claims separate from equipment and service claims.

## FAA source identity signals (public catalog)

### FAA Order 8260.3G — TERPS

| Field                | Current public signal                                                                                                                                                                                            |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Issuing body         | FAA, Office of Primary Responsibility AFS-400                                                                                                                                                                    |
| Document             | Order 8260.3G                                                                                                                                                                                                    |
| Full title           | United States Standard for Terminal Instrument Procedures (TERPS)                                                                                                                                                |
| Date issued          | 2024-07-01                                                                                                                                                                                                       |
| Status               | Active                                                                                                                                                                                                           |
| Purpose signal       | "Prescribes standardized methods for design and evaluation of IFPs prescribed under Title 14, Code of Federal Regulations (14 CFR) part 97 as well as other IFPs and ATC procedures not specified under part 97" |
| Applicability signal | Pertinent to 14 CFR parts 1, 71, 77, 91, 95, 97, 121, 125, 129, 135 and 171                                                                                                                                      |

### FAA Order 8260.58D — PBN Instrument Procedure Design

| Field                | Current public signal                                                                                                                                                                                                           |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Issuing body         | FAA, Office of Primary Responsibility AFS-400                                                                                                                                                                                   |
| Document             | Order 8260.58D                                                                                                                                                                                                                  |
| Full title           | United States Standard for Performance Based Navigation (PBN) Instrument Procedure Design                                                                                                                                       |
| Date issued          | 2025-01-15                                                                                                                                                                                                                      |
| Status               | Active                                                                                                                                                                                                                          |
| Purpose signal       | "Provides guidance for the design and evaluation of Performance Based Navigation (PBN) Instrument Flight Procedures (IFPs)"                                                                                                     |
| Scope signal         | PBN IFPs are those based on Area Navigation (RNAV) or Required Navigation Performance (RNP), including transitions to an Instrument Landing System (ILS) or Ground Based Augmentation (GBAS) Landing System (GLS) final segment |
| Applicability signal | Pertinent to 14 CFR part 95 and 97                                                                                                                                                                                              |

## EASA source identity signals (public catalog)

### EASA Easy Access Rules for ATM/ANS Equipment (November 2024)

| Field            | Current public signal                                                                                                                                  |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Issuing body     | EASA                                                                                                                                                   |
| Document         | Easy Access Rules for ATM/ANS Equipment                                                                                                                |
| Legal basis      | Commission Implementing Regulation (EU) 2023/1769 and Commission Delegated Regulation (EU) 2023/1768                                                   |
| Publication date | 25 November 2024                                                                                                                                       |
| Formats          | PDF and XML                                                                                                                                            |
| Scope signal     | Certification and declaration of ATM/ANS systems and constituents; approval of organisations involved in design or production; AMC and GM to the above |

### EASA PBN Operations Transition Material

| Field        | Current public signal                                                                                                                                                                                                |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Issuing body | EASA                                                                                                                                                                                                                 |
| Domain       | Transition to performance-based navigation (PBN) operations                                                                                                                                                          |
| Scope signal | Identifies navigation specifications and functionalities to be used for en-route ATS routes, standard instrument departure routes (SID), standard terminal arrival routes (STAR), and instrument approach procedures |
| Note         | EASA AMC/GM and Acceptable Means of Compliance material exist for PBN operational approval, including approach procedures predicated on PBN                                                                          |

## What this source-family can currently anchor

Until direct extraction from the official FAA/EASA procedure-design and PBN material is performed, this note can support broad routing statements such as:

- FAA Order 8260.3G (TERPS) is the current U.S. standard for terminal instrument procedure design.
- FAA Order 8260.58D is the current U.S. standard for PBN instrument procedure design.
- EASA AMC/GM and Easy Access Rules provide European PBN operational-approval and ATM/ANS equipment certification material.
- National procedure-design criteria and operational approvals are jurisdiction-specific and must not be treated as portable without explicit equivalence evidence.
- Equipment MOPS and article approval do not, by themselves, establish that a published procedure exists, that an operator is approved, or that a particular crew/aircraft combination may conduct the operation.

## What this source-family must not be used for yet

Do not use this note alone to publish:

- exact U.S. TERPS design tolerances or obstacle-clearance values;
- exact FAA PBN transition criteria or procedure-design calculations;
- exact EASA AMC/GM operational-approval requirements extracted in detail;
- airport-specific approach availability or minima;
- any claim that FAA and EASA requirements are equivalent without direct comparison evidence;
- training-hour, simulator-session, or operator-manual requirements asserted as standard.

## Relationship to other source notes in this knowledge base

| National regulator | Procedure-design order       | PBN order/material       | Operational-approval AMC/GM     | Article approval                            |
| ------------------ | ---------------------------- | ------------------------ | ------------------------------- | ------------------------------------------- |
| FAA                | Order 8260.3G (TERPS)        | Order 8260.58D           | ACs, OpSpecs, operator-specific | [[Source - FAA TSO-C145e and TSO-C146e]]    |
| EASA               | National SERA / AIP material | AMC/GM to Part-ARO / AUR | AMC/GM; Easy Access Rules       | [[Source - EASA ETSO-C145e and ETSO-C146e]] |
| ICAO               | Doc 8168 Vol II              | Doc 9613                 | Doc 9613; SARPs in Annexes      | — (TSO/ETSO is national)                    |

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
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]]

## Extraction template for future direct-source cycles

### FAA Order 8260.3G required

- [ ] Direct-text extraction of Table of Contents and GNSS/SBAS/APV/LPV-relevant sections
- [ ] Direct-text extraction of alert-limit and protection-level references as used in procedure design
- [ ] Cross-check against [[Source - RTCA DO-229]] for equipment-procedure boundary alignment

### FAA Order 8260.58D required

- [ ] Direct-text extraction of RNAV and RNP procedure-design criteria
- [ ] Direct-text extraction of GBAS/GLS transition material
- [ ] Cross-check against Doc 9613 navigation specifications

### EASA AMC/GM required

- [ ] Identification of exact AMC/GM document numbers and editions for PBN operational approval
- [ ] Direct-text extraction of approach-procedure predication on PBN
- [ ] Cross-check against EASA ETSO and Easy Access Rules for equipment-procedure boundary alignment
