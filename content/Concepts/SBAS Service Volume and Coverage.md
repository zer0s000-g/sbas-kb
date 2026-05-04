---
title: SBAS Service Volume and Coverage
description: Core concept note separating SBAS signal/service coverage from procedure availability, aircraft eligibility, and operational approval
tags: [sbas, service-volume, coverage, service-provider, operations, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: active
verification_status: source-routed-core-concept-no-new-operational-claims
---

# SBAS Service Volume and Coverage

## Purpose

This note explains how the knowledge base should treat SBAS service volume and coverage claims.

Coverage is a service or signal-support concept. It is not the same as operational authorization, procedure publication, receiver approval, or aircraft/operator eligibility.

## Claim boundary

| Statement type                                         | Correct owner                                    | Required evidence                                                        |
| ------------------------------------------------------ | ------------------------------------------------ | ------------------------------------------------------------------------ |
| A provider describes a service area or coverage region | service-provider source note                     | official provider service definition, status page, or performance report |
| A signal can be received                               | service/provider or technical measurement note   | source-specific signal evidence                                          |
| A receiver can process supported SBAS messages         | receiver/equipment source family                 | MOPS/article-approval evidence                                           |
| A procedure is published for a runway                  | operational validation dashboard / aviation note | AIP/AIS/procedure source                                                 |
| An aircraft/operator may use the procedure             | operational validation dashboard / aviation note | avionics, aircraft, operator, and regulator evidence                     |

## Why coverage is often overused

A map or service-region statement can be useful for planning, but it is an incomplete aviation claim. Operational use requires multiple layers beyond geography:

1. source-defined service commitment;
2. applicable signal/message support;
3. receiver capability and approval basis;
4. procedure design and publication;
5. aircraft installation and operator authorization;
6. current operational status and contingency logic.

## Safe wording pattern

```text
The source supports a coverage or service-area statement within its stated scope. It does not by itself establish procedure availability, aircraft eligibility, or operational authorization.
```

## Relationship to service-provider notes

Use [[Source - SBAS Service Providers]] as the family router and child source notes for system-specific evidence. This page should not duplicate system facts from those source notes.

## Relationship to operational validation

Use [[SBAS Operational Validation Dashboard]] before converting a coverage statement into an aviation operational statement.

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Service Performance Concepts]]
- [[Source - SBAS Service Providers]]
- [[SBAS Operational Validation Dashboard]]
- [[SBAS Standards Source Matrix]]

## See also

- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Approach Capability Taxonomy]]
- [[SBAS MOC]]
