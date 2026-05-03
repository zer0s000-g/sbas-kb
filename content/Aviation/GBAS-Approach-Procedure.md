---
title: GBAS Approach Procedure and SBAS Integration
description: Institutional learning page explaining Ground-Based Augmentation System approaches as a local-area augmentation concept, with explicit source and approval caveats
tags: [aviation, approach, gbas, gls, sbas, integrity, procedure]
category: aviation-operations
created: 2026-04-19
modified: 2026-05-03
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# GBAS Approach Procedure and SBAS Integration

## Scope and reader profile

This page explains GBAS as a local-area augmentation approach concept and connects it to the integrity learning path. It is written for technical readers, researchers, aviation specialists, regulators, ANSP staff, and implementation teams who need a disciplined overview before consulting operational sources.

This page is not an approach chart, flight manual, regulator approval, avionics manual, or procedure-design standard. Do not use it to determine minima, aircraft eligibility, crew authorization, or whether a specific airport/runway supports GBAS approaches. Those determinations require official AIP/AIS data, procedure charts, regulator material, service-provider status, approved avionics documentation, and operator procedures.

## Executive summary

**GBAS** means **Ground-Based Augmentation System**. In this knowledge base, GBAS is treated as a local-area GNSS augmentation concept that provides precision approach capability at a specific airport. GBAS is architecturally different from SBAS: it uses ground reference stations and data links local to the airport rather than wide-area GEO broadcast.

A simplified learning statement is:

```text
GBAS is a local-area augmentation system that supports precision approach procedures at equipped airports, subject to ground infrastructure, aircraft equipment, procedure publication, and operational approval.
```

GBAS approach procedures (sometimes called GLS procedures) use GBAS corrections to achieve precision approach accuracy. GBAS is typically discussed alongside SBAS because both augment GNSS, but they use fundamentally different architectures and have different service-delivery models.

## What GBAS depends on

A GBAS operation depends on multiple layers working together:

| Layer                  | Required question                                                                        |
| ---------------------- | ---------------------------------------------------------------------------------------- |
| Ground infrastructure  | Is the GBAS ground station installed, operational, and certified for the airport?        |
| Receiver and avionics  | Is the aircraft equipped and approved for GBAS/GLS approach mode?                        |
| Procedure publication  | Is a GBAS/GLS procedure published for the runway and current cycle?                      |
| Integrity checks       | Are the relevant [[Protection Levels]] acceptable against the relevant [[Alert Limits]]? |
| Crew/operator approval | Is the operator and crew authorized to conduct the operation?                            |
| Contingency logic      | Is the required response defined if GBAS service or integrity conditions degrade?        |

A technical GBAS signal alone does not establish GBAS operational availability. Unlike SBAS, GBAS requires dedicated local ground infrastructure at each equipped airport.

## Relationship to SBAS and integrity

GBAS is relevant to the SBAS knowledge base because it is a complementary augmentation concept that shares integrity principles:

1. [[SBAS Architecture]] describes the wide-area augmentation approach; GBAS uses a local-area architecture.
2. [[SBAS Integrity]] explains bounded-error principles that apply to both SBAS and GBAS.
3. [[Protection Levels]] express bounded-error concepts used in usability checks for both systems.
4. [[Alert Limits]] represent operation-specific acceptability thresholds applicable to both systems.
5. The approved procedure and avionics determine how the pilot and aircraft use GBAS guidance.

This page intentionally avoids giving unsourced numerical thresholds. Earlier draft values have been removed from the narrative until they can be tied to specific standards or approved operational sources.

## GBAS compared with nearby concepts

| Concept   | Relationship to GBAS                         | Important distinction                                               |
| --------- | -------------------------------------------- | ------------------------------------------------------------------- |
| SBAS      | Both augment GNSS; different architectures   | SBAS uses wide-area GEO broadcast; GBAS uses local ground stations  |
| LPV       | LPV is an SBAS-enabled approach type         | LPV does not require local ground infrastructure                    |
| LNAV/VNAV | Both may provide vertical guidance           | Different augmentation basis and approval logic                     |
| RNAV      | GBAS approaches use RNAV navigation concepts | GBAS provides local augmentation rather than area navigation        |
| RNP       | Both may support precision approaches        | RNP requires onboard monitoring; GBAS relies on ground augmentation |

See [[LPV-Approach-Procedure]], [[LNAV-VNAV-Approach-Procedure]], [[RNAV-Approach-Procedure]], and [[RNP-Approach-Procedure]] for nearby aviation notes.

## Operational interpretation

For a public knowledge base, the safest institutional phrasing is:

```text
GBAS may provide precision approach capability where the local ground infrastructure, aircraft equipment, procedure publication, operational approval, and real-time integrity conditions support it.
```

Avoid unsupported claims such as:

- universal GBAS minima or decision heights;
- generic accuracy values detached from a standard or service definition;
- aircraft cost figures or benefit percentages without a sourced case study;
- pilot training hours without regulator/operator source support;
- regional GBAS availability inferred only from airport infrastructure lists.

## Benefits to evaluate

GBAS can be valuable because it may provide precision approach capability without installing a traditional ILS at every runway. However, the actual benefit depends on local and regional conditions:

- airport infrastructure and GBAS ground station availability;
- terrain and obstacle environment;
- weather and operational minima needs;
- aircraft equipage;
- procedure-design capacity;
- regulator/ANSP approval and oversight;
- ground station maintenance and certification;
- maintenance of AIS/AIM and charting processes.

For ASEAN implementation analysis, this connects GBAS to [[ASEAN SBAS Operational Demand Drivers]], [[ASEAN SBAS Deployment Barriers]], and [[ASEAN SBAS Service-Model Options]].

## Source anchors and current maturity

Current source scaffolds relevant to this page include:

- [[SBAS Standards Source Matrix]] -- current claim-routing matrix for standards/source families.
- [[Source - RTCA DO-229]] -- current GPS/SBAS airborne-equipment source-family anchor; supports equipment routing, not procedure-design or operational approval.
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] -- ICAO procedure-design and PBN navigation specification source family.
- [[Source - FAA and EASA Procedure-Design and PBN Material]] -- FAA TERPS / PBN orders and EASA AMC/GM material.
- [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]] -- regulator/article-approval routing.
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]] -- ICAO SARPs/technical-provisions source-family anchor for GNSS/SBAS, including GBAS provisions.
- [[SBAS Source Backlog]] -- active standards-source verification queue.

This page is now `source-scaffold-linked`. It is a learning and navigation page, not a verified operational requirements table.

## Replaced draft material

This page previously contained unsourced numerical performance values (accuracy figures, alert limits, detection times, decision heights, weather minima, wind limits, fuel savings percentages, cost figures, and pilot-training hours), as well as corrupted wikilinks. Those have been removed or repaired. Future values may be reintroduced only when each value is linked to a source, context, jurisdiction, procedure type, and revision/date.

## See also

- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Source Backlog]]
