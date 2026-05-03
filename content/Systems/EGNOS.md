---
title: EGNOS
description: Source-routed system note for the European Geostationary Navigation Overlay Service, grounded in official EGNOS Safety of Life Service Definition material and separated from ETSO, procedure-design, AIP, and operational-authorization sources
tags: [system, egnos, sbas, aviation, regional-system, europe]
created: 2026-04-23
modified: 2026-05-03
status: reviewed
verification_status: source-routed-to-official-egnos-sol-sdd
---

# EGNOS

## Scope status

This page is a source-routed system note for EGNOS, Europe's SBAS implementation and aviation Safety of Life service family.

The verified EGNOS-specific claims on this page route to [[Source - EGNOS]]. Cross-system provider context routes to [[Source - SBAS Service Providers]]. Article approval, procedure design, and operational authorization are intentionally separated.

Boundary:

- This page does not publish country/runway-specific EGNOS procedure availability or minima.
- This page does not treat EGNOS SoL service definition as aircraft, receiver, operator, or national operational authorization.
- This page does not duplicate detailed SDD excerpts; those belong in [[Source - EGNOS]].

## Working definition

EGNOS is the European Geostationary Navigation Overlay Service, Europe's satellite-based augmentation system. Official EGNOS Safety of Life Service Definition material describes the aviation SoL service as augmenting GPS L1 C/A through correction data and integrity information for safety-critical aviation applications.

## Official source signals

| Signal type              | Current authenticated source-routed statement                                                                                                                                     |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| System identity          | EGNOS = European Geostationary Navigation Overlay Service; routed to [[Source - EGNOS]]                                                                                           |
| Service document         | EGNOS Safety of Life Service Definition Document, Version 03-06 / Issue 3.6, published 2024-09-09 and marked In Force                                                             |
| Service scope            | Official EGNOS material describes the SoL Service for Aviation as openly provided, freely accessible without direct charge, and tailored to safety-critical aviation applications |
| ICAO requirement context | Official EGNOS material states that the service is compliant with APV-I and Category I precision-approach requirements as defined by ICAO Annex 10                                |
| Authorization boundary   | Official EGNOS material states that operational use may require specific authorization by relevant authorities                                                                    |

## Relationship to civil aviation use

EGNOS matters in this KB because it connects European service-provider material to:

- EASA article-approval routing in [[Source - EASA ETSO-C145e and ETSO-C146e]];
- ICAO SARPs routing in [[Source - ICAO Annex 10 Volume I GNSS SBAS]];
- PBN/procedure-design routing in [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]];
- operational deployment questions that must later be resolved through regulator, ANSP, and AIP material.

## Claims intentionally not duplicated here

To prevent overlapping knowledge, this page does not reproduce the EGNOS SDD's service-area, architecture, performance, liability, or user-obligation detail. Those details belong in [[Source - EGNOS]] and any later direct-extraction child notes.

## Source anchors

- [[Source - EGNOS]] -- dedicated EGNOS child source note for official EGNOS SoL Service Definition material.
- [[Source - SBAS Service Providers]] -- service-provider family router for system identity and source-maturity tracking.
- [[Source - EASA ETSO-C145e and ETSO-C146e]] -- EASA article-approval routing.
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]] -- ICAO SARPs routing.
- [[SBAS Standards Source Matrix]] -- claim-routing matrix for standards/source families.

## Open verification questions

- Which current official EGNOS/ESSP source should be used for live performance/status claims?
- Which national AIP/ANSP sources should be used for country-specific EGNOS procedure deployment?
- Which EGNOS service documents should be extracted if Open Service, EDAS, or maritime ESMAS enters the KB scope?

## See also

- [[Source - EGNOS]]
- [[Source - SBAS Service Providers]]
- [[WAAS vs EGNOS]]
- [[WAAS]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[SBAS Source Backlog]]
