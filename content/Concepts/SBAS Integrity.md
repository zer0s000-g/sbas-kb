---
title: SBAS Integrity
description: Draft concept note on the role of integrity in satellite-based augmentation for aviation
tags: [concept, sbas, integrity, aviation, provisional]
created: 2026-04-23
modified: 2026-04-23
status: draft
verification_status: source-scaffold-linked
---

# SBAS Integrity

## Definition status
This note is a draft concept note.

Boundary:
- It synthesizes existing vault language and terminology.
- It is linked to provisional source scaffolds, not yet to verified source extraction.
- Treat detailed operational thresholds and quantitative requirements elsewhere in the vault as provisional unless tied to dedicated source notes.

## Working definition
Within the current vault, SBAS integrity is the function by which an augmentation service supports timely user warning when positioning information should not be relied upon for the intended operation.

This framing is consistent with the vault's recurring emphasis on:
- integrity monitoring
- alerting
- protection levels
- operational use in approach procedures

## Why integrity matters in SBAS
SBAS is not only about improving position accuracy. In aviation context, the vault repeatedly treats integrity as the safety-relevant mechanism that determines whether SBAS-supported guidance can be used for a given phase of flight.

Operationally, integrity connects:
- system monitoring in [[SBAS-Standards-Regulation]]
- approach-use logic in [[SBAS in Civil Aviation MOC]]
- procedure-level concepts in [[LPV-Approach-Procedure]] and [[LNAV-VNAV-Approach-Procedure]]
- safety terminology in [[Safety-Terminology]]

## Closely related concepts
- [[Protection Levels]]
- [[Alert Limits]]
- [[Safety-Terminology]]
- [[SBAS-Terminology]]
- [[WAAS]]

## Current source anchors
These are source scaffolds, not completed source notes.
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9855]]
- [[Source - ICAO Doc 9854]]
- [[Source - RTCA DO-289]]

## What the vault currently implies
The current vault implies that SBAS integrity includes at least the following themes:
- continuous monitoring of navigation solution suitability
- comparison of navigation performance against operation-specific bounds
- timely alerting when those bounds are not met
- coupling between technical integrity concepts and procedure authorization in civil aviation

These statements are synthesis from existing notes and still need direct source confirmation.

## Aviation implications
In the current vault structure, integrity appears as the bridge between system design and operational approval.

Examples already present in draft notes:
- approach procedures refer to integrity warnings and missed-approach logic
- the civil-aviation MOC links integrity to protection level and alert-limit requirements
- standards notes connect integrity to certification and monitoring requirements

## Open provenance questions
- Which core SBAS integrity statements should be anchored to [[Source - RTCA DO-242]] versus [[Source - RTCA DO-229]]?
- Which statements about testing and monitoring belong under [[Source - ICAO Doc 9854]] or [[Source - RTCA DO-289]] instead of technical-specification notes?
- Which parts of the current vault are using integrity as a generic safety term rather than a specifically defined operational concept?

## See also
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
