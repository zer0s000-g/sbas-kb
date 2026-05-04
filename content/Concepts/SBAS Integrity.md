---
title: SBAS Integrity
description: Institutional concept page explaining SBAS integrity, use-or-non-use logic, source boundaries, and its relationship to protection levels, alert limits, and LPV operations
tags: [concept, sbas, integrity, aviation, protection-levels, alert-limits]
created: 2026-04-23
modified: 2026-05-03
status: reviewed
verification_status: source-scaffold-linked-core-integrity
last_itf7_signal: "ITF/7 preliminary guidance (May 2025) confirms LP, LPV, LNAV/VNAV, LNAV as SBAS operational types; confirms SBAS Class 3 (LP+LPV) and Class 4 (fail-down to LNAV) avionics terminology"
---

# SBAS Integrity

## Scope and reader profile

This page explains **SBAS integrity** as a safety-relevant concept for aviation and implementation planning. It is intended for engineers, aviation specialists, researchers, regulators, ANSP staff, and readers using this knowledge base to understand why SBAS is more than a positioning-accuracy improvement.

This page is institutional-grade explanatory material, but it is not a substitute for the applicable ICAO, RTCA, EUROCAE, regulator, service-provider, aircraft, or operator documentation. Exact definitions, numerical thresholds, annunciation requirements, and procedure eligibility must be verified against authoritative sources before operational use.

## Executive summary

In SBAS, **integrity** is the function that supports timely warning when navigation information should not be used for the intended operation.

A concise institutional framing is:

```text
SBAS integrity is the service-and-receiver logic that helps decide whether an augmented GNSS solution is usable, not merely accurate.
```

The central distinction is important:

- **Accuracy** asks how close the estimated position is to the true position.
- **Integrity** asks whether the user can trust the navigation solution for a defined operation, and whether the user is warned quickly enough when that trust is no longer justified.

## Why integrity is central to SBAS

SBAS exists in aviation because a navigation service must do more than improve the estimated position. It must also support safety-relevant **use-or-non-use decisions**.

Integrity connects several layers:

1. monitoring of GNSS satellite and signal behavior;
2. estimation of residual uncertainty after corrections are applied;
3. generation and broadcast of integrity-related information;
4. receiver-side computation and checks;
5. comparison against operation-specific limits;
6. pilot/avionics response when the operation is no longer supported.

This is why [[SBAS Architecture]] treats integrity as a central architectural function rather than a side feature.

## Conceptual relationship

The core learning chain in this knowledge base is:

```text
SBAS integrity
  → produces or supports bounded-error information
  → represented to the receiver/user through protection-level concepts
  → compared against operation-specific alert limits
  → drives continue / discontinue / do-not-use decisions
```

Related pages:

- [[Protection Levels]] — bounded-error concept used in usability checks.
- [[Alert Limits]] — operation-specific threshold concept.
- [[LPV-Approach-Procedure]] — aviation use case where integrity discipline is critical.
- [[SBAS in Civil Aviation MOC]] — operational navigation map.

## Accuracy, correction, and integrity boundaries

Use [[SBAS Corrections and Integrity Separation]] for the source-of-truth distinction between correction and integrity.

This page owns the use-or-non-use concept. It does not own detailed message definitions, protection-level equations, alert-limit values, or procedure approval evidence.

| Boundary                                | Correct routing                                                |
| --------------------------------------- | -------------------------------------------------------------- |
| Signal/message details                  | [[SBAS Signal and Message Flow]]                               |
| Correction versus integrity distinction | [[SBAS Corrections and Integrity Separation]]                  |
| Receiver versus ground responsibility   | [[SBAS Ground Segment and Airborne Receiver Responsibilities]] |
| Operational approval escalation         | [[SBAS Operational Validation Dashboard]]                      |

## Integrity is not the same as accuracy

A common mistake is to treat high accuracy as sufficient for aviation use. In an institutional SBAS context, that is not adequate.

| Concept      | Question answered                                                                                     | Why it matters                                                               |
| ------------ | ----------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| Accuracy     | How close is the estimated position to the true position?                                             | Important for navigation quality, but not sufficient for safety-critical use |
| Integrity    | Can the user trust the navigation solution for this operation, and will unsafe conditions be alerted? | Central to aviation use-or-non-use decisions                                 |
| Availability | Is the required service usable when needed?                                                           | Supports planning and operational dependability                              |
| Continuity   | Will the service remain usable through the operation?                                                 | Important during time-critical phases such as approach                       |

A highly accurate solution that is not properly bounded or monitored may still be unsuitable for aviation operations requiring integrity assurance.

## What integrity depends on

SBAS integrity depends on both technical and institutional elements:

- reference-station monitoring quality;
- correction and integrity-message generation;
- conservative treatment of residual errors;
- ionospheric monitoring and uncertainty handling;
- receiver processing and alerting logic;
- service definition and performance monitoring;
- procedure design and publication;
- regulator, ANSP, aircraft, and operator approval chains.

For low-latitude and equatorial regions, ionospheric behavior is especially important. In this knowledge base, the research branch beginning with [[SBAS Ionospheric Threat — Empirical Evidence]] supports threat discovery and validation planning. It does not itself define an operational SBAS integrity model.

## Operational interpretation

For aviation readers, the simplified concept is:

```text
An SBAS-supported operation can continue only when the navigation solution remains within the required integrity bounds and all other operational approval conditions are satisfied.
```

This statement is conceptual. It must not be used to infer actual minima, alert limits, protection-level thresholds, receiver behavior, or procedure eligibility without source verification.

## Source anchors and current maturity

Current source scaffolds relevant to this page include:

- [[SBAS Standards Source Matrix]]
- [[SBAS Core Claim Routing]]
- [[SBAS Operational Validation Dashboard]]
- [[Source - RTCA DO-229]] — airborne equipment and receiver-related source-family anchor; official-text extraction still needed before using detailed receiver-integrity or alerting language.
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]] — ICAO SARPs/technical-provisions source-family routing scaffold.
- [[Source - ICAO Doc 9849]] — ICAO GNSS implementation-guidance scaffold.
- [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] — verified ITF/7 working paper confirms LP/LPV/LNAV/VNAV/LNAV operational types and Class 3/4 SBAS avionics as of May 2025; primary regional coordination forum anchor.
- [[Source - EASA ETSO-C145e and ETSO-C146e]] — public article-approval source family for ETSO receiver approval context.
- [[SBAS Source Backlog]] — active standards-source verification queue.

> **Institutional grounding note (2026-05-03):** The ICAO APAC ITF/7 Preliminary Draft SBAS Implementation Guidance Document (A3-WP05, rev3, 14 May 2025) confirms the following verified SBAS operational terminology as of its publication date:
>
> - Operational types: LP, LPV, LNAV/VNAV, LNAV
> - SBAS avionics classes: Class 3 (LP+LPV capability), Class 4 (fail-down to LNAV)
> - These confirm that the integrity-critical LPV operation and Class 3 avionics capability are recognized in the current ICAO APAC guidance framework.
>   This signal is consistent with but does not replace the DO-229F MOPS and Annex 10 SARPs definitions, which remain the primary authoritative source.

The source notes above are still scaffolds unless explicitly marked otherwise. This integrity page therefore remains `source-scaffold-linked`: it is suitable as a structured learning page, but not yet as a fully source-verified normative page.

## Implementation relevance

For implementation teams, integrity affects more than avionics. It shapes:

- system design requirements;
- monitoring network strategy;
- ionospheric threat-model validation;
- service definition and performance reporting;
- safety case structure;
- procedure publication decisions;
- contingency and outage handling;
- regulator and ANSP accountability.

For ASEAN-focused planning, these issues connect directly to [[ASEAN SBAS Deployment Barriers]], [[ASEAN SBAS Governance and Institutional Actors]], and [[ASEAN SBAS Service-Model Options]].

## Common misunderstandings

- **“SBAS improves accuracy, so integrity is automatically solved.”** Incorrect. Accuracy and integrity answer different questions.
- **“If SBAS coverage exists, LPV is automatically available.”** Incorrect. Procedures, approvals, service status, aircraft equipment, and operator authorization also matter.
- **“A research ionospheric model is an operational integrity model.”** Incorrect. Research models can support threat discovery and validation but do not automatically become certified service logic.
- **“One regional system’s performance figures can be copied into another region.”** Incorrect. Ionosphere, network geometry, service definition, and institutional approval differ by region.

## Open verification tasks

1. Verify which integrity statements should be anchored primarily to RTCA airborne-equipment material versus system-level augmentation material.
2. Separate DO-229 receiver/equipment integrity and annunciation requirements from Annex 10/service-provider monitoring requirements and from operational procedure responses.
3. Tie protection-level and alert-limit definitions to specific standards and service definitions.
4. Replace remaining unsourced numerical claims in procedure notes with source-backed statements or cautious qualitative language.
5. Identify which integrity claims belong to Annex 10, which belong to RTCA/EUROCAE receiver standards, and which belong to service-provider, procedure-design, or regulator sources.

## See also

- [[Protection Levels]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Signal and Message Flow]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Core Claim Routing]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
