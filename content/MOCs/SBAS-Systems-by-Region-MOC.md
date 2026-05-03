---
title: SBAS Systems by Region MOC
description: Institutional navigation map for regional SBAS implementations, comparators, and source-backed system research
tags: [MOC, regional, sbas, comparison, systems]
category: mocs
created: 2026-04-19
modified: 2026-05-03
version: 2.0
status: reviewed
verification_status: synthesis-with-caveats
---

# SBAS Systems by Region MOC

## Scope

This note maps regional SBAS systems and system-comparison research. It is a navigation and synthesis page, not a certified service-performance table.

Exact system status, coverage, performance, service levels, satellite payloads, and operational approvals must be checked against current service-provider, regulator, and standards material before use in formal analysis.

## Primary regional system notes

| System | Region / role                                  | Current note |
| ------ | ---------------------------------------------- | ------------ |
| WAAS   | United States / North America reference system | [[WAAS]]     |
| EGNOS  | Europe reference system                        | [[EGNOS]]    |
| MSAS   | Japan / Asia-Pacific comparator                | [[MSAS]]     |
| GAGAN  | India / low-latitude regional comparator       | [[GAGAN]]    |
| BDSBAS | China / BeiDou-linked Asia-Pacific comparator  | [[BDSBAS]]   |

Future source-backed notes may cover KASS, SDCM, SouthPAN, ASECNA, and other SBAS or SBAS-like programs. Until dedicated notes exist, those systems should be discussed as candidate research targets rather than linked as completed pages.

## Comparison and synthesis notes

- [[WAAS vs EGNOS]]
- [[MSAS vs GAGAN]]
- [[Asia-Pacific SBAS Implementation Patterns]]
- [[Japan MSAS GBAS Lessons for ASEAN SBAS]]
- [[GIPTA 2.0 and ASEAN SBAS Implementation Pathway]]

## ASEAN relevance

ASEAN does not currently appear in this knowledge base as a single deployed regional SBAS equivalent to WAAS or EGNOS. The ASEAN branch is instead an implementation-planning branch focused on readiness, governance, barriers, demand, source evidence, and service-model choice.

Start with:

- [[ASEAN SBAS Adoption Landscape]]
- [[ASEAN SBAS Readiness Heuristic]]
- [[ASEAN SBAS Operational Demand Drivers]]
- [[ASEAN SBAS Deployment Barriers]]
- [[ASEAN SBAS Governance and Institutional Actors]]
- [[ASEAN SBAS Service-Model Options]]
- [[GIPTA 2.0 MOC]]

## How to compare systems responsibly

Regional SBAS systems should not be compared only by headline accuracy or coverage numbers. A high-quality comparison should separate:

| Dimension                | Why it matters                                                                |
| ------------------------ | ----------------------------------------------------------------------------- |
| Service definition       | Defines what the provider claims and for which users                          |
| Aviation approval status | Determines whether signals support actual operations                          |
| Coverage and geometry    | Indicates where service may be usable, not necessarily where procedures exist |
| Integrity concept        | Determines safety-relevant usability                                          |
| Procedure inventory      | Shows where operational benefits are actually available                       |
| Aircraft equipage        | Determines who can use the procedures                                         |
| Regulatory environment   | Determines approval and oversight pathway                                     |
| Ionospheric environment  | Especially important for low-latitude and equatorial regions                  |
| Institutional model      | Determines who operates, funds, monitors, and governs the service             |

## Source posture

Current system notes are useful but still need stronger direct source anchors. Priority source families include:

- service-provider definition documents and performance reports;
- regulator and ANSP operational approval material;
- ICAO APAC and regional planning documents;
- RTCA/EUROCAE/ICAO standards scaffolds in [[SBAS Source Backlog]];
- ASEAN and GIPTA-specific source stacks in [[ASEAN SBAS Source Backlog]] and [[GIPTA 2.0 MOC]].

## Research priorities

1. Build a source-backed regional comparison matrix.
2. Verify each system note against official service-provider sources.
3. Separate technical service availability from published aviation procedure availability.
4. Deepen Asia-Pacific comparator evidence for ASEAN planning.
5. Add candidate notes for KASS, SouthPAN, SDCM, and ASECNA only after source scaffolds exist.

## See also

- [[SBAS MOC]]
- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS-vs-Other-Augmentation-Methods]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[ASEAN SBAS Source Backlog]]
