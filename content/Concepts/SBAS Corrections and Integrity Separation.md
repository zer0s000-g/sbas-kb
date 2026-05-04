---
title: SBAS Corrections and Integrity Separation
description: Core concept note separating SBAS accuracy-improvement corrections from integrity and use-or-non-use decision support
tags: [sbas, corrections, integrity, accuracy, safety, core]
created: 2026-05-03
modified: 2026-05-04
status: active
verification_status: source-routed-concept-no-numerical-claims
---

# SBAS Corrections and Integrity Separation

## Purpose

This note exists to prevent one of the most damaging SBAS documentation errors: treating correction as if it automatically proves integrity.

SBAS provides information that can improve positioning and information that supports integrity decisions. Those functions are connected, but they are not the same claim.

## Core distinction

| Function     | Question answered                                                                            | Safe statement                                                                                        |
| ------------ | -------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| Correction   | How can modeled navigation errors be reduced?                                                | Corrections can improve the estimated position when applicable and properly used                      |
| Integrity    | Can the user rely on the solution for this operation, and will unsafe conditions be alerted? | Integrity supports use-or-non-use decisions through bounded-error and alerting logic                  |
| Availability | Is the required service usable when needed?                                                  | Availability depends on service definition, geometry, monitoring, ionosphere, receiver, and operation |
| Continuity   | Will the required service remain usable through the operation?                               | Continuity is operation-context dependent and must be source-specific                                 |

Accuracy improvement is not sufficient for aviation operational use unless the solution is also bounded, monitored, and accepted by the applicable operational chain.

## Correction families

At concept level, SBAS corrections may address several GNSS error contributors, including satellite-related errors and ionospheric delay. Use [[SBAS Satellite Orbit and Clock Corrections]], [[SBAS Ionospheric Grid Correction Concept]], and [[SBAS Correction Timescale Taxonomy]] for mechanism/category routing. Exact categories, definitions, and applicability must be extracted from standards and service-provider documents before use in authoritative tables.

This note may say that corrections are part of the SBAS architecture. It must not say that a specific system, region, airport, aircraft, or procedure receives a particular correction unless the relevant source exists.

## Integrity families

Integrity-related SBAS information supports bounded-error and usability decisions. In this KB, the integrity chain is routed through:

```text
SBAS Integrity
  -> Protection Levels
  -> Alert Limits
  -> Operational validation / procedure / aircraft / operator evidence
```

This note does not own the details of protection-level equations, alert-limit values, cockpit annunciations, or procedure responses.

## Non-overlap map

| Topic                                    | Owned by                                  |
| ---------------------------------------- | ----------------------------------------- |
| Beginner explanation of why SBAS matters | [[What is SBAS]]                          |
| End-to-end architecture                  | [[SBAS Architecture]]                     |
| Signal/message chain                     | [[SBAS Signal and Message Flow]]          |
| Correction/integrity distinction         | this note                                 |
| Use-or-non-use logic                     | [[SBAS Integrity]]                        |
| Protection-bound concept                 | [[Protection Levels]]                     |
| Operation threshold concept              | [[Alert Limits]]                          |
| Operational authorization                | [[SBAS Operational Validation Dashboard]] |

## Blocked inferences

Do not infer:

- correction availability from coverage alone;
- integrity from accuracy alone;
- LPV availability from SBAS signal reception;
- aircraft eligibility from service-provider status;
- current procedure availability from standards or MOPS alone;
- regional readiness from another system’s published performance.

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-229]]
- [[Source - SBAS Service Providers]]
- [[SBAS Operational Validation Dashboard]]

## Implementation relevance

For ASEAN or any other regional implementation analysis, this separation matters because low-latitude ionospheric behavior can affect both correction quality and integrity bounding. Research notes can help identify threats, but they cannot be promoted into operational correction or integrity service logic without service-design and approval evidence.

## See also

- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[Total Electron Content (TEC)]]
- [[Ionospheric Model Validation]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[SBAS Satellite Orbit and Clock Corrections]]
- [[SBAS Ionospheric Grid Correction Concept]]
- [[SBAS Correction Timescale Taxonomy]]
- [[SBAS Integrity Data and User Bounds]]
