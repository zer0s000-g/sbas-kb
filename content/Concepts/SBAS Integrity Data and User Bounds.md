---
title: SBAS Integrity Data and User Bounds
description: Core concept note routing SBAS integrity-data and user-bound claims between corrections, protection levels, alert limits, and operational validation
tags: [sbas, integrity, protection-levels, alert-limits, receiver, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: reviewed
verification_status: source-routed-core-mechanism
---

# SBAS Integrity Data and User Bounds

## Purpose

This note explains the core routing boundary for integrity data and user-bounding language.

It does not publish equations, numerical thresholds, message fields, receiver algorithms, or operation-specific alert limits.

## Concept relationship

| Concept                      | Role                                             | Owner                                                                                 |
| ---------------------------- | ------------------------------------------------ | ------------------------------------------------------------------------------------- |
| corrections                  | reduce or model errors                           | [[SBAS Corrections and Integrity Separation]], [[SBAS Correction Timescale Taxonomy]] |
| integrity data               | supports bounding and usability decisions        | this note, with source routing                                                        |
| protection levels            | receiver/user-side bound concept                 | [[Protection Levels]]                                                                 |
| alert limits                 | operation/procedure usability threshold concept  | [[Alert Limits]]                                                                      |
| receiver mode / annunciation | cockpit/user presentation boundary               | [[SBAS Receiver Modes and Annunciation]]                                              |
| operational approval         | regulator/procedure/aircraft/operator validation | [[SBAS Operational Validation Dashboard]]                                             |

## Core rule

Integrity data must not be treated as merely another accuracy correction. It belongs to the safety/usability chain: the receiver must be able to determine whether the navigation solution should be used for the intended operation.

## Blocked claim patterns

Do not publish:

- numerical protection-level equations without direct source support;
- alert-limit values detached from operation and procedure context;
- receiver alert timing or annunciation details without MOPS/avionics evidence;
- statements that a correction source alone proves integrity;
- operational authorization from an integrity concept alone.

## Safe wording pattern

```text
The source supports integrity-bound routing at concept level. Detailed bounds, equations, alerting behavior, and operational use require direct standards, receiver, procedure, and approval evidence.
```

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Corrections and Integrity Separation]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Receiver Modes and Annunciation]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - RTCA DO-229]]

## See also

- [[SBAS Standards to Operations Evidence Ladder]]
- [[SBAS Service Performance Concepts]]
