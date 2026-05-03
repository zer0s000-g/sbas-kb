---
title: RNAV Approach Procedure and SBAS Integration
description: Institutional learning page explaining Area Navigation as a PBN-supported aviation operation, with explicit source and approval caveats
tags: [aviation, approach, rnav, sbas, pbn, integrity, procedure]
category: aviation-operations
created: 2026-04-19
modified: 2026-05-03
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# RNAV Approach Procedure and SBAS Integration

## Scope and reader profile

This page explains RNAV as a PBN-supported aviation concept and connects it to the integrity learning path. It is written for technical readers, researchers, aviation specialists, regulators, ANSP staff, and implementation teams who need a disciplined overview before consulting operational sources.

This page is not an approach chart, flight manual, regulator approval, avionics manual, or procedure-design standard. Do not use it to determine minima, aircraft eligibility, crew authorization, or whether a specific airport/runway supports RNAV approaches. Those determinations require official AIP/AIS data, procedure charts, regulator material, service-provider status, approved avionics documentation, and operator procedures.

## Executive summary

**RNAV** means **Area Navigation**. In this knowledge base, RNAV is treated as the broad family of navigation concepts that permit aircraft to fly any desired flight path using a combination of onboard navigation sensors and external signals, rather than being constrained to fly directly to or from ground-based navaids.

A simplified learning statement is:

```text
RNAV is a navigation concept that enables flexible flight paths using onboard navigation; SBAS can serve as one of several possible augmentation sources for approved RNAV operations.
```

An RNAV approach is an instrument approach procedure designed using RNAV navigation specifications. It may use SBAS, GNSS, DME/DME, VOR/DME, or other approved sensors, depending on the applicable navigation specification.

## What RNAV depends on

An RNAV operation depends on multiple layers working together:

| Layer                    | Required question                                                                                             |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| Navigation specification | Does the procedure meet the applicable RNAV navigation specification (RNAV 10, RNAV 5, RNAV 2, RNAV 1, etc.)? |
| Receiver and avionics    | Is the aircraft equipped and approved for the required RNAV specification?                                    |
| Procedure publication    | Is an RNAV approach procedure published for the runway and current cycle?                                     |
| Integrity checks         | Are the relevant [[Protection Levels]] acceptable against the relevant [[Alert Limits]]?                      |
| Crew/operator approval   | Is the operator and crew authorized to conduct the operation?                                                 |
| Contingency logic        | Is the required response defined if service, receiver mode, or integrity conditions degrade?                  |

A technical SBAS signal alone does not establish RNAV operational availability. RNAV is a broader navigation family that includes SBAS-enabled modes but also includes non-SBAS sensor combinations.

## Relationship to SBAS integrity

SBAS contributes to RNAV by providing augmentation and integrity monitoring for GNSS-based RNAV operations:

1. [[SBAS Architecture]] provides the monitoring, correction, broadcast, and receiver-processing chain.
2. [[SBAS Integrity]] explains why use-or-non-use logic is central.
3. [[Protection Levels]] express bounded-error concepts used in usability checks.
4. [[Alert Limits]] represent operation-specific acceptability thresholds.
5. The approved procedure and avionics determine how the pilot and aircraft use the guidance.

This page intentionally avoids giving unsourced numerical thresholds. Earlier draft values have been removed from the narrative until they can be tied to specific standards or approved operational sources.

## RNAV compared with nearby concepts

| Concept   | Relationship to RNAV                                          | Important distinction                                             |
| --------- | ------------------------------------------------------------- | ----------------------------------------------------------------- |
| LPV       | LPV uses RNAV for lateral guidance plus SBAS for vertical     | LPV is a specific approach type, not a general navigation concept |
| LNAV/VNAV | Uses RNAV for lateral guidance plus VNAV for vertical         | Vertical source and approval logic may differ                     |
| RNP       | RNP extends RNAV with onboard performance monitoring/alerting | RNP requires onboard monitoring; RNAV may not                     |
| SBAS      | SBAS can serve as an augmentation source for RNAV             | SBAS is a system; RNAV is a navigation concept                    |
| GBAS      | GBAS provides local augmentation for precision approaches     | Different augmentation architecture from SBAS                     |

See [[LPV-Approach-Procedure]], [[LNAV-VNAV-Approach-Procedure]], [[RNP-Approach-Procedure]], and [[GBAS-Approach-Procedure]] for nearby aviation notes.

## Operational interpretation

For a public knowledge base, the safest institutional phrasing is:

```text
RNAV may provide flexible flight-path capability where the navigation specification, aircraft equipment, procedure publication, operational approval, and real-time integrity conditions support it.
```

Avoid unsupported claims such as:

- universal RNAV minima or decision heights;
- generic accuracy values detached from a standard or service definition;
- aircraft cost figures or benefit percentages without a sourced case study;
- pilot training hours without regulator/operator source support;
- regional RNAV availability inferred only from SBAS coverage.

## Benefits to evaluate

RNAV can be valuable because it enables more flexible and efficient flight paths compared to conventional ground-based navigation. However, the actual benefit depends on local and regional conditions:

- airspace design and route structure;
- terrain and obstacle environment;
- aircraft equipage;
- procedure-design capacity;
- regulator/ANSP approval and oversight;
- navigation service status and performance;
- maintenance of AIS/AIM and charting processes.

For ASEAN implementation analysis, this connects RNAV to [[ASEAN SBAS Operational Demand Drivers]], [[ASEAN SBAS Deployment Barriers]], and [[ASEAN SBAS Service-Model Options]].

## Source anchors and current maturity

Current source scaffolds relevant to this page include:

- [[SBAS Standards Source Matrix]] -- current claim-routing matrix for standards/source families.
- [[Source - RTCA DO-229]] -- current GPS/SBAS airborne-equipment source-family anchor; supports equipment routing, not procedure-design or operational approval.
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] -- ICAO procedure-design and PBN navigation specification source family.
- [[Source - FAA and EASA Procedure-Design and PBN Material]] -- FAA TERPS / PBN orders and EASA AMC/GM material.
- [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]] -- regulator/article-approval routing.
- [[SBAS Source Backlog]] -- active standards-source verification queue.

This page is now `source-scaffold-linked`. It is a learning and navigation page, not a verified operational requirements table.

## Replaced draft material

This page previously contained unsourced numerical performance values (accuracy figures, alert limits, detection times, decision heights, weather minima, wind limits, fuel savings percentages, cost figures, and pilot-training hours). Those have been removed from the main narrative because they were not tied to visible source anchors. Future values may be reintroduced only when each value is linked to a source, context, jurisdiction, procedure type, and revision/date.

## See also

- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[GBAS-Approach-Procedure]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Source Backlog]]
