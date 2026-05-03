---
title: Research Log - 2026-05-03 - Service Provider Child Source Completion
description: Work log for the five-cycle SBAS service-provider source-hardening pass covering WAAS, EGNOS, KASS, BDSBAS, and service-provider routing updates
tags: [research-log, source-hardening, sbas, service-provider, waas, egnos, kass, bdsbas]
created: 2026-05-03
modified: 2026-05-03
status: complete
verification_status: qa-pending-at-creation
---

# Research Log - 2026-05-03 - Service Provider Child Source Completion

## Scope

This cycle completed a first-layer service-provider child-source pass for four remaining high-value SBAS systems and updated the family routing layer.

The pass followed the institutional rule that system pages must not duplicate source-note detail. Each system page now states only source-routed system meaning and directs detailed evidence to the applicable child source note.

## Source notes created

| Source note         | Primary source material used                                                                      | Safe current role                                                                                    | Boundary retained                                                                                     |
| ------------------- | ------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| [[Source - WAAS]]   | FAA WAAS public page and FAA August 2025 WAAS quick-facts PDF                                     | WAAS identity, FAA broad aviation-service signal, FAA LP/LPV public count snapshots                  | No real-time status, service-volume, aircraft/operator authorization, or runway minima claims         |
| [[Source - EGNOS]]  | Official EGNOS Safety of Life SDD page and in-force Issue 3.6 PDF                                 | EGNOS SoL aviation-service definition, public/free access signal, APV-I/CAT-I service-intent context | No country-specific authorization, AIP, receiver approval, or live performance claims                 |
| [[Source - KASS]]   | KARI KASS page, ICAO APAC ITF/5 IP/09, and bounded Thales Alenia Space certification announcement | KASS identity, governance, architecture, PRN/Service Provider ID, APAC implementation context        | No Korean runway/procedure, AIP minima, second-GEO current status, or final regulator approval claims |
| [[Source - BDSBAS]] | China Satellite Navigation Office BDSBAS-B1C ICD and bounded NAVIGATION 2021 technical context    | BDSBAS identity, official B1C signal-interface, GEO PRN, timing/message-interface signals            | No CAAC aviation service declaration, APV/CAT operational availability, or procedure claims           |

## System pages hardened

- [[WAAS]] now routes official FAA evidence to [[Source - WAAS]].
- [[EGNOS]] now routes official EGNOS SoL SDD evidence to [[Source - EGNOS]].
- [[KASS]] now routes KARI/ICAO APAC evidence to [[Source - KASS]].
- [[BDSBAS]] now routes official ICD evidence to [[Source - BDSBAS]].

## Routing and synthesis pages updated

- [[Source - SBAS Service Providers]] now treats the current major-system set as first-layer child-source covered.
- [[SBAS Source Backlog]] now shifts remaining service-provider work from child-source creation to deeper regulator/AIP/performance extraction.
- [[ASEAN SBAS Source Backlog]] now records WAAS, EGNOS, KASS, and BDSBAS as bounded comparator source anchors.
- [[SBAS Standards Source Matrix]] now routes the full child-source set and keeps comparative performance tables prohibited.
- [[SBAS-Systems-by-Region-MOC]] now lists system notes with source posture and dedicated source-note anchors.
- [[WAAS vs EGNOS]] was rewritten as a source-posture comparison rather than a performance ranking.
- [[Asia-Pacific SBAS Implementation Patterns]] was rewritten as bounded comparator synthesis for ASEAN planning.

## Non-overlap decisions

- Detailed FAA LPV/LP counts remain in [[Source - WAAS]], not duplicated into [[WAAS]] or [[WAAS vs EGNOS]].
- Detailed EGNOS SDD signals remain in [[Source - EGNOS]], not duplicated into [[EGNOS]].
- KASS architecture and PRN/Service Provider ID details remain in [[Source - KASS]], not duplicated into [[KASS]].
- BDSBAS PRN, signal, timing, and message-interface details remain in [[Source - BDSBAS]], not duplicated into [[BDSBAS]].
- Comparative performance remains prohibited until equivalent official evidence exists across compared systems.

## Next source-hardening priorities

1. Regulator/AIP/procedure extraction for operational procedure availability.
2. Performance/service-volume reports for each provider before any comparison matrix.
3. ICAO APAC ITF full-meeting extraction for ASEAN governance and APAC coordination evidence.
4. SDCM and ASECNA source scaffolds only if they enter scope and official public sources are available.

## QA status

QA is performed after this log is created as part of the same cycle. Required gates:

- Prettier formatting.
- `npm run check`.
- Quartz build.
- Wikilink audit.
- Publication/privacy audit.
- Markdown table audit.
- Commit, push, and live verification.
