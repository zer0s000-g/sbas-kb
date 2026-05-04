---
title: SBAS Service Performance Concepts
description: Core concept note separating SBAS accuracy, integrity, availability, continuity, coverage, and service-commitment claims without importing operational approval claims
tags: [sbas, performance, integrity, availability, continuity, service-definition, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: active
verification_status: source-routed-core-concept-no-new-normative-claims
---

# SBAS Service Performance Concepts

## Purpose

This note defines how the knowledge base talks about SBAS performance without collapsing different claim families into one unsupported statement.

It does not publish numerical performance values, service commitments, or operational minima. Those belong in source notes, service-provider documents, standards, regulator/AIP evidence, or procedure documentation.

## Non-overlap rule

This note owns only the conceptual separation among performance terms. It does not own:

- SBAS architecture: [[SBAS Architecture]]
- signal/message chain: [[SBAS Signal and Message Flow]]
- correction versus integrity boundary: [[SBAS Corrections and Integrity Separation]]
- system-specific service statements: [[Source - SBAS Service Providers]] and child source notes
- regulator/AIP/procedure approval: [[SBAS Operational Validation Dashboard]]

## Performance concept separation

| Concept            | Core question                                                            | Evidence family                                                       | Boundary                                                                                   |
| ------------------ | ------------------------------------------------------------------------ | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Accuracy           | How close is the estimated position to the true position?                | standards, service definitions, performance reports                   | Accuracy alone does not prove integrity or operational authorization                       |
| Integrity          | Is the user warned or excluded when the solution should not be used?     | Annex 10 / DO-229 source families, integrity concept pages            | Integrity claims require bounded-error and alerting context, not accuracy statements alone |
| Availability       | Is the required service usable when needed under the stated conditions?  | service definitions, performance reports, procedure/operation context | Availability depends on the service and operation; it is not universal coverage            |
| Continuity         | Is the service expected to remain usable through the relevant operation? | service definitions and operational context                           | Continuity is operation-specific and cannot be inferred from a static map                  |
| Coverage           | Where is the service or signal intended to be usable?                    | service-provider documentation and service-volume evidence            | Coverage does not prove procedure publication, aircraft eligibility, or operator approval  |
| Service commitment | What the provider commits to deliver and monitor                         | official service definitions and provider publications                | Provider commitments do not replace standards, receiver approval, or AIP evidence          |

## Safe wording pattern

Use layered language:

```text
A source may support a statement about [performance concept] within [source scope], but it does not by itself prove [different evidence layer].
```

Examples:

- A service-definition page may support a service-availability claim within its stated scope, but it does not prove aircraft/operator approval.
- A receiver standard may support receiver-capability routing, but it does not prove a regional service is currently available.
- A performance report may support measured service behavior during a period, but it does not automatically prove future procedure availability.

## Blocked claim patterns

Do not publish:

- “accurate enough for LPV” without integrity, receiver, procedure, and approval evidence;
- “inside the service area means operationally approved”;
- “broadcasting SBAS means every compatible receiver may fly a procedure”;
- “one provider’s service statistics apply to another provider”;
- “research/testbed performance is certified service performance.”

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Service Volume and Coverage]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Operational Validation Dashboard]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-229]]
- [[Source - SBAS Service Providers]]

## See also

- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
