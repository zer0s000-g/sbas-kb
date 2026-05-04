---
title: SBAS Ground Segment and Airborne Receiver Responsibilities
description: Core concept note separating SBAS service/ground-segment responsibilities from airborne receiver and operational-approval responsibilities
tags: [sbas, ground-segment, receiver, avionics, service-provider, operations]
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: source-routed-concept-no-operational-approval
---

# SBAS Ground Segment and Airborne Receiver Responsibilities

## Purpose

This note separates responsibilities across the SBAS safety chain. It prevents ground-segment, service-provider, receiver, and operational-approval claims from being merged into one unsupported statement.

## Responsibility split

| Layer                   | Typical responsibility                                                                                                  | Evidence family                                                         |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| GNSS constellation      | Base navigation signals                                                                                                 | constellation/interface and ICAO/GNSS technical sources                 |
| SBAS ground segment     | Monitoring, correction estimation, integrity-related processing, service monitoring                                     | Annex 10 / Doc 9849 / service-provider documentation                    |
| SBAS broadcast path     | Uplink and augmentation signal delivery                                                                                 | service-provider and standards evidence                                 |
| Airborne receiver       | Decode messages, apply supported corrections, compute/check usability, present modes/alerts according to approval basis | DO-229 and article-approval evidence such as ETSO                       |
| Procedure and operation | Decide whether a runway/procedure/aircraft/operator may use the capability                                              | procedure-design, regulator, ANSP, AIP, aircraft, and operator evidence |

## What the ground segment can prove

A service-provider or ground-segment source may support statements about system architecture, broadcast service, monitoring network, service definition, or performance reports within its scope.

It does not automatically prove:

- a particular receiver can use the service;
- a particular runway has an approved SBAS procedure;
- an aircraft installation is approved;
- an operator is authorized;
- a pilot may fly a specific operation.

## What receiver standards can prove

Receiver standards and article-approval sources can support receiver capability and equipment-approval context within their scope.

They do not automatically prove:

- a regional service is available;
- a specific procedure is published;
- a state regulator has approved an operation;
- the service provider is meeting current performance commitments.

## Why this matters

SBAS documentation often fails when it compresses the safety chain into one sentence such as “the system supports LPV.”

Institutional-grade documentation must ask: which layer supports what?

| Better question                      | Required answer                                      |
| ------------------------------------ | ---------------------------------------------------- |
| Is the technical service defined?    | service-definition evidence                          |
| Is the receiver capability approved? | MOPS / ETSO / article evidence                       |
| Is a procedure published?            | AIP/procedure evidence                               |
| Is aircraft/operator use authorized? | aircraft, avionics, operator, and regulator evidence |
| Is the service currently suitable?   | performance/status and operational evidence          |

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-229]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[Source - SBAS Service Providers]]
- [[SBAS Operational Validation Dashboard]]

## See also

- [[SBAS Architecture]]
- [[SBAS Signal and Message Flow]]
- [[SBAS Corrections and Integrity Separation]]
- [[LPV-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]
