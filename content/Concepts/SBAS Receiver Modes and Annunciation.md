---
title: SBAS Receiver Modes and Annunciation
description: Core routing note for SBAS receiver modes, alerts, and annunciation concepts without publishing detailed MOPS requirements or cockpit procedures
tags: [sbas, receiver, avionics, annunciation, modes, integrity, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: active
verification_status: source-routed-core-concept-no-detailed-mops-claims
---

# SBAS Receiver Modes and Annunciation

## Purpose

This note explains where receiver-mode and annunciation claims belong in the knowledge base.

It does not publish cockpit procedures, detailed alerting logic, message validity rules, receiver algorithms, equipment classes, or pilot operating instructions. Those require direct standards, avionics, aircraft, and operator sources.

## Receiver concept boundaries

| Topic              | Safe concept-level statement                                                                                     | Required evidence before detail                                    |
| ------------------ | ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Receiver mode      | A receiver may present or use modes according to its design and approval basis                                   | MOPS, article approval, aircraft/avionics manuals                  |
| Annunciation       | The receiver/flight deck must communicate relevant mode or alert status to the crew according to approved design | avionics and aircraft documentation                                |
| Integrity alerting | Receiver behavior is part of the integrity chain                                                                 | DO-229 and operational sources before detailed timing/logic claims |
| Procedure use      | Receiver mode must match procedure and operation requirements                                                    | procedure chart/AIP, aircraft, operator, and regulator evidence    |

## What this note blocks

Do not infer:

- a cockpit annunciation from a service-provider source;
- a receiver mode from SBAS coverage;
- aircraft eligibility from a generic equipment standard;
- procedure authorization from receiver capability alone;
- pilot action from a concept page.

## Relationship to integrity

Receiver behavior is where the broadcast and airborne approval layers meet operational use. It must be routed through:

1. [[SBAS Signal and Message Flow]] for message path;
2. [[SBAS Corrections and Integrity Separation]] for correction/integrity distinction;
3. [[Protection Levels]] and [[Alert Limits]] for usability concepts;
4. [[SBAS Standards to Operations Evidence Ladder]] for escalation into operations.

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Standards to Operations Evidence Ladder]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[Source - RTCA DO-229]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[SBAS Operational Validation Dashboard]]

## See also

- [[LPV-Approach-Procedure]]
- [[SBAS Approach Capability Taxonomy]]
- [[SBAS Integrity]]
