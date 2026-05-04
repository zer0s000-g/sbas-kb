---
title: SBAS Core Claim Routing
description: Institutional routing map for core SBAS claims, separating architecture, corrections, integrity, receiver behavior, service-provider evidence, and operational approval evidence
tags: [sbas, core, source-routing, standards, provenance, institutional]
category: standards
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: source-routing-no-new-normative-claims
---

# SBAS Core Claim Routing

## Purpose

This note protects the core SBAS knowledge layer from overlap and source drift.

It does not define SBAS technical requirements. It owns only the routing rules: which note and source family should carry each kind of core claim.

## Non-overlap rule

Do not duplicate detailed standards, service-provider, or operational claims here.

- Core concept pages own concise explanations.
- Source notes own extracted evidence and boundaries.
- The standards matrix owns cross-source classification.
- The operational validation dashboard owns regulator, ANSP, AIP, aircraft, and operator escalation.

## Core claim-routing table

| Claim type                                      | Preferred KB owner                                             | Primary source family to check                                                                                                                          | Do not use instead                                        |
| ----------------------------------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| What SBAS is                                    | [[What is SBAS]]                                               | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]]                                                                               | service-provider marketing pages alone                    |
| Functional architecture                         | [[SBAS Architecture]]                                          | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]], system-specific service-provider notes where architecture is system-specific | a regional system page as a generic architecture source   |
| Signal/message flow                             | [[SBAS Signal and Message Flow]]                               | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]]                                                                                 | unsourced message-number tables                           |
| Correction-vs-integrity distinction             | [[SBAS Corrections and Integrity Separation]]                  | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]], [[Source - ICAO Doc 9849]]                                                     | accuracy-performance claims alone                         |
| Protection-level concept                        | [[Protection Levels]]                                          | [[Source - RTCA DO-229]], [[Source - ICAO Annex 10 Volume I GNSS SBAS]]                                                                                 | procedure minima, chart minima, or service coverage pages |
| Alert-limit concept                             | [[Alert Limits]]                                               | [[Source - RTCA DO-229]], [[Source - ICAO Annex 10 Volume I GNSS SBAS]], regulator/procedure evidence when operational                                  | free-floating numerical tables                            |
| Ground segment responsibility                   | [[SBAS Ground Segment and Airborne Receiver Responsibilities]] | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]], service-provider source notes                                                | receiver MOPS alone                                       |
| Airborne receiver responsibility                | [[SBAS Ground Segment and Airborne Receiver Responsibilities]] | [[Source - RTCA DO-229]], [[Source - EASA ETSO-C145e and ETSO-C146e]]                                                                                   | service-provider status pages alone                       |
| Service availability or coverage                | [[Source - SBAS Service Providers]] and child source notes     | system-specific service-provider documentation                                                                                                          | Annex 10 or DO-229 alone                                  |
| Procedure availability and operational approval | [[SBAS Operational Validation Dashboard]]                      | regulator, ANSP, AIP, aircraft, avionics, and operator evidence                                                                                         | service-provider source notes alone                       |

## Current source posture

The core SBAS layer is now suitable for institutional learning and source-routed analysis. It is not yet a fully extracted normative standards layer.

The source posture is:

- Annex 10, Volume I is represented as a public-catalog-reviewed ICAO SARPs/technical-provisions routing note.
- Doc 9849 is represented as an ICAO GNSS implementation-guidance routing note with public metadata and public working-paper signals.
- DO-229 is represented as the airborne equipment MOPS routing note; detailed direct official-text extraction remains a high-value future target.
- EASA ETSO-C145e/C146e is the preferred public article-approval source family for this skip-FAA cycle.
- Service-provider child notes exist for major systems, but those notes do not prove procedure availability or operator approval.

## Blocked claim patterns

Do not publish these patterns unless the relevant source family is extracted and linked:

| Blocked pattern                                                     | Why blocked                                                                              |
| ------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| “SBAS guarantees LPV at airports inside coverage”                   | service coverage does not equal procedure publication or aircraft/operator approval      |
| “Protection level equals actual error”                              | protection level is a conservative bound used for integrity/usability decisions          |
| “Alert limit is a chart minimum”                                    | alert limits, procedure minima, and operational minima are different evidence layers     |
| “A testbed model is an operational correction model”                | research validation is not service certification                                         |
| “One SBAS system’s performance proves another system’s performance” | systems differ by service definition, network geometry, ionosphere, and approval context |

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Operational Validation Dashboard]]
- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS Signal and Message Flow]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Source Backlog]]
