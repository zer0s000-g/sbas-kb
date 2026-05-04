---
title: SBAS Satellite Orbit and Clock Corrections
description: Core concept note routing SBAS satellite orbit and clock correction claims without duplicating standards text or service-provider details
tags: [sbas, corrections, orbit, clock, gnss, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: reviewed
verification_status: source-routed-core-mechanism
---

# SBAS Satellite Orbit and Clock Corrections

## Purpose

This note owns the concept-level boundary for SBAS satellite orbit and clock correction claims.

It does not publish correction equations, message numbers, accuracy budgets, update intervals, or provider-specific performance commitments.

## Non-overlap rule

Use this note for the **type of correction problem**. Use other notes for adjacent claims:

| Adjacent topic                       | Owner                                               |
| ------------------------------------ | --------------------------------------------------- |
| message path                         | [[SBAS Signal and Message Flow]]                    |
| correction timing categories         | [[SBAS Correction Timescale Taxonomy]]              |
| correction versus integrity boundary | [[SBAS Corrections and Integrity Separation]]       |
| service performance commitments      | [[SBAS Service Performance Concepts]]               |
| provider-specific evidence           | [[Source - SBAS Service Providers]] and child notes |
| receiver behavior                    | [[SBAS Receiver Modes and Annunciation]]            |

## Concept boundary

At concept level, orbit and clock correction language may state only that SBAS can support user positioning by providing information related to satellite orbit/clock error handling, subject to the standards and service definition.

Do not expand this into:

- exact message structures;
- numerical correction magnitudes;
- update rates;
- validity periods;
- detailed algorithms;
- aircraft approval;
- procedure availability.

## Why this distinction matters

Orbit and clock corrections may improve the user's navigation solution, but they do not by themselves prove integrity or operation suitability. Integrity needs bounded-error and alerting context, and operational use needs the full standards-to-operations evidence ladder.

## Safe wording pattern

```text
The source supports concept-level orbit/clock correction routing. It does not by itself establish integrity, receiver approval, procedure publication, or operational use.
```

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Correction Timescale Taxonomy]]
- [[SBAS Signal and Message Flow]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9849]]

## See also

- [[SBAS Integrity Data and User Bounds]]
- [[Protection Levels]]
- [[Alert Limits]]
