---
title: SBAS Architecture Flow
description: Compact flow diagram of the SBAS observation, processing, broadcast, receiver, and operational-use chain
tags: [sbas, architecture, diagram, flow, gnss]
created: 2026-05-02
modified: 2026-05-03
status: reviewed
verification_status: source-routed-core-diagram
---

# SBAS Architecture Flow

## Scope

This page provides a compact flow representation of the SBAS architecture. It is intended as a navigation aid for readers moving between [[What is SBAS]], [[SBAS Architecture]], [[SBAS Integrity]], and aviation operations pages.

## Functional flow

```mermaid
flowchart LR
  GNSS[GNSS satellites] --> REF[SBAS reference stations]
  GNSS --> USER[SBAS-capable user receiver]
  REF --> NET[Ground communications network]
  NET --> PROC[Master / processing stations]
  PROC --> MON[Integrity and service monitoring]
  MON --> MSG[Correction and integrity messages]
  MSG --> UPLINK[Uplink stations]
  UPLINK --> GEO[SBAS broadcast satellite or payload]
  GEO --> USER
  USER --> CHECK[Receiver applies corrections and checks integrity]
  CHECK --> OPS[Aviation operation if procedure, approval, equipment, and service conditions are satisfied]
  MON --> ALERT[Service alerts, alarms, or non-use conditions]
  ALERT --> OPS
```

## How to read the diagram

The diagram has two simultaneous paths:

1. **Correction path:** observations are processed into augmentation messages that improve user positioning.
2. **Integrity path:** monitoring and bounding determine whether the augmented solution should be used for the intended operation.

For aviation, the integrity path is not optional. SBAS-supported operations depend on the receiver and operational context determining that the navigation solution remains within the applicable bounds.

## Key interpretation cautions

- A broadcast signal alone does not equal operational approval.
- A technically capable receiver does not equal procedure availability.
- Regional coverage does not guarantee local runway minima.
- Research or testbed results do not automatically become certified operational service.
- Ionospheric threat discovery supports service design and validation; it is not itself an operational SBAS correction model.
- Message reception does not prove receiver approval, procedure publication, aircraft eligibility, or operator authorization.

## Source routing

Use [[SBAS Core Claim Routing]] to decide which source family can support each claim. Use [[SBAS Signal and Message Flow]] for the message chain and [[SBAS Ground Segment and Airborne Receiver Responsibilities]] for responsibility boundaries.

## See also

- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS Signal and Message Flow]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS in Civil Aviation MOC]]
- [[ASEAN SBAS Service-Model Options]]
