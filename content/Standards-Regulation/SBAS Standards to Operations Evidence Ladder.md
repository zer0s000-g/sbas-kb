---
title: SBAS Standards to Operations Evidence Ladder
description: Institutional evidence ladder separating SBAS standards, service definitions, receiver approval, procedure design, AIP publication, aircraft installation, and operator authorization
tags: [sbas, standards, operations, evidence, regulator, procedure, institutional]
category: standards
created: 2026-05-04
modified: 2026-05-04
status: active
verification_status: source-routing-no-new-operational-claims
---

# SBAS Standards to Operations Evidence Ladder

## Purpose

This note defines the evidence ladder required before a core SBAS statement can become an operational aviation statement.

It is a routing note, not an operational approval document.

## The ladder

| Layer                              | Question                                                  | Primary owner in this KB                                   | Evidence family                                                       |
| ---------------------------------- | --------------------------------------------------------- | ---------------------------------------------------------- | --------------------------------------------------------------------- |
| 1. Standards concept               | What does the standards family define or constrain?       | [[SBAS Standards Source Matrix]]                           | Annex 10, DO-229, Doc 9849, procedure-design source notes             |
| 2. Service definition              | What does the provider state it broadcasts or supports?   | [[Source - SBAS Service Providers]] and child notes        | official provider service definitions/status/performance publications |
| 3. Receiver capability             | What can the approved receiver process and present?       | [[SBAS Receiver Modes and Annunciation]]                   | MOPS and article-approval source families                             |
| 4. Procedure design                | What type of procedure can be designed?                   | procedure-design source notes and aviation pages           | PANS-OPS/PBN and state design material                                |
| 5. Procedure publication           | Is a procedure published for a specific runway and cycle? | [[SBAS Operational Validation Dashboard]]                  | AIP/AIS/procedure database evidence                                   |
| 6. Aircraft/operator authorization | May this aircraft/operator fly it?                        | [[SBAS Operational Validation Dashboard]]                  | aircraft, avionics, operator, and regulator evidence                  |
| 7. Current operational use         | Is it usable now under current status and contingencies?  | operational validation dashboard and source-specific notes | current service, NOTAM/status, AIP, operator, and procedure evidence  |

## Rule

A claim can move upward only when the next evidence layer is explicitly sourced. Lower layers do not automatically prove higher layers.

## Common failure modes

- Treating Annex 10 or DO-229 as proof that a state has published procedures.
- Treating a service-provider page as proof that aircraft and operators are approved.
- Treating an AIP procedure as proof that all SBAS-capable aircraft may fly it.
- Treating a receiver capability label as a service-performance claim.

## Relationship to existing routing notes

- [[SBAS Core Claim Routing]] owns core claim ownership.
- [[SBAS Operational Validation Dashboard]] owns operational escalation and validation status.
- This note owns the evidence ladder between standards and operations.

## Source anchors

- [[SBAS Standards Source Matrix]]
- [[SBAS Core Claim Routing]]
- [[SBAS Operational Validation Dashboard]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-229]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]]
- [[Source - SBAS Service Providers]]

## See also

- [[SBAS Approach Capability Taxonomy]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[LPV-Approach-Procedure]]
