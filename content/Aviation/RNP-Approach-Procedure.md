---
title: RNP Approach Procedure and SBAS Integration
description: Institutional learning page explaining Required Navigation Performance as a PBN-supported aviation operation, with explicit source and approval caveats
tags: [aviation, approach, rnp, sbas, pbn, integrity, procedure]
category: aviation-operations
created: 2026-04-19
modified: 2026-05-03
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# RNP Approach Procedure and SBAS Integration

## Scope and reader profile

This page explains RNP as a PBN-supported aviation concept and connects it to the integrity learning path. It is written for technical readers, researchers, aviation specialists, regulators, ANSP staff, and implementation teams who need a disciplined overview before consulting operational sources.

This page is not an approach chart, flight manual, regulator approval, avionics manual, or procedure-design standard. Do not use it to determine minima, aircraft eligibility, crew authorization, or whether a specific airport/runway supports RNP approaches. Those determinations require official AIP/AIS data, procedure charts, regulator material, service-provider status, approved avionics documentation, and operator procedures.

## Executive summary

**RNP** means **Required Navigation Performance**. In this knowledge base, RNP is treated as a performance-based navigation specification that extends RNAV by requiring onboard performance monitoring and alerting capability. RNP specifications are defined in ICAO Doc 9613 and related PBN material.

A simplified learning statement is:

```text
RNP is a navigation specification requiring onboard performance monitoring and alerting; SBAS can serve as one of several possible augmentation sources for approved RNP operations.
```

RNP approach procedures are designed using PBN navigation specifications that incorporate self-contained onboard monitoring. If the aircraft determines it cannot maintain the required performance, it must alert the crew.

## What RNP depends on

An RNP operation depends on multiple layers working together:

| Layer                    | Required question                                                                                                       |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------- |
| Navigation specification | Does the procedure meet the applicable RNP navigation specification (RNP 4, RNP 2, RNP 1, RNP APCH, RNP AR APCH, etc.)? |
| Receiver and avionics    | Is the aircraft equipped and approved for the required RNP specification, including onboard monitoring/alerting?        |
| Procedure publication    | Is an RNP approach procedure published for the runway and current cycle?                                                |
| Integrity checks         | Are the relevant [[Protection Levels]] acceptable against the relevant [[Alert Limits]]?                                |
| Crew/operator approval   | Is the operator and crew authorized for the specific RNP specification?                                                 |
| Contingency logic        | Is the required response defined if performance monitoring alerts or integrity conditions degrade?                      |

A technical SBAS signal alone does not establish RNP operational availability. RNP operations require the aircraft to actively monitor and alert on navigation performance.

## Relationship to SBAS integrity

SBAS contributes to RNP by providing augmentation and integrity monitoring for GNSS-based RNP operations:

1. [[SBAS Architecture]] provides the monitoring, correction, broadcast, and receiver-processing chain.
2. [[SBAS Integrity]] explains why use-or-non-use logic is central.
3. [[Protection Levels]] express bounded-error concepts used in usability checks.
4. [[Alert Limits]] represent operation-specific acceptability thresholds.
5. The approved procedure and avionics determine how the pilot and aircraft use the guidance.

This page intentionally avoids giving unsourced numerical thresholds. Earlier draft values have been removed from the narrative until they can be tied to specific standards or approved operational sources.

## RNP compared with nearby concepts

| Concept   | Relationship to RNP                                       | Important distinction                                              |
| --------- | --------------------------------------------------------- | ------------------------------------------------------------------ |
| RNAV      | RNP extends RNAV with onboard monitoring/alerting         | RNAV does not require onboard performance monitoring               |
| LPV       | LPV uses SBAS for vertical guidance with integrity        | LPV is a specific approach type; RNP is a navigation specification |
| LNAV/VNAV | LNAV/VNAV uses lateral and vertical navigation            | LNAV/VNAV vertical source and approval logic may differ            |
| SBAS      | SBAS can serve as an augmentation source for RNP          | SBAS is a system; RNP is a navigation specification                |
| GBAS      | GBAS provides local augmentation for precision approaches | Different augmentation architecture from SBAS                      |

See [[LPV-Approach-Procedure]], [[LNAV-VNAV-Approach-Procedure]], [[RNAV-Approach-Procedure]], and [[GBAS-Approach-Procedure]] for nearby aviation notes.

## Operational interpretation

For a public knowledge base, the safest institutional phrasing is:

```text
RNP may provide performance-based navigation capability where the navigation specification, aircraft equipment with onboard monitoring/alerting, procedure publication, operational approval, and real-time integrity conditions support it.
```

Avoid unsupported claims such as:

- universal RNP minima or decision heights;
- generic accuracy values detached from a standard or service definition;
- aircraft cost figures or benefit percentages without a sourced case study;
- pilot training hours without regulator/operator source support;
- regional RNP availability inferred only from SBAS coverage.

## Benefits to evaluate

RNP can be valuable because it enables precise curved flight paths with integrity monitoring, particularly valuable in congested airspace and complex terrain. However, the actual benefit depends on local and regional conditions:

- airspace design and route structure;
- terrain and obstacle environment;
- aircraft equipage and onboard monitoring capability;
- procedure-design capacity;
- regulator/ANSP approval and oversight;
- navigation service status and performance;
- maintenance of AIS/AIM and charting processes.

For ASEAN implementation analysis, this connects RNP to [[ASEAN SBAS Operational Demand Drivers]], [[ASEAN SBAS Deployment Barriers]], and [[ASEAN SBAS Service-Model Options]].

## Source anchors and current maturity

Current source scaffolds relevant to this page include:

- [[SBAS Standards Source Matrix]] -- current claim-routing matrix for standards/source families.
- [[Source - RTCA DO-229]] -- current GPS/SBAS airborne-equipment source-family anchor; supports equipment routing, not procedure-design or operational approval.
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] -- ICAO procedure-design and PBN navigation specification source family; Doc 9613 defines RNP specifications.
- [[Source - FAA and EASA Procedure-Design and PBN Material]] -- FAA TERPS / PBN orders and EASA AMC/GM material.
- [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]] -- regulator/article-approval routing.
- [[SBAS Source Backlog]] -- active standards-source verification queue.

This page is now `source-scaffold-linked`. It is a learning and navigation page, not a verified operational requirements table.

## Replaced draft material

This page previously contained unsourced numerical performance values (accuracy figures, alert limits, detection times, decision heights, weather minima, wind limits, fuel savings percentages, cost figures, and pilot-training hours). Those have been removed from the main narrative because they were not tied to visible source anchors. Future values may be reintroduced only when each value is linked to a source, context, jurisdiction, procedure type, and revision/date.

## See also

- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[GBAS-Approach-Procedure]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Source Backlog]]
