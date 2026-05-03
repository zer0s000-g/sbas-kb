---
title: WAAS
description: Source-routed system note for the FAA Wide Area Augmentation System, grounded in official FAA public WAAS material and separated from MOPS, TSO, procedure-design, and aircraft/operator-approval sources
tags: [system, waas, sbas, aviation, regional-system, united-states]
created: 2026-04-23
modified: 2026-05-03
status: reviewed
verification_status: source-routed-to-official-faa-waas-material
---

# WAAS

## Scope status

This page is a source-routed system note for WAAS, the U.S. SBAS implementation operated in the FAA civil-aviation context.

The verified WAAS-specific claims on this page route to [[Source - WAAS]]. Cross-system provider context routes to [[Source - SBAS Service Providers]]. Equipment and article-approval claims are kept separate and route to [[Source - RTCA DO-229]] and [[Source - FAA TSO-C145e and TSO-C146e]].

Boundary:

- This page does not publish real-time WAAS status, service-volume boundaries, or availability statistics.
- This page does not approve a particular aircraft, receiver, operator, route, runway, or procedure.
- This page does not compare WAAS performance against other SBAS systems unless matched official provider evidence exists.

## Working definition

WAAS is the Wide Area Augmentation System, the FAA/U.S. satellite-based augmentation implementation for civil aviation. FAA public material describes WAAS as supporting all classes of aircraft and all phases of flight, including en-route navigation, departures, arrivals, and vertically guided landing approaches at qualified locations in the U.S. National Airspace System context.

## Official source signals

| Signal type            | Current authenticated source-routed statement                                                                                                               |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| System identity        | WAAS = Wide Area Augmentation System; routed to [[Source - WAAS]]                                                                                           |
| Operating authority    | Federal Aviation Administration, U.S. Department of Transportation                                                                                          |
| Service role           | FAA public material describes WAAS as developed for civil aviation and supporting all classes of aircraft in all phases of flight                           |
| Approach context       | FAA material connects WAAS to vertically guided landing approaches in instrument meteorological conditions at qualified locations                           |
| LPV/LP public snapshot | FAA August 2025 quick-facts material reports LPV and LP procedure-count snapshots; keep those counts in [[Source - WAAS]] rather than duplicating them here |

## Relationship to civil aviation use

WAAS is relevant to the KB because it is a major operational SBAS reference point for civil aviation. It connects service-provider commitments to:

- airborne SBAS equipment standards in [[Source - RTCA DO-229]];
- FAA article approval in [[Source - FAA TSO-C145e and TSO-C146e]];
- procedure-design and PBN context in [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] and [[Source - FAA and EASA Procedure-Design and PBN Material]];
- civil-aviation navigation and approach topics in [[SBAS in Civil Aviation MOC]].

## Claims intentionally not duplicated here

To prevent overlapping knowledge, this page does not copy the full FAA LPV/LP counts, equipment caveats, or source excerpts. Those belong in [[Source - WAAS]]. This page only states the system-level meaning and routes readers to the source note.

## Source anchors

- [[Source - WAAS]] -- dedicated WAAS child source note for official FAA WAAS material.
- [[Source - SBAS Service Providers]] -- service-provider family router for system identity and source-maturity tracking.
- [[Source - RTCA DO-229]] -- SBAS airborne-equipment MOPS routing.
- [[Source - FAA TSO-C145e and TSO-C146e]] -- FAA article-approval routing.
- [[SBAS Standards Source Matrix]] -- claim-routing matrix for standards/source families.

## Open verification questions

- Which FAA source should be treated as the canonical WAAS service-definition/performance standard for service-volume and availability claims?
- Which FAA procedure-publication source should be used if runway-specific LPV/LP procedure availability enters the KB?
- Which FAA operational guidance should be used for aircraft/operator authorization questions?

## See also

- [[Source - WAAS]]
- [[Source - SBAS Service Providers]]
- [[WAAS vs EGNOS]]
- [[EGNOS]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Source Backlog]]
