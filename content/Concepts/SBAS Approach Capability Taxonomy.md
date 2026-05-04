---
title: SBAS Approach Capability Taxonomy
description: Core taxonomy note routing LP, LPV, LNAV/VNAV, and related approach-capability language without turning capability labels into procedure or approval claims
tags: [sbas, approach, lpv, lnav-vnav, capability, taxonomy, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: active
verification_status: source-routed-taxonomy-no-operational-approval-claims
---

# SBAS Approach Capability Taxonomy

## Purpose

This note owns only the high-level taxonomy boundary for SBAS-related approach-capability language. It prevents LP, LPV, LNAV/VNAV, LNAV, APV, and related labels from being used as if they automatically prove a published procedure or operational authorization.

It does not define minima, procedure-design criteria, avionics requirements, or country-specific procedure inventories.

## Non-overlap ownership

| Topic                                | Owner                                                                 |
| ------------------------------------ | --------------------------------------------------------------------- |
| LPV learning page                    | [[LPV-Approach-Procedure]]                                            |
| Procedure-design / PBN source family | [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]]           |
| Receiver capability source family    | [[Source - RTCA DO-229]], [[Source - EASA ETSO-C145e and ETSO-C146e]] |
| Service-provider evidence            | [[Source - SBAS Service Providers]] and child notes                   |
| Operational proof                    | [[SBAS Operational Validation Dashboard]]                             |
| Capability taxonomy boundary         | this note                                                             |

## Capability-label caution

Capability labels are not operational proof.

| Label family       | What it can discuss at concept level                                               | What must not be inferred                                                           |
| ------------------ | ---------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| LP / LPV           | SBAS-supported approach-capability concepts where source families support the term | that a runway has a published LP/LPV procedure                                      |
| LNAV/VNAV          | lateral plus vertical navigation approach concept                                  | that SBAS is the only vertical source or that a specific operation is authorized    |
| LNAV               | lateral navigation approach concept                                                | that vertical guidance or SBAS integrity is available                               |
| APV / PBN language | approach and navigation-specification context                                      | exact criteria, minima, or state approval without procedure-design and AIP evidence |

## Safe wording pattern

```text
The label identifies a capability or procedure family. Operational use requires evidence for the service, receiver, procedure, aircraft, operator, and regulator layers.
```

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Standards to Operations Evidence Ladder]]
- [[SBAS Operational Validation Dashboard]]
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]]
- [[Source - RTCA DO-229]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[Source - SBAS Service Providers]]

## See also

- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[SBAS Service Volume and Coverage]]
