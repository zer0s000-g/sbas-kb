---
title: SBAS Core Claim Routing
description: Institutional routing map for core SBAS claims, separating architecture, corrections, integrity, receiver behavior, service-provider evidence, and operational approval evidence
tags: [sbas, core, source-routing, standards, provenance, institutional]
category: standards
created: 2026-05-03
modified: 2026-05-04
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

| Claim type                                      | Preferred KB owner                                             | Primary source family to check                                                                                                                          | Do not use instead                                           |
| ----------------------------------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ |
| What SBAS is                                    | [[What is SBAS]]                                               | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]]                                                                               | service-provider marketing pages alone                       |
| Functional architecture                         | [[SBAS Architecture]]                                          | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]], system-specific service-provider notes where architecture is system-specific | a regional system page as a generic architecture source      |
| Signal/message flow                             | [[SBAS Signal and Message Flow]]                               | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]]                                                                                 | unsourced message-number tables                              |
| Correction-vs-integrity distinction             | [[SBAS Corrections and Integrity Separation]]                  | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]], [[Source - ICAO Doc 9849]]                                                     | accuracy-performance claims alone                            |
| Protection-level concept                        | [[Protection Levels]]                                          | [[Source - RTCA DO-229]], [[Source - ICAO Annex 10 Volume I GNSS SBAS]]                                                                                 | procedure minima, chart minima, or service coverage pages    |
| Alert-limit concept                             | [[Alert Limits]]                                               | [[Source - RTCA DO-229]], [[Source - ICAO Annex 10 Volume I GNSS SBAS]], regulator/procedure evidence when operational                                  | free-floating numerical tables                               |
| Ground segment responsibility                   | [[SBAS Ground Segment and Airborne Receiver Responsibilities]] | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - ICAO Doc 9849]], service-provider source notes                                                | receiver MOPS alone                                          |
| Airborne receiver responsibility                | [[SBAS Ground Segment and Airborne Receiver Responsibilities]] | [[Source - RTCA DO-229]], [[Source - EASA ETSO-C145e and ETSO-C146e]]                                                                                   | service-provider status pages alone                          |
| Service performance concepts                    | [[SBAS Service Performance Concepts]]                          | standards, service definitions, performance reports, operational-validation evidence when operational                                                   | accuracy claims alone                                        |
| Service volume and coverage                     | [[SBAS Service Volume and Coverage]]                           | service-provider service definitions and child source notes                                                                                             | procedure, aircraft, or operator evidence                    |
| Approach capability labels                      | [[SBAS Approach Capability Taxonomy]]                          | DO-229 / ETSO / procedure-design / AIP evidence depending on claim layer                                                                                | capability labels as operational proof                       |
| Standards-to-operations escalation              | [[SBAS Standards to Operations Evidence Ladder]]               | standards, service-provider, receiver, procedure, AIP, aircraft, operator, and regulator evidence                                                       | a single source family for the whole chain                   |
| Receiver modes and annunciation                 | [[SBAS Receiver Modes and Annunciation]]                       | DO-229, ETSO, avionics/aircraft/operator evidence when detailed                                                                                         | service-provider coverage or generic receiver mentions       |
| Ranging sources and time reference              | [[SBAS Ranging Sources and Time Reference]]                    | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]], GNSS/source-provider evidence where applicable                                 | service-provider pages alone or generic timing claims        |
| Satellite orbit and clock corrections           | [[SBAS Satellite Orbit and Clock Corrections]]                 | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]], [[Source - ICAO Doc 9849]]                                                     | operational approval or integrity claims by correction alone |
| Ionospheric grid correction concept             | [[SBAS Ionospheric Grid Correction Concept]]                   | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]], ionospheric research source notes for threat discovery only                    | GIVE/model/service certification from research notes         |
| Correction timescale taxonomy                   | [[SBAS Correction Timescale Taxonomy]]                         | Annex 10 / DO-229 / Doc 9849 source families                                                                                                            | update interval/message tables without extraction            |
| Integrity data and user bounds                  | [[SBAS Integrity Data and User Bounds]]                        | [[Source - ICAO Annex 10 Volume I GNSS SBAS]], [[Source - RTCA DO-229]], receiver/procedure evidence where operational                                  | accuracy or correction claims alone                          |
| Service status and operational notices          | [[SBAS Service Status and Operational Notices]]                | service-provider, regulator, ANSP, AIS/AIP, NOTAM/status, aircraft/operator evidence as applicable                                                      | static concept pages for current operational status          |
| Service availability or coverage                | [[Source - SBAS Service Providers]] and child source notes     | system-specific service-provider documentation                                                                                                          | Annex 10 or DO-229 alone                                     |
| Procedure availability and operational approval | [[SBAS Operational Validation Dashboard]]                      | regulator, ANSP, AIP, aircraft, avionics, and operator evidence                                                                                         | service-provider source notes alone                          |

## Current source posture

The core SBAS layer is now suitable for institutional learning and source-routed analysis. It is not yet a fully extracted normative standards layer.

The source posture is:

- Annex 10, Volume I is represented as a public-catalog-reviewed ICAO SARPs/technical-provisions routing note.
- Doc 9849 is represented as an ICAO GNSS implementation-guidance routing note with public metadata and public working-paper signals.
- DO-229 is represented as the airborne equipment MOPS routing note; detailed direct official-text extraction remains a high-value future target.
- EASA ETSO-C145e/C146e is the preferred public article-approval source family for this skip-FAA cycle.
- Service-provider child notes exist for major systems, but those notes do not prove procedure availability or operator approval.
- The second core-solidification pass added service-performance, coverage, approach-capability, evidence-ladder, and receiver-mode routing notes without adding new detailed normative claims or long-reference website extraction.
- The third core-solidification pass added mechanism routing for ranging/time reference, satellite orbit/clock corrections, ionospheric grid-correction context, correction timescales, integrity data/user bounds, and service-status/notice claims. It remains concept/routing-only and avoids long reference-website expansion.

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
- [[SBAS Service Performance Concepts]]
- [[SBAS Service Volume and Coverage]]
- [[SBAS Approach Capability Taxonomy]]
- [[SBAS Standards to Operations Evidence Ladder]]
- [[SBAS Receiver Modes and Annunciation]]
- [[SBAS Ranging Sources and Time Reference]]
- [[SBAS Satellite Orbit and Clock Corrections]]
- [[SBAS Ionospheric Grid Correction Concept]]
- [[SBAS Correction Timescale Taxonomy]]
- [[SBAS Integrity Data and User Bounds]]
- [[SBAS Service Status and Operational Notices]]
- [[SBAS Source Backlog]]
