---
title: Protection Levels
description: Institutional concept page explaining protection levels as bounded-error measures used in SBAS integrity and aviation usability decisions
tags: [concept, protection-levels, sbas, integrity, aviation, alert-limits]
created: 2026-04-23
modified: 2026-05-02
status: reviewed
verification_status: source-scaffold-linked
---

# Protection Levels

## Scope and reader profile

This page explains **protection levels** as they are used in the SBAS integrity learning path. It is written for technical readers who need the operational meaning of the concept without treating provisional values in draft notes as verified requirements.

Exact mathematical definitions, confidence assumptions, receiver algorithms, and operation-specific thresholds must be checked against authoritative standards, service-provider documentation, and approved equipment/procedure material.

## Executive summary

A **protection level** is a conservative bound used to support a navigation usability decision. In an SBAS aviation context, it expresses whether the estimated navigation error is bounded tightly enough for the intended operation.

In simplified form:

```text
Protection level = a bound on possible navigation error for a specified dimension and operation context.
```

The protection level is not the same as the actual position error. It is a safety-oriented bound used to decide whether the navigation solution remains acceptable.

## Relationship to integrity and alert limits

Protection levels sit between the broader integrity function and the operational alert-limit decision:

```text
SBAS integrity provides monitored, bounded-error information.
The receiver or approved system logic represents that bound through protection levels.
Protection levels are compared with alert limits.
If the relevant protection level is not acceptable for the operation, the operation should not continue under that basis.
```

Related pages:

- [[SBAS Integrity]] — broader safety function.
- [[Alert Limits]] — operation-specific acceptability threshold.
- [[LPV-Approach-Procedure]] — example aviation context.

## Horizontal and vertical dimensions

Protection-level concepts are commonly discussed in horizontal and vertical dimensions because aviation operations can have different lateral and vertical requirements.

| Dimension                     | General interpretation             | Aviation relevance                                                   |
| ----------------------------- | ---------------------------------- | -------------------------------------------------------------------- |
| Horizontal protection concept | Bound on horizontal position error | Lateral containment, route/approach guidance, navigation performance |
| Vertical protection concept   | Bound on vertical position error   | Vertically guided operations and approach safety context             |

This page intentionally avoids assigning numerical values. Numeric thresholds must be tied to specific standards, service definitions, procedure types, and equipment approvals.

## Why protection levels matter

Protection levels matter because they convert integrity monitoring into operational decision support.

They help answer:

- Is the navigation solution bounded well enough for this operation?
- Is the receiver able to support the required mode or procedure?
- Should the operation continue under the selected guidance basis?
- Has the system crossed into a condition where an alert or mode change is required?

In this sense, protection levels are not merely mathematical outputs. They are part of the aviation safety chain connecting SBAS architecture to cockpit usability.

## Protection level is not actual error

A common misunderstanding is to read a protection level as the measured error. It is better understood as a conservative bound used for safety decision-making.

| Item                    | Meaning                                                                                                      |
| ----------------------- | ------------------------------------------------------------------------------------------------------------ |
| Actual navigation error | Difference between true position and estimated position; usually not directly known by the user in real time |
| Estimated accuracy      | Statistical or modeled estimate of expected position quality                                                 |
| Protection level        | Conservative bound used to support integrity and use-or-non-use decisions                                    |
| Alert limit             | Threshold associated with the intended operation                                                             |

The operational question is not “is the actual error small right now?” but “is the error sufficiently bounded for the approved operation?”

## Source anchors and current maturity

Current source scaffolds relevant to protection-level work include:

- [[SBAS Standards Source Matrix]]
- [[Source - RTCA DO-229]] — receiver/equipment source-family anchor for future official extraction of protection-level and usability-check language
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-242]]
- [[Source - ICAO Doc 9855]]
- [[Source - ICAO Doc 9854]]
- [[Source - RTCA DO-289]]
- [[SBAS Source Backlog]]

The page is `source-scaffold-linked`, not fully source-verified. It should be used as a structured conceptual reference until Annex 10, DO-229 receiver-standard, and operational-source scaffolds are deepened through direct official-text extraction.

## Use in the knowledge base

Protection-level language appears in:

- [[SBAS Integrity]]
- [[Alert Limits]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[Safety-Terminology]]

This page should be treated as the preferred concept anchor for future cleanup of those references.

## Implementation relevance

For implementation planning, protection levels influence:

- receiver eligibility and mode availability;
- integrity monitoring and performance reporting;
- procedure design and publication logic;
- safety-case arguments;
- validation of ionospheric and other error sources;
- interpretation of service outages or degraded modes.

For low-latitude regions, protection-level design and validation are linked to the ionospheric threat environment. See [[SBAS Ionospheric Threat — Empirical Evidence]] for the current research branch.

## Open verification tasks

1. Identify the source that should provide the primary definition of horizontal and vertical protection concepts for this KB.
2. Audit procedure notes for unsourced protection-level values or implied thresholds.
3. Separate generic GNSS protection-level language from SBAS-specific operational use.
4. Add source-backed equations only after the relevant standard or service definition is directly verified.
5. Link future numerical values to explicit source, operation, dimension, and confidence context.

## See also

- [[SBAS Integrity]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Source Backlog]]
