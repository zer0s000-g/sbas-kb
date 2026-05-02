---
title: LPV Approach Procedure and SBAS Integration
description: Institutional learning page explaining Localizer Performance with Vertical guidance as an SBAS-supported aviation operation, with explicit source and approval caveats
tags: [aviation, approach, lpv, sbas, integrity, procedure]
category: aviation-operations
created: 2026-04-19
modified: 2026-05-02
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# LPV Approach Procedure and SBAS Integration

## Scope and reader profile

This page explains LPV as an SBAS-supported aviation concept and connects it to the integrity learning path. It is written for technical readers, researchers, aviation specialists, regulators, ANSP staff, and implementation teams who need a disciplined overview before consulting operational sources.

This page is not an approach chart, flight manual, regulator approval, avionics manual, or procedure-design standard. Do not use it to determine minima, aircraft eligibility, crew authorization, or whether a specific airport/runway supports LPV. Those determinations require official AIP/AIS data, procedure charts, regulator material, service-provider status, approved avionics documentation, and operator procedures.

## Executive summary

**LPV** means **Localizer Performance with Vertical guidance**. In this knowledge base, LPV is treated as the clearest aviation example of why SBAS integrity matters: the operation depends not merely on improved GNSS accuracy, but on bounded-error information, alerting, approved receiver behavior, published procedure design, and operational authorization.

A simplified learning statement is:

```text
LPV is an SBAS-enabled vertically guided approach concept where the receiver and operation must satisfy integrity, availability, procedure, equipment, and approval conditions.
```

## What LPV depends on

An LPV operation depends on multiple layers working together:

| Layer                  | Required question                                                                            |
| ---------------------- | -------------------------------------------------------------------------------------------- |
| SBAS service           | Is an approved SBAS service available and suitable for the operation?                        |
| Receiver and avionics  | Is the aircraft equipped and approved for the required mode?                                 |
| Procedure publication  | Is an LPV procedure published for the runway and current cycle?                              |
| Integrity checks       | Are the relevant [[Protection Levels]] acceptable against the relevant [[Alert Limits]]?     |
| Crew/operator approval | Is the operator and crew authorized to conduct the operation?                                |
| Contingency logic      | Is the required response defined if service, receiver mode, or integrity conditions degrade? |

A technical SBAS signal alone does not establish LPV operational availability.

## Relationship to SBAS integrity

LPV is a useful training case because it makes the integrity chain concrete:

1. [[SBAS Architecture]] provides the monitoring, correction, broadcast, and receiver-processing chain.
2. [[SBAS Integrity]] explains why use-or-non-use logic is central.
3. [[Protection Levels]] express bounded-error concepts used in usability checks.
4. [[Alert Limits]] represent operation-specific acceptability thresholds.
5. The approved procedure and avionics determine how the pilot and aircraft use the guidance.

This page intentionally avoids giving unsourced numerical thresholds. Earlier draft values have been removed from the authoritative narrative until they can be tied to specific standards or approved operational sources.

## LPV compared with nearby concepts

| Concept       | Relationship to LPV                                                        | Important distinction                                            |
| ------------- | -------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| LNAV          | Lateral navigation approach concept                                        | Does not imply the same vertical-guidance basis as LPV           |
| LNAV/VNAV     | Lateral plus vertical navigation concept                                   | May use different vertical-navigation sources and approval logic |
| RNAV          | Area navigation family                                                     | Broader than LPV; not itself an SBAS mode                        |
| RNP           | Performance-based navigation with onboard monitoring/alerting requirements | Related to PBN concepts but not equivalent to LPV                |
| GBAS approach | Local-area augmentation approach context                                   | Different augmentation architecture from SBAS                    |

See [[LNAV-VNAV-Approach-Procedure]], [[RNAV-Approach-Procedure]], [[RNP-Approach-Procedure]], and [[GBAS-Approach-Procedure]] for nearby aviation notes.

## Operational interpretation

For a public knowledge base, the safest institutional phrasing is:

```text
LPV may provide vertically guided approach capability where the SBAS service, aircraft equipment, procedure publication, operational approval, and real-time integrity conditions support it.
```

Avoid unsupported claims such as:

- universal LPV minima;
- universal decision heights;
- generic accuracy values detached from a standard or service definition;
- airport cost savings without a sourced case study;
- regional LPV availability inferred only from SBAS coverage;
- training-hour requirements without regulator/operator source support.

## Benefits to evaluate

LPV can be valuable because it may support vertically guided access without installing a traditional precision-approach ground system at every runway. However, the actual benefit depends on local and regional conditions:

- runway and airport network geometry;
- terrain and obstacle environment;
- weather and operational minima needs;
- aircraft equipage;
- procedure-design capacity;
- regulator/ANSP approval and oversight;
- SBAS service status and performance;
- maintenance of AIS/AIM and charting processes.

For ASEAN implementation analysis, this connects LPV to [[ASEAN SBAS Operational Demand Drivers]], [[ASEAN SBAS Deployment Barriers]], and [[ASEAN SBAS Service-Model Options]].

## Source anchors and current maturity

Current source scaffolds relevant to this page include:

- [[SBAS Standards Source Matrix]] — current claim-routing matrix for standards/source families.
- [[Source - RTCA DO-229]] — current GPS/SBAS airborne-equipment source-family anchor.
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]] — current ICAO SARPs/technical-provisions source-family routing anchor for GNSS/SBAS.
- [[Source - ICAO Doc 9849]] — current ICAO GNSS implementation-guidance source-family anchor.
- [[Source - RTCA DO-242]], [[Source - RTCA DO-289]], [[Source - ICAO Doc 9854]], and [[Source - ICAO Doc 9855]] — red-flag provenance notes retained because earlier drafts likely mis-scoped them for SBAS.
- [[SBAS Source Backlog]] — active standards-source verification queue.

This page is now `source-scaffold-linked`. It is a high-quality learning and navigation page, not a verified operational requirements table.

## Implementation checklist for research use

For research or planning, evaluate LPV through the following questions:

1. What official source confirms SBAS service status for the relevant region?
2. What AIP/AIS/procedure source confirms the actual LPV procedure inventory?
3. What aircraft equipage assumptions are being made?
4. What regulator or ANSP material defines approval and oversight?
5. What integrity, protection-level, and alert-limit sources apply?
6. What outage, downgrade, or missed-approach procedures are specified in approved material?
7. What local operational problem is LPV intended to solve?

## Replaced draft material

This page previously contained unsourced numerical performance values, generic weather minima, pilot-training hours, cost figures, and benefit percentages. Those have been removed from the main narrative because they were not tied to visible source anchors. Future values may be reintroduced only when each value is linked to a source, context, jurisdiction, procedure type, and revision/date.

## Open verification tasks

1. Build a verified source note for LPV procedure and approval terminology.
2. Identify which claims belong to airborne-equipment standards versus procedure-design or regulator material.
3. Add source-backed LPV examples from official AIP/AIS or regulator/ANSP pages.
4. Separate LPV conceptual explanation from region-specific implementation claims.
5. Connect verified LPV material back to [[SBAS in Civil Aviation MOC]], [[SBAS-Standards-Regulation]], and the Annex 10 / DO-229 / procedure-design source split.

## See also

- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[What is SBAS]]
- [[SBAS Source Backlog]]
