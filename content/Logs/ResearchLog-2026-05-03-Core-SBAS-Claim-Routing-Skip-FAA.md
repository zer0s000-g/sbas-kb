---
title: Research Log - 2026-05-03 - Core SBAS Claim Routing Skip FAA
description: Work log for the ten-cycle core SBAS solidification pass that prioritized core knowledge, avoided overlapping claims, and intentionally skipped new FAA-specific extraction
tags: [research-log, sbas, core-knowledge, source-hardening, provenance]
created: 2026-05-03
modified: 2026-05-03
status: completed
verification_status: internal-work-log
---

# Research Log - 2026-05-03 - Core SBAS Claim Routing Skip FAA

## Scope

This log records the ten-cycle core SBAS solidification pass requested on 2026-05-03.

User constraints:

- Documentation quality must be institutional grade.
- Overlapping knowledge is forbidden.
- Claims must be validated/authenticated against original or authoritative sources.
- The pass should prioritize core SBAS knowledge.
- Long reference-website expansion should be skipped.
- FAA-specific extraction should be skipped.

## Source posture

No new long reference-website expansion was performed in this pass. The work used existing source anchors and source-family routing already present in the vault, especially:

- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-229]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]]
- [[Source - SBAS Service Providers]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Operational Validation Dashboard]]

Existing FAA-related notes were not deleted because they are part of the historical source-routing graph, but this cycle did not deepen FAA TSO, procedure-design, NFDC, WAAS, or other FAA-specific extraction.

## Core routing added

Created [[SBAS Core Claim Routing]] as the institutional routing note for core concept claims.

The note separates the following claim families:

| Claim family                        | Owner note                                                     | Boundary                                                                    |
| ----------------------------------- | -------------------------------------------------------------- | --------------------------------------------------------------------------- |
| Definition and beginner orientation | [[What is SBAS]]                                               | High-level explanation only                                                 |
| Architecture                        | [[SBAS Architecture]] / [[SBAS Architecture Flow]]             | System chain only; no detailed standards values                             |
| Signal/message flow                 | [[SBAS Signal and Message Flow]]                               | Flow explanation only; no message-number or bit-field claims                |
| Correction versus integrity         | [[SBAS Corrections and Integrity Separation]]                  | Accuracy support is not operational safety approval                         |
| Ground/airborne responsibility      | [[SBAS Ground Segment and Airborne Receiver Responsibilities]] | Service, receiver, procedure, aircraft, and operator layers remain separate |
| Integrity/protection/alerting       | [[SBAS Integrity]], [[Protection Levels]], [[Alert Limits]]    | Relationships only; no unsupported numerical thresholds                     |
| Operational validation              | [[SBAS Operational Validation Dashboard]]                      | Escalation path only; not original evidence                                 |

## Core notes created

- [[SBAS Signal and Message Flow]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Core Claim Routing]]

## Existing core notes hardened

- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS Architecture Flow]]
- [[SBAS-Terminology]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[Ionospheric Model Validation]]
- [[Total Electron Content (TEC)]]
- [[SBAS MOC]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]

## Non-overlap rules established

- Core concept notes explain relationships; they do not own detailed standards text.
- Standards source notes own evidence provenance and source-family boundaries.
- Service-provider notes own provider-specific identity and bounded service/development signals.
- The operational validation dashboard owns the escalation ladder from service-provider evidence to regulator, ANSP, AIP, procedure, aircraft, and operator evidence.
- Numerical alerting, protection-level, message, and operational values remain blocked until direct primary-source extraction supports them.

## Deferred work

- Direct Annex 10 extraction remains the highest-value core standards task.
- Direct DO-229 extraction remains required before receiver/message/protection-level details can be published as verified requirements.
- Direct Doc 9849 extraction remains required before state-implementation guidance can be treated as fully verified.
- Non-FAA operational validation can proceed for EGNOS, GAGAN, MSAS, KASS, BDSBAS, SouthPAN, and SDCM where official regulator/AIP/service-performance sources are available.

## See also

- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[SBAS MOC]]
