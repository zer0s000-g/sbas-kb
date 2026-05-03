---
title: BDSBAS
description: Source-routed system note for the BeiDou Satellite-Based Augmentation System, grounded in the official BDSBAS-B1C ICD and bounded technical-public evidence without overstating aviation operational approval
tags: [system, bdsbas, sbas, aviation, regional-system, beidou, china]
created: 2026-04-23
modified: 2026-05-03
status: reviewed
verification_status: source-routed-to-official-bdsbas-icd
---

# BDSBAS

## Scope status

This page is a source-routed system note for BDSBAS, the BeiDou Satellite-Based Augmentation System.

The verified BDSBAS-specific claims on this page route to [[Source - BDSBAS]]. Cross-system provider context routes to [[Source - SBAS Service Providers]]. ICAO SARPs and equipment/MOPS claims remain separated through [[Source - ICAO Annex 10 Volume I GNSS SBAS]] and [[Source - RTCA DO-229]].

Boundary:

- This page does not publish current CAAC operational approval, airport/runway procedure availability, or approach minima.
- This page does not treat a signal-interface ICD as a service declaration.
- This page does not convert technical-development targets into operational claims.

## Working definition

BDSBAS is the BeiDou Satellite-Based Augmentation System. The official China Satellite Navigation Office BDSBAS-B1C ICD identifies BDSBAS as part of the BeiDou system and defines the Single Frequency BDSBAS-B1C signal interface.

## Official source signals

| Signal type                   | Current authenticated source-routed statement                                                                                        |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| System identity               | BDSBAS = BeiDou Satellite-Based Augmentation System; routed to [[Source - BDSBAS]]                                                   |
| Official source               | BDSBAS-B1C Signal In Space Interface Control Document, Version 1.0, July 2020                                                        |
| Issuing authority             | China Satellite Navigation Office                                                                                                    |
| Signal-interface role         | The official ICD defines BDSBAS-B1C Single Frequency service signal characteristics and message structure                            |
| GEO/PRN signal                | The official ICD identifies GEO slots and PRNs for BDSBAS-B1C; details are kept in [[Source - BDSBAS]]                               |
| Technical-development context | NAVIGATION 2021 article supports bounded development context for SF/DFMC and APV-I/CAT-I targets, but not final operational approval |

## Relationship to civil aviation use

BDSBAS matters in this KB because it is a China/BeiDou-centered SBAS implementation relevant to Asia-Pacific SBAS comparison and future regional interoperability questions. Its current authenticated layer in this vault is strongest for official signal-interface evidence, not for aviation-operational procedure deployment.

Use BDSBAS as:

- a system identity and signal-interface source-routed page;
- an Asia-Pacific comparator in [[ASEAN SBAS Source Backlog]] only with explicit boundaries;
- a future extraction target for CAAC/service-declaration/procedure-publication evidence.

## Claims intentionally not duplicated here

To prevent overlapping knowledge, this page does not copy the ICD's PRN, timing, modulation, or message-structure details. Those details belong in [[Source - BDSBAS]]. This page only states the system-level meaning and source boundaries.

## Source anchors

- [[Source - BDSBAS]] -- dedicated BDSBAS child source note for official BDSBAS-B1C ICD signals and bounded technical-public context.
- [[Source - SBAS Service Providers]] -- service-provider family router for system identity and source-maturity tracking.
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]] -- ICAO SARPs routing.
- [[Source - RTCA DO-229]] -- SBAS MOPS routing.
- [[SBAS Standards Source Matrix]] -- claim-routing matrix for standards/source families.

## Open verification questions

- Which CAAC or official Chinese civil-aviation source declares BDSBAS operational aviation service, if publicly available?
- Which current BeiDou/CSNO source defines BDSBAS service area, performance commitment, and status beyond the B1C ICD?
- Which source should be used for DFMC/B2a operational maturity if that branch enters the KB?

## See also

- [[Source - BDSBAS]]
- [[Source - SBAS Service Providers]]
- [[Asia-Pacific SBAS Implementation Patterns]]
- [[MSAS]]
- [[GAGAN]]
- [[KASS]]
- [[SouthPAN]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS Source Backlog]]
