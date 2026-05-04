---
title: SBAS Service Status and Operational Notices
description: Core routing note for SBAS service-status, outage, notice, NOTAM, and current-operational-use claims without duplicating provider-specific status pages
tags: [sbas, service-status, operations, notam, validation, core]
category: concepts
created: 2026-05-04
modified: 2026-05-04
status: reviewed
verification_status: source-routed-core-mechanism
---

# SBAS Service Status and Operational Notices

## Purpose

This note explains how to route SBAS service-status and operational-notice claims.

It does not list current outages, NOTAMs, AIRAC cycle data, procedure status, or provider-specific operational bulletins.

## Non-overlap rule

| Claim type                                                  | Correct owner                                                              |
| ----------------------------------------------------------- | -------------------------------------------------------------------------- |
| service-provider identity or service definition             | [[Source - SBAS Service Providers]] and child source notes                 |
| service area / coverage                                     | [[SBAS Service Volume and Coverage]]                                       |
| service performance concept                                 | [[SBAS Service Performance Concepts]]                                      |
| procedure publication                                       | [[SBAS Operational Validation Dashboard]] and aviation/procedure notes     |
| current outage / notice / cycle-specific operational status | source-specific regulator, ANSP, AIS/AIP, NOTAM, or provider status source |
| this page                                                   | routing rules for status/notice claims only                                |

## Why this boundary matters

A static knowledge-base page can easily become stale if it lists current operational status. This page therefore routes status claims to the evidence family that must be checked, instead of duplicating transient facts.

## Safe wording pattern

```text
At publication time, the referenced source described [status/notice context]. Current operational use must be checked against current service, AIP/AIS, NOTAM, procedure, aircraft, and operator evidence.
```

## Blocked claim patterns

Do not publish:

- current outage or NOTAM details in a generic concept note;
- a permanent operational claim from an old status page;
- provider service status as proof of procedure availability;
- procedure availability as proof of aircraft/operator authorization;
- operational continuity claims without source-dated evidence.

## Source anchors

- [[SBAS Core Claim Routing]]
- [[SBAS Standards to Operations Evidence Ladder]]
- [[SBAS Operational Validation Dashboard]]
- [[SBAS Service Performance Concepts]]
- [[Source - SBAS Service Providers]]

## See also

- [[SBAS Service Volume and Coverage]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Approach Capability Taxonomy]]
