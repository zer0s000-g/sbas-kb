---
title: SBAS Ranging Sources and Time Reference
description: Core concept note separating GNSS ranging, SBAS GEO ranging or broadcast support, and time-reference claims without operational overclaiming
tags: [sbas, gnss, ranging, time, architecture, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: reviewed
verification_status: source-routed-core-mechanism
---

# SBAS Ranging Sources and Time Reference

## Purpose

This note explains where SBAS ranging-source and time-reference claims belong in the knowledge base.

It is a **core mechanism routing note**, not a message specification, timing-accuracy table, or receiver-approval statement.

## Non-overlap rule

This note owns only the conceptual separation among:

- GNSS constellation ranging signals;
- SBAS broadcast support;
- any source-supported SBAS GEO ranging or ranging-like role;
- time-reference alignment as a standards/service concept;
- receiver use of these inputs.

It does not own:

- message contents — use [[SBAS Signal and Message Flow]];
- correction categories — use [[SBAS Correction Timescale Taxonomy]];
- integrity/useability bounds — use [[SBAS Integrity Data and User Bounds]];
- receiver modes — use [[SBAS Receiver Modes and Annunciation]];
- operational use — use [[SBAS Standards to Operations Evidence Ladder]].

## Conceptual layers

| Layer               | Safe concept-level statement                                                                                            | Evidence family before detail                                           |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| GNSS ranging source | The user receiver derives measurements from GNSS signals according to its supported constellations and receiver design  | GNSS standards and receiver/equipment evidence                          |
| SBAS broadcast path | SBAS information is broadcast to users through SBAS signal channels described by the relevant source family             | Annex 10 / DO-229 / service-provider source notes                       |
| SBAS GEO role       | Some sources may describe SBAS GEO broadcast and, where supported by the standards/service context, ranging-related use | direct standards/service evidence before system-specific statements     |
| Time reference      | Time alignment is part of the navigation/correction problem                                                             | Annex 10 / DO-229 / service-definition evidence before numerical claims |
| Receiver use        | The airborne/user receiver combines measurements and SBAS data according to its approval basis                          | receiver standards, avionics, aircraft, and operator evidence           |

## Blocked claim patterns

Do not infer:

- that SBAS broadcast reception proves a receiver may use it for a procedure;
- that a GEO broadcast path always creates an operational ranging source;
- that a generic time-reference statement proves a numerical timing tolerance;
- that service-provider architecture proves aircraft or operator authorization;
- that one SBAS system's signal role applies to another system without source-specific support.

## Safe wording pattern

```text
The source supports a concept-level statement about ranging or time-reference context within its own scope. It does not by itself establish receiver approval, procedure availability, or operational authorization.
```

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Architecture]]
- [[SBAS Signal and Message Flow]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - RTCA DO-229]]
- [[Source - SBAS Service Providers]]

## See also

- [[SBAS Correction Timescale Taxonomy]]
- [[SBAS Service Performance Concepts]]
- [[SBAS Standards to Operations Evidence Ladder]]
