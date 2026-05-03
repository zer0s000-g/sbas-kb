---
title: LNAV/VNAV Approach Procedure and SBAS Integration
description: Institutional learning page explaining Lateral Navigation / Vertical Navigation as a PBN-supported aviation operation, with explicit source and approval caveats
tags: [aviation, approach, lnav-vnav, sbas, pbn, integrity, procedure]
category: aviation-operations
created: 2026-04-19
modified: 2026-05-03
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# LNAV/VNAV Approach Procedure and SBAS Integration

## Scope and reader profile

This page explains LNAV/VNAV as a PBN-supported aviation concept and connects it to the integrity learning path. It is written for technical readers, researchers, aviation specialists, regulators, ANSP staff, and implementation teams who need a disciplined overview before consulting operational sources.

This page is not an approach chart, flight manual, regulator approval, avionics manual, or procedure-design standard. Do not use it to determine minima, aircraft eligibility, crew authorization, or whether a specific airport/runway supports LNAV/VNAV. Those determinations require official AIP/AIS data, procedure charts, regulator material, service-provider status, approved avionics documentation, and operator procedures.

## Executive summary

**LNAV/VNAV** means **Lateral Navigation / Vertical Navigation**. In this knowledge base, LNAV/VNAV is treated as a PBN-supported approach concept where lateral guidance is provided by RNAV or SBAS, and vertical guidance is provided by barometric VNAV or equivalent approved sources.

A simplified learning statement is:

```text
LNAV/VNAV is an approach procedure type where the aircraft must satisfy lateral-navigation and vertical-navigation integrity, procedure-design, equipment, and approval conditions.
```

The distinction between LNAV/VNAV and LPV is important: LNAV/VNAV vertical guidance may be advisory rather than final-approach-grade, depending on the procedure design, equipment certification, and regulator approval for the specific operation.

## What LNAV/VNAV depends on

An LNAV/VNAV operation depends on multiple layers working together:

| Layer                    | Required question                                                                            |
| ------------------------ | -------------------------------------------------------------------------------------------- |
| Navigation specification | Does the procedure meet the applicable PBN navigation specification (RNAV/RNP)?              |
| Receiver and avionics    | Is the aircraft equipped and approved for LNAV/VNAV mode?                                    |
| Procedure publication    | Is an LNAV/VNAV procedure published for the runway and current cycle?                        |
| Integrity checks         | Are the relevant [[Protection Levels]] acceptable against the relevant [[Alert Limits]]?     |
| Crew/operator approval   | Is the operator and crew authorized to conduct the operation?                                |
| Contingency logic        | Is the required response defined if service, receiver mode, or integrity conditions degrade? |

A technical navigation signal alone does not establish LNAV/VNAV operational availability.

## Relationship to SBAS integrity

LNAV/VNAV is useful for understanding how SBAS contributes to approach operations:

1. [[SBAS Architecture]] provides the monitoring, correction, broadcast, and receiver-processing chain.
2. [[SBAS Integrity]] explains why use-or-non-use logic is central.
3. [[Protection Levels]] express bounded-error concepts used in usability checks.
4. [[Alert Limits]] represent operation-specific acceptability thresholds.
5. The approved procedure and avionics determine how the pilot and aircraft use the guidance.

This page intentionally avoids giving unsourced numerical thresholds. Earlier draft values have been removed from the narrative until they can be tied to specific standards or approved operational sources.

## LNAV/VNAV compared with nearby concepts

| Concept | Relationship to LNAV/VNAV                                         | Important distinction                                        |
| ------- | ----------------------------------------------------------------- | ------------------------------------------------------------ |
| LPV     | LPV is also vertically guided; different integrity/approval basis | LPV requires SBAS for final-approach-grade vertical guidance |
| LNAV    | Lateral navigation approach concept                               | Does not provide vertical guidance                           |
| RNAV    | Area navigation family                                            | Broader than LNAV/VNAV; not itself an approach type          |
| RNP     | Performance-based navigation with onboard monitoring/alerting     | Related to PBN concepts but not equivalent to LNAV/VNAV      |
| GBAS    | Local-area augmentation approach context                          | Different augmentation architecture from SBAS                |

See [[LPV-Approach-Procedure]], [[RNAV-Approach-Procedure]], [[RNP-Approach-Procedure]], and [[GBAS-Approach-Procedure]] for nearby aviation notes.

## Operational interpretation

For a public knowledge base, the safest institutional phrasing is:

```text
LNAV/VNAV may provide vertical navigation guidance where the PBN navigation specification, aircraft equipment, procedure publication, operational approval, and real-time integrity conditions support it.
```

Avoid unsupported claims such as:

- universal LNAV/VNAV minima or decision heights;
- generic accuracy values detached from a standard or service definition;
- aircraft cost figures or benefit percentages without a sourced case study;
- pilot training hours without regulator/operator source support;
- regional LNAV/VNAV availability inferred only from SBAS coverage.

## Benefits to evaluate

LNAV/VNAV can be valuable because it may provide vertical guidance capability at airports where full LPV procedures are not yet published. However, the actual benefit depends on local and regional conditions:

- runway and airport network geometry;
- terrain and obstacle environment;
- weather and operational minima needs;
- aircraft equipage;
- procedure-design capacity;
- regulator/ANSP approval and oversight;
- SBAS or alternative navigation service status and performance;
- maintenance of AIS/AIM and charting processes.

For ASEAN implementation analysis, this connects LNAV/VNAV to [[ASEAN SBAS Operational Demand Drivers]], [[ASEAN SBAS Deployment Barriers]], and [[ASEAN SBAS Service-Model Options]].

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
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[GBAS-Approach-Procedure]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Source Backlog]]
