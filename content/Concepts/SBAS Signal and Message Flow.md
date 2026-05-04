---
title: SBAS Signal and Message Flow
description: Core concept note explaining the SBAS observation-to-message-to-receiver chain while routing detailed message definitions to Annex 10 and airborne-equipment standards
tags: [sbas, signals, messages, architecture, integrity, receiver]
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: source-routed-concept-no-message-number-extraction
---

# SBAS Signal and Message Flow

## Scope

This note explains the functional SBAS signal and message chain at institutional concept level.

It deliberately does not publish detailed SBAS message-type definitions, bit fields, numerical timing requirements, or receiver algorithms. Those details must be extracted from [[Source - ICAO Annex 10 Volume I GNSS SBAS]] and [[Source - RTCA DO-229]] before they become authoritative KB content.

## Functional chain

SBAS information moves through a safety-relevant chain:

1. GNSS satellites transmit base navigation signals.
2. SBAS reference stations observe the signals at surveyed locations.
3. Processing functions estimate corrections and integrity-related parameters.
4. The service packages the information into augmentation messages.
5. Uplink infrastructure sends those messages to the broadcast payload.
6. The SBAS broadcast signal delivers messages to user receivers.
7. The receiver applies supported messages and performs mode/usability checks.
8. The operation continues only when the receiver, procedure, service, aircraft, crew, and approval basis all support the intended use.

See [[SBAS Architecture Flow]] for the compact diagram and [[SBAS Ground Segment and Airborne Receiver Responsibilities]] for responsibility separation.

## Message content families

At a concept level, SBAS message flow can be understood through content families rather than message numbers.

| Content family                             | Conceptual purpose                                                            | Source-routing boundary                                                           |
| ------------------------------------------ | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| Satellite status / usability               | Indicates which GNSS satellites or augmentation signals may be used           | exact flags and validity rules require standards extraction                       |
| Fast or satellite-related corrections      | Reduces satellite clock/orbit and related errors where supported              | detailed applicability belongs to Annex 10 / DO-229 extraction                    |
| Ionospheric correction and uncertainty     | Supports delay correction and integrity bounding for ionosphere-related error | do not replace with research TEC model notes                                      |
| Integrity bounds / degradation information | Supports receiver usability and alerting decisions                            | do not publish numerical bounds without standards and service-definition evidence |
| Timing and service messages                | Supports receiver processing, time alignment, and service interpretation      | details remain standards-bound                                                    |

## Why message flow is not enough

A message can be valid as a technical broadcast object without proving aviation operational authorization.

The following are separate layers:

| Layer                             | Evidence needed                                      |
| --------------------------------- | ---------------------------------------------------- |
| Message format exists             | standards/source extraction                          |
| Receiver can process it           | receiver MOPS and article-approval evidence          |
| Service broadcasts it in a region | service-provider source evidence                     |
| Procedure can use it              | procedure-design and AIP/procedure evidence          |
| Aircraft/operator may fly it      | aircraft, avionics, operator, and regulator evidence |

This separation prevents the common error of treating signal reception as procedure eligibility.

## Relationship to integrity

SBAS message flow has a correction path and an integrity path. The correction path improves the navigation solution. The integrity path helps determine whether that solution is usable for the intended operation.

The integrity path connects this note to:

- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Ranging Sources and Time Reference]]
- [[SBAS Corrections and Integrity Separation]]

## Current source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-229]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[SBAS Operational Validation Dashboard]]

## Open verification tasks

1. Directly extract official SBAS message families from the applicable Annex 10 amendment baseline.
2. Map airborne receiver processing and message-eligibility requirements to DO-229 extraction.
3. Separate service-provider message support from generic standards definitions.
4. Add only source-backed message tables; avoid unsourced message-number summaries.

## See also

- [[SBAS Architecture]]
- [[SBAS Architecture Flow]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Integrity]]
- [[SBAS Source Backlog]]
