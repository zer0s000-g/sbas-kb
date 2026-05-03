---
title: Asia-Pacific SBAS Implementation Patterns
description: Source-routed synthesis note comparing Asia-Pacific SBAS implementation patterns with explicit boundaries around comparator transferability for ASEAN planning
tags: [synthesis, sbas, asia-pacific, msas, gagan, bdsbas, kass, southpan, regional-systems]
created: 2026-04-23
modified: 2026-05-03
status: reviewed
verification_status: source-routed-comparator-synthesis
---

# Asia-Pacific SBAS Implementation Patterns

## Scope status

This is a source-routed synthesis note for Asia-Pacific SBAS implementation patterns. It uses system-specific source notes as bounded comparator evidence; it does not claim that one system's operational model, coverage, or approval status transfers to ASEAN.

Boundary:

- It does not verify current airport/runway procedure availability across the region.
- It does not compare service performance numerically.
- It does not infer ASEAN feasibility from neighboring systems without ASEAN-specific evidence.

## Why this note exists

The KB now has a stronger first-layer source backbone for several Asia-Pacific or Asia-Pacific-relevant SBAS systems:

| System       | Source-routed comparator role                                                                    | Dedicated source note             |
| ------------ | ------------------------------------------------------------------------------------------------ | --------------------------------- |
| [[MSAS]]     | Japan/QZSS SBAS transmission-service and APAC implementation comparator                          | [[Source - MSAS]]                 |
| [[GAGAN]]    | India low-latitude/equatorial-adjacent implementation comparator                                 | [[Source - GAGAN SBAS Operation]] |
| [[SouthPAN]] | Australia/New Zealand early Open Services and future aviation SoL comparator                     | [[Source - SouthPAN]]             |
| [[KASS]]     | Republic of Korea SBAS governance/certification/architecture comparator                          | [[Source - KASS]]                 |
| [[BDSBAS]]   | China/BeiDou signal-interface and development-context comparator                                 | [[Source - BDSBAS]]               |
| [[SDCM]]     | Russian/GLONASS augmentation research target with historical ICAO and GLONASS-IAC source posture | [[Source - SDCM]]                 |

## Current source-routed pattern

| Pattern                                                           | Supported by                                                                                                        | Safe interpretation                                                                                                          |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| State or regional service-provider ownership differs by system    | [[Source - MSAS]], [[Source - GAGAN SBAS Operation]], [[Source - SouthPAN]], [[Source - KASS]], [[Source - BDSBAS]] | Governance model is system-specific and must not be generalized                                                              |
| APAC implementation forums provide regional signals               | [[Source - ICAO APAC GBAS-SBAS Implementation Forums]]                                                              | ICAO APAC papers can support regional coordination signals, not national operational approval                                |
| Low-latitude/ionospheric context matters                          | [[Source - GAGAN SBAS Operation]] and [[Source - SouthPAN]] as bounded comparators                                  | These are comparator signals, not direct ASEAN feasibility proof                                                             |
| Signal-interface maturity is not the same as operational approval | [[Source - BDSBAS]]                                                                                                 | An ICD can support interface claims without proving aviation procedure availability                                          |
| Development-context evidence is not current operational approval  | [[Source - SDCM]]                                                                                                   | Historical ICAO and GLONASS/IAC evidence can identify the system and source family, but not current aviation operational use |
| Certification/status announcements require source typing          | [[Source - KASS]]                                                                                                   | Contractor-public and official provider signals need regulator/AIP follow-up before operational claims                       |

## ASEAN relevance

Asia-Pacific systems are useful for ASEAN planning only when treated as bounded evidence:

- GAGAN can inform questions about low-latitude infrastructure, ionosphere monitoring, and regional implementation sequencing, but does not prove ASEAN service feasibility.
- SouthPAN can inform service-definition and staged-service thinking, but its Australian/New Zealand context does not transfer directly to Southeast Asia.
- MSAS and KASS can inform Northeast Asian institutional and technical implementation comparisons, but not ASEAN procedure availability.
- BDSBAS can inform BeiDou/SBAS signal-interface and China-centered development context, but not CAAC or ASEAN operational approval without further sources.
- SDCM can inform GLONASS augmentation/source-family awareness, but its current KB evidence is development-context and GLONASS-system-posture evidence rather than operational aviation-service evidence.

## What remains uncertain

- Which APAC systems have current, official, public aviation procedure inventories suitable for comparison.
- Which service-definition/performance reports are sufficiently equivalent to support a regional matrix.
- Which ASEAN states have institutional evidence for adopting, hosting, using, or coordinating an SBAS service.
- How equatorial ionospheric behavior should be sourced for ASEAN-specific feasibility rather than inferred from adjacent systems.

## Best next support targets

- Full extraction of [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] across ITF meetings and working papers.
- [[Source - Equatorial Ionosphere and SBAS Feasibility]] with technical literature and implementation-study evidence.
- Regulator/AIP extraction for operational procedure claims in Japan, India, Korea, China, Australia/New Zealand, Russia/SDCM if aviation use is claimed, and any ASEAN state under study.
- [[SBAS Operational Validation Dashboard]] as the routing layer for deciding whether a claim has enough evidence to graduate from comparator context to operational aviation status.
- Service-provider performance/service-volume reports for each system before any regional comparison table is attempted.

## See also

- [[MSAS]]
- [[GAGAN]]
- [[SouthPAN]]
- [[KASS]]
- [[BDSBAS]]
- [[Source - MSAS]]
- [[Source - GAGAN SBAS Operation]]
- [[Source - SouthPAN]]
- [[Source - KASS]]
- [[Source - BDSBAS]]
- [[SDCM]]
- [[Source - SDCM]]
- [[SBAS Operational Validation Dashboard]]
- [[ASEAN SBAS Adoption Landscape]]
- [[ASEAN SBAS Readiness Heuristic]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS Source Backlog]]
