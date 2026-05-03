---
title: SBAS Systems by Region MOC
description: Institutional navigation map for regional SBAS implementations, comparators, and source-backed system research
tags: [MOC, regional, sbas, comparison, systems]
category: mocs
created: 2026-04-19
modified: 2026-05-03
version: 2.1
status: reviewed
verification_status: source-routed-with-service-provider-child-notes
---

# SBAS Systems by Region MOC

## Scope

This note maps regional SBAS systems and system-comparison research. It is a navigation and synthesis page, not a certified service-performance table.

Exact system status, coverage, performance, service levels, satellite payloads, procedure publication, and operational approvals must be checked against current service-provider, regulator, standards, and AIP/procedure material before use in formal analysis.

## Primary regional system notes

| System   | Region / role                                              | Current note | Dedicated source note             | Source posture                                                                                                                     |
| -------- | ---------------------------------------------------------- | ------------ | --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| WAAS     | United States / North America reference system             | [[WAAS]]     | [[Source - WAAS]]                 | Official FAA public WAAS material extracted; deeper status/performance/procedure evidence still required                           |
| EGNOS    | Europe reference system                                    | [[EGNOS]]    | [[Source - EGNOS]]                | Official EGNOS SoL SDD material extracted; national authorization/AIP evidence still required                                      |
| MSAS     | Japan / Asia-Pacific comparator                            | [[MSAS]]     | [[Source - MSAS]]                 | Official QZSS and ICAO APAC material extracted; current post-2023 LPV status still bounded                                         |
| GAGAN    | India / low-latitude regional comparator                   | [[GAGAN]]    | [[Source - GAGAN SBAS Operation]] | ICAO APAC ITF/7 and AAI GEO FAQ extracted; exact service performance/procedure minima still bounded                                |
| BDSBAS   | China / BeiDou-linked Asia-Pacific comparator              | [[BDSBAS]]   | [[Source - BDSBAS]]               | Official BDSBAS-B1C ICD extracted; CAAC aviation service/procedure evidence still required                                         |
| KASS     | Republic of Korea / Northeast Asia comparator              | [[KASS]]     | [[Source - KASS]]                 | KARI, ICAO APAC ITF/5, and bounded contractor-public certification signals extracted; Korean regulator/AIP evidence still required |
| SouthPAN | Australia and New Zealand / early Open Services comparator | [[SouthPAN]] | [[Source - SouthPAN]]             | Official GA/LINZ open-service and SIS Open Services material extracted; certified aviation SoL/AIP evidence still required         |

Future source-backed notes may cover SDCM, ASECNA, and other SBAS or SBAS-like programs. Until dedicated notes exist, those systems should be discussed as candidate research targets rather than as completed source-routed pages.

## Comparison and synthesis notes

- [[WAAS vs EGNOS]]
- [[MSAS vs GAGAN]]
- [[Asia-Pacific SBAS Implementation Patterns]]
- [[Japan MSAS GBAS Lessons for ASEAN SBAS]]
- [[GIPTA 2.0 and ASEAN SBAS Implementation Pathway]]

## ASEAN relevance

ASEAN does not currently appear in this knowledge base as a single deployed regional SBAS equivalent to WAAS or EGNOS. The ASEAN branch is instead an implementation-planning branch focused on readiness, governance, barriers, demand, source evidence, and service-model choice.

The system notes above should be used as bounded comparator evidence only. Do not transfer operational claims from WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, or SouthPAN into ASEAN planning without ASEAN-specific institutional, service-model, regulator, and implementation evidence.

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
| Source maturity          | Prevents unsourced comparisons between systems with unequal evidence depth    |

## Source posture

The current major-system layer now has first-layer dedicated source notes for WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, and SouthPAN.

That does not mean the systems are fully verified for operational use. Priority source families still include:

- service-provider definition documents and performance reports;
- regulator and ANSP operational approval material;
- AIP/procedure publications for airport/runway-specific claims;
- ICAO APAC and regional planning documents;
- RTCA/EUROCAE/ICAO standards scaffolds in [[SBAS Source Backlog]];
- ASEAN and GIPTA-specific source stacks in [[ASEAN SBAS Source Backlog]] and [[GIPTA 2.0 MOC]].

## Research priorities

1. Deepen service-provider source notes with performance, service-volume, and status documents where official public sources exist.
2. Verify each operational procedure claim against regulator/ANSP/AIP sources.
3. Separate technical service availability from published aviation procedure availability.
4. Deepen Asia-Pacific comparator evidence for ASEAN planning.
5. Add candidate notes for SDCM and ASECNA only after source scaffolds exist.

## See also

- [[SBAS MOC]]
- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS-vs-Other-Augmentation-Methods]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[ASEAN SBAS Source Backlog]]
- [[Source - SBAS Service Providers]]
