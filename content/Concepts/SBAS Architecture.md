---
title: SBAS Architecture
description: Institutional explanation of the end-to-end Satellite-Based Augmentation System architecture, from GNSS monitoring to aviation receiver use
tags: [sbas, architecture, gnss, integrity, aviation, systems]
created: 2026-05-02
modified: 2026-05-02
status: institutional
verification_status: synthesis-with-caveats
---

# SBAS Architecture

## Scope and reader profile

This page explains the functional architecture of a Satellite-Based Augmentation System. It is written for readers who need to understand how SBAS works as an operational chain rather than as a collection of isolated terms.

The architecture below is a reference model. Exact implementation details vary by system, generation, region, service definition, and standards baseline.

## Executive summary

SBAS architecture links five major functions:

1. **observe** GNSS performance at surveyed reference locations
2. **estimate** corrections and integrity information over a wide area
3. **validate** whether the service can safely support intended operations
4. **broadcast** augmentation messages to equipped users
5. **apply and monitor** the messages in certified receivers and operational procedures

The architecture is therefore both technical and institutional. A working SBAS is not just satellites and algorithms; it also requires monitoring, maintenance, procedure design, certification, safety oversight, and user equipment standards.

## System elements

| Element | Primary role | Notes for aviation interpretation |
|---|---|---|
| GNSS constellations | Provide the base ranging signals that users navigate with | SBAS augments GNSS; it does not replace GNSS |
| Reference stations | Measure GNSS signal behavior at known locations | Station geometry and reliability affect service monitoring capability |
| Communications network | Carries observations from reference stations to processing centers | Latency, redundancy, and data quality matter for real-time service |
| Master/processing stations | Estimate corrections, integrity parameters, and service messages | This is where monitoring logic becomes operational information |
| Uplink stations | Send SBAS messages to broadcast satellites or broadcast payloads | Uplink continuity is part of service dependability |
| Broadcast satellites/payloads | Transmit augmentation messages to users | Often GEO in traditional SBAS; exact architecture depends on system design |
| User receivers | Apply corrections and check integrity information | Certified aviation use depends on approved equipment and procedures |
| Operations and monitoring organization | Maintains service, alarms, configuration control, and performance reporting | Institutional capability is as important as technical architecture |

## Functional data path

The core architecture can be read as a safety-relevant data path:

1. GNSS signals are observed by reference stations and user receivers.
2. Reference-station observations are sent to processing facilities.
3. Processing facilities estimate correction and integrity information.
4. The service validates whether the information is suitable for broadcast.
5. Uplink infrastructure transmits messages to broadcast satellites or payloads.
6. Users receive both GNSS and SBAS signals.
7. The receiver applies SBAS messages and computes whether the navigation solution is usable.
8. The operation proceeds only if the receiver, procedure, aircraft, crew, and approval basis support the intended use.

See [[SBAS Architecture Flow]] for a compact diagram.

## Correction and integrity products

SBAS messages commonly support several classes of user information:

- satellite orbit and clock correction information
- ionospheric correction or ionospheric uncertainty information
- integrity bounds and degradation indicators
- satellite health and usability information
- timing and service messages needed for receiver processing

This page intentionally avoids assigning exact message numbers or performance thresholds. Those details must be tied to the applicable standards and service definitions before being used as authoritative references.

## Integrity as the central architectural feature

The defining architectural difference between a casual correction service and aviation-grade augmentation is integrity.

Within this knowledge base, [[SBAS Integrity]] is the bridge between system architecture and operational use. Integrity links:

- monitoring of GNSS and augmentation behavior
- conservative bounding of residual errors
- receiver-side checks against [[Protection Levels]] and [[Alert Limits]]
- operational eligibility for approach and other flight phases
- alerting when the service should not be used

A useful architecture description must therefore explain both the correction path and the warning path. An accurate but unbounded navigation solution is not sufficient for safety-relevant aviation use.

## Interfaces and dependencies

SBAS architecture depends on several interface classes:

| Interface | Why it matters |
|---|---|
| GNSS signal interface | determines what base measurements are available |
| reference-station data interface | affects quality, latency, and monitoring coverage |
| processing-to-uplink interface | affects message timeliness and continuity |
| broadcast signal/message interface | determines receiver compatibility |
| receiver-to-procedure interface | determines what the pilot, avionics, and procedure can use |
| service-provider-to-regulator interface | determines approval, reporting, and safety accountability |

For institutional deployment, the last two interfaces are often as decisive as the first four.

## Architecture and regional implementation

A region considering SBAS deployment must evaluate more than coverage maps. It must decide how architecture, governance, and service model interact.

Key questions include:

- Is the service national, regional, hosted, or cooperative?
- Who operates the reference network, processing function, uplink, and monitoring organization?
- Which regulator or regional body accepts safety accountability?
- Which aircraft equipage and procedure-design pathways exist?
- How will low-latitude ionospheric behavior be monitored and bounded?
- How will outages, configuration changes, and performance reporting be handled?

The ASEAN branch explores these questions through [[ASEAN SBAS Adoption Landscape]], [[ASEAN SBAS Governance and Institutional Actors]], [[ASEAN SBAS Service-Model Options]], and [[GIPTA 2.0 and ASEAN SBAS Implementation Pathway]].

## Relationship to other augmentation methods

SBAS is one augmentation architecture among several:

- [[SBAS-vs-Other-Augmentation-Methods]] compares wide-area, local-area, and aircraft-based approaches.
- [[GBAS-Approach-Procedure]] represents the local-area augmentation branch.
- [[RNP-Approach-Procedure]] and [[RNAV-Approach-Procedure]] connect GNSS navigation to performance-based navigation concepts.

The central distinction is scale and accountability: SBAS provides wide-area correction and integrity information through a service architecture, while GBAS and ABAS solve different operational problems with different infrastructure and approval models.

## Source anchors and caveats

Relevant source scaffolds include:

- [[Source - RTCA DO-229]]
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-289]]
- [[Source - ICAO Doc 9854]]
- [[Source - ICAO Doc 9855]]

These source notes should be strengthened before this architecture page is promoted from synthesis-based institutional guidance to fully standards-linked reference material.

## See also

- [[What is SBAS]]
- [[SBAS Architecture Flow]]
- [[SBAS-Terminology]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS Source Backlog]]
