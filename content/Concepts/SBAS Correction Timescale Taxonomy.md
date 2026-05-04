---
title: SBAS Correction Timescale Taxonomy
description: Core taxonomy for routing fast, long-term, and ionospheric correction language without publishing detailed standards requirements
tags: [sbas, corrections, taxonomy, integrity, standards, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: reviewed
verification_status: source-routed-core-mechanism
---

# SBAS Correction Timescale Taxonomy

## Purpose

This note provides a conservative taxonomy for SBAS correction categories and timescale language.

It does not define message numbers, update intervals, validity timers, degradation rules, or algorithms.

## Taxonomy boundary

| Category language              | Concept-level use                                                                                                         | Do not infer                                                  |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| fast correction                | short-timescale correction concept for rapidly varying satellite-related errors where supported by standards/source notes | exact update interval, message type, or service commitment    |
| long-term correction           | slower correction concept for satellite orbit/clock context where supported by standards/source notes                     | exact model, validity, or accuracy                            |
| ionospheric correction         | correction/integrity context for ionospheric delay                                                                        | operational grid, GIVE value, or service certification        |
| degradation / timeout language | evidence that correction usability is time/status dependent                                                               | cockpit action, alerting logic, or detailed receiver behavior |

## Non-overlap rule

This note owns category separation only. It links to:

- [[SBAS Satellite Orbit and Clock Corrections]] for orbit/clock correction context;
- [[SBAS Ionospheric Grid Correction Concept]] for ionospheric correction routing;
- [[SBAS Signal and Message Flow]] for message-chain context;
- [[SBAS Receiver Modes and Annunciation]] for receiver presentation boundaries;
- [[SBAS Integrity Data and User Bounds]] for integrity-related user-bound context.

## Blocked claim patterns

Do not publish:

- exact correction update intervals without direct source extraction;
- a universal correction taxonomy if a source uses narrower definitions;
- service-specific performance claims copied into a generic concept note;
- receiver timeout or annunciation behavior without receiver/avionics evidence;
- procedure usability claims from correction-category language alone.

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Corrections and Integrity Separation]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9849]]

## See also

- [[SBAS Service Performance Concepts]]
- [[Protection Levels]]
- [[Alert Limits]]
