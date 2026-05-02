---
title: What is SBAS?
description: Institutional beginner gateway explaining Satellite-Based Augmentation Systems for aviation, integrity, architecture, standards, and implementation planning
tags: [sbas, gnss, beginner, aviation, integrity, architecture]
created: 2026-05-02
modified: 2026-05-02
status: institutional
verification_status: synthesis-with-caveats
---

# What is SBAS?

## Scope and reader profile

This page is the beginner gateway for the SBAS knowledge base. It is intended for technical readers who are new to SBAS but need a reliable mental model: civil aviation specialists, researchers, students, ANSP staff, regulators, procedure designers, and regional implementation teams.

The page provides an institutional-grade overview, but it is not a certification document. Operational minima, equipment approval, service availability, and safety-case decisions must be checked against the applicable standards, regulator material, service-provider documentation, and aircraft/operator approvals.

## Short definition

**Satellite-Based Augmentation System (SBAS)** is a wide-area augmentation service for GNSS. It uses a ground monitoring network and processing infrastructure to generate correction and integrity information, then broadcasts that information to users through satellite signals.

For aviation, the most important point is that SBAS is not only an accuracy improvement system. Its safety value comes from **integrity**: the ability to support timely warning when navigation information should not be used for a particular operation.

## The operational problem SBAS solves

Unaugmented GNSS can provide useful positioning, but aviation operations also need confidence that the navigation solution is suitable for the intended phase of flight. SBAS helps by addressing several operational needs:

- correction of GNSS-related errors over a wide service area
- integrity monitoring and alerting for safety-relevant use
- improved availability of vertically guided approach procedures where conventional ground infrastructure may be limited
- consistent regional service coverage for equipped aircraft
- a technical basis for LPV and other SBAS-supported operational concepts where approved

The practical result is not simply “better GPS.” SBAS is a service architecture that connects satellites, ground monitoring, real-time computation, broadcast messages, certified receivers, procedure design, and operational approval.

## Basic system chain

At a high level, SBAS works through the following chain:

1. **GNSS satellites** transmit navigation signals.
2. **SBAS reference stations** observe GNSS signal behavior at known surveyed locations.
3. **Processing or master stations** estimate correction and integrity information from the monitoring network.
4. **Uplink stations** send SBAS messages to broadcast satellites or other broadcast infrastructure.
5. **SBAS broadcast signals** deliver correction and integrity data to users.
6. **SBAS-capable receivers** apply the messages and determine whether the resulting navigation solution is usable for the intended operation.

See [[SBAS Architecture]] for a fuller explanation and [[SBAS Architecture Flow]] for a compact flow diagram.

## What SBAS adds to GNSS

| Function | Meaning for users | Aviation significance |
|---|---|---|
| Correction | Improves the navigation solution by reducing modeled error sources | Supports more consistent positioning performance across a service area |
| Integrity | Provides information used to determine whether the solution should be trusted | Central to safety-relevant procedure use |
| Availability | Increases the chance that service requirements are met where coverage and geometry allow | Important for operational dependability and procedure planning |
| Continuity | Supports uninterrupted use during a defined operation | Important during approach and other time-critical phases |
| Standardized broadcast | Delivers augmentation data through aviation-relevant signal and message structures | Enables certified avionics and harmonized operations |

These concepts should not be treated as generic marketing claims. Their exact meaning depends on the applicable service definition, equipment standard, procedure type, region, and phase of flight.

## Relationship to aviation operations

SBAS is most visible to aviation users through vertically guided approach operations such as LPV where the service, receiver, procedure, aircraft, crew, and regulatory approval chain all support the operation.

Within this knowledge base, the aviation branch starts at [[SBAS in Civil Aviation MOC]] and links to:

- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[GBAS-Approach-Procedure]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]

Draft procedure notes may contain provisional figures or illustrative language. Treat them as learning aids until each claim is tied to specific source anchors.

## What SBAS is not

SBAS is often misunderstood. The following boundaries are important:

- SBAS is **not** a standalone navigation constellation. It augments GNSS.
- SBAS is **not** the same as GBAS. GBAS is airport/local-area augmentation; SBAS is wide-area augmentation.
- SBAS is **not** the same as ABAS/RAIM. ABAS uses aircraft/receiver-side monitoring logic rather than a regional augmentation broadcast.
- SBAS availability in a region does **not** automatically mean every runway has an approved LPV procedure.
- SBAS technical feasibility does **not** automatically mean institutional, regulatory, economic, or operational readiness.
- SBAS research use of GNSS-RO or ionospheric modeling is **not** itself an operational correction service.

See [[SBAS-vs-Other-Augmentation-Methods]] for augmentation comparisons.

## Standards and source posture

This site currently has source scaffolds for several high-value standards and guidance references, including:

- [[SBAS Standards Source Matrix]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-289]]
- [[Source - ICAO Doc 9854]]
- [[Source - ICAO Doc 9855]]

These source notes are useful anchors, but several still require direct verification of exact title, edition, scope, and downstream claim support. Use [[SBAS Source Backlog]] as the active queue for source-hardening work.

## Implementation relevance

For implementation planning, SBAS should be evaluated as a system-of-systems problem:

- technical feasibility: ionosphere, coverage, monitoring, broadcast, receiver ecosystem
- operational value: approach access, terrain/weather constraints, remote or archipelagic networks
- institutional readiness: regulator, ANSP, AIS/AIM, procedure design, safety oversight
- service model: national, regional, hosted, testbed, or phased deployment pathway
- source discipline: standards and institutional evidence must be separated from synthesis

The ASEAN branch applies this logic to Southeast Asia through [[ASEAN SBAS Adoption Landscape]], [[ASEAN SBAS Deployment Barriers]], and [[ASEAN SBAS Service-Model Options]].

## See also

- [[SBAS Architecture]]
- [[SBAS Architecture Flow]]
- [[SBAS-Terminology]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
