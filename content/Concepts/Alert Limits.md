---
title: Alert Limits
description: Institutional concept page explaining alert limits as operation-specific thresholds in SBAS integrity and aviation usability decisions
tags: [concept, alert-limits, sbas, integrity, aviation, protection-levels]
created: 2026-04-23
modified: 2026-05-02
status: reviewed
verification_status: source-scaffold-linked
---

# Alert Limits

## Scope and reader profile

This page explains **alert limits** in the SBAS integrity learning path. It is intended for readers who need to understand how operation-specific thresholds relate to protection levels, alerts, and use-or-non-use decisions.

Exact alert-limit values, dimensions, procedure-specific requirements, and alerting behavior must be verified against authoritative standards, service definitions, equipment documentation, and approved operational material.

## Executive summary

An **alert limit** is an operation-specific threshold used to decide whether the navigation solution is acceptable for continued use in that operation.

In simplified form:

```text
If the relevant protection level is within the relevant alert limit,
the navigation solution may be usable for the operation, provided all other required conditions are also satisfied.
```

The alert limit is not a generic warning preference. It is tied to the operation and must be interpreted through the applicable aviation approval context.

## Relationship to protection levels

Alert limits and protection levels are paired concepts:

| Concept               | Role                                                           |
| --------------------- | -------------------------------------------------------------- |
| [[Protection Levels]] | Express a conservative bound on navigation error               |
| Alert limits          | Define the maximum acceptable bound for the intended operation |
| [[SBAS Integrity]]    | Provides the broader monitoring and alerting function          |

A simplified relationship is:

```text
Protection level ≤ alert limit → operation may be supported, if all other conditions are satisfied.
Protection level > alert limit → operation is not supported under that basis.
```

This is conceptual. The exact logic, timing, annunciation, and operational response must come from the applicable standards and approved operating procedures.

## Why alert limits are operation-specific

Different operations tolerate different navigation-error bounds. En-route, terminal, non-precision, and vertically guided approach contexts do not have identical safety requirements.

Alert limits therefore depend on:

- phase of flight;
- procedure type;
- lateral versus vertical dimension;
- aircraft equipment and receiver mode;
- service definition and regional approval;
- procedure publication and operational authorization.

This is why this knowledge base avoids publishing free-floating alert-limit numbers unless they are tied to a verified source and context.

## What alert limits are not

Alert limits are often misunderstood. They are not:

- the actual navigation error;
- a generic accuracy target;
- an arbitrary cockpit warning threshold;
- evidence by themselves that a procedure is authorized;
- interchangeable across regions, systems, service definitions, or operation types.

They are part of a structured integrity decision chain.

## Operational interpretation

For aviation use, alert limits help determine whether the current navigation mode remains acceptable for the intended operation.

A useful institutional phrasing is:

```text
The alert limit defines the operation's tolerance boundary; the protection level indicates whether the current bounded solution fits inside that boundary.
```

If it does not, the operation must transition according to the approved procedure and aircraft/operator guidance. This page does not define that response.

## Source anchors and current maturity

Relevant current source scaffolds include:

- [[SBAS Standards Source Matrix]]
- [[Source - RTCA DO-229]] — receiver/equipment source-family anchor for future official extraction of alerting and usability-check language
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-242]]
- [[Source - ICAO Doc 9855]]
- [[Source - ICAO Doc 9854]]
- [[Source - RTCA DO-289]]
- [[SBAS Source Backlog]]

This page remains `source-scaffold-linked`. It provides a careful conceptual framework, but not yet a verified table of alert-limit values. Any future values must be tied to exact source family, operation type, revision/date, and applicability conditions; DO-229 alone is not enough to publish operational minima or procedure-specific thresholds.

## Use in the knowledge base

Alert-limit language appears in:

- [[SBAS Integrity]]
- [[Protection Levels]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]

This page should be the preferred concept anchor for future cleanup of alerting and threshold language.

## Implementation relevance

For implementation planning, alert limits affect:

- service-performance assessment;
- procedure eligibility and publication;
- cockpit mode availability and annunciation;
- safety case and hazard analysis;
- contingency procedures and downgrade logic;
- training and operational documentation.

For regional SBAS planning, they highlight why a signal or coverage footprint is not enough. The service must support the operation’s integrity requirements under the relevant regional conditions.

## Open verification tasks

1. Verify authoritative source language for alert-limit definitions and dimensions.
2. Audit procedure pages for unsourced alert-limit values and remove or qualify them.
3. Separate alert-limit concepts from generic weather minima, decision altitude/height, and procedure chart minima.
4. Add source-backed values only when the source, operation type, dimension, and revision are explicit.
5. Connect verified alert-limit material to [[LPV-Approach-Procedure]] and [[SBAS in Civil Aviation MOC]].

## See also

- [[SBAS Integrity]]
- [[Protection Levels]]
- [[LPV-Approach-Procedure]]
- [[SBAS Architecture]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Source Backlog]]
