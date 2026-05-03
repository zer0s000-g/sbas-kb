---
title: KASS
description: Source-routed system note for the Korea Augmentation Satellite System, grounded in official KARI and ICAO APAC material with explicit boundaries for Korean aviation procedure and operational-approval claims
tags: [system, kass, sbas, aviation, regional-system, korea]
created: 2026-05-03
modified: 2026-05-03
status: reviewed
verification_status: source-routed-to-official-kari-icao-apac-material
---

# KASS

## Scope status

This page is a source-routed system note for KASS, the Korea Augmentation Satellite System.

The verified KASS-specific claims on this page route to [[Source - KASS]]. Cross-system provider context routes to [[Source - SBAS Service Providers]]. Standards, MOPS, and procedure-design questions remain separated through the source matrix.

Boundary:

- This page does not publish airport/runway-specific Korean APV/LPV procedure availability.
- This page does not publish Korean AIP minima or aircraft/operator authorization.
- This page does not treat contractor-public status announcements as a substitute for regulator/AIP evidence.

## Working definition

KASS is the Republic of Korea's satellite-based augmentation implementation. Official KARI material describes KASS as Korea's independent SBAS, developed under the Ministry of Land, Infrastructure and Transport with KARI as project manager, to correct GPS signal errors and provide high-reliability location services across the Korean peninsula.

## Official source signals

| Signal type                     | Current authenticated source-routed statement                                                                                                                                                         |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| System identity                 | Korea Augmentation Satellite System (KASS); routed to [[Source - KASS]]                                                                                                                               |
| Government/program context      | ICAO APAC ITF/5 IP/09 describes KASS as a MOLIT-led Korean SBAS program                                                                                                                               |
| KARI role                       | KARI public material describes KARI's project/management role and KASS operation context                                                                                                              |
| Architecture signal             | KARI and ICAO APAC material identify reference, processing, control, uplink, and GEO segments; details are kept in [[Source - KASS]]                                                                  |
| ICAO APAC implementation signal | ITF/5 IP/09 reports Service Provider ID 6, PRN 134, GPS L1 augmentation, and APV-I/Incheon FIR planning context                                                                                       |
| Operational-status boundary     | Thales Alenia Space announced national certification and operational service in January 2024; use this only as bounded contractor-public status context unless Korean regulator/AIP evidence is added |

## Relationship to civil aviation use

KASS matters in this KB because it is a Northeast Asian SBAS implementation with official APAC implementation-paper signals. It is relevant to:

- APAC regional implementation patterns in [[Source - ICAO APAC GBAS-SBAS Implementation Forums]];
- service-provider family maturity in [[Source - SBAS Service Providers]];
- standards/source routing in [[SBAS Standards Source Matrix]];
- ASEAN comparator analysis in [[ASEAN SBAS Source Backlog]].

## Claims intentionally not duplicated here

To prevent overlapping knowledge, this page does not copy KASS PRN, architecture, or roadmap detail from the source note. Those details belong in [[Source - KASS]]. This page only states the system-level meaning and routes readers to the authenticated source layer.

## Source anchors

- [[Source - KASS]] -- dedicated KASS child source note for KARI, ICAO APAC, and bounded contractor-public signals.
- [[Source - SBAS Service Providers]] -- service-provider family router for system identity and source-maturity tracking.
- [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] -- APAC implementation-paper source family.
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]] -- ICAO SARPs routing.
- [[SBAS Standards Source Matrix]] -- claim-routing matrix for standards/source families.

## Open verification questions

- Which MOLIT/Korean aviation authority page is the best canonical source for KASS certification and service declaration?
- Which Korean AIP/procedure source should be used for runway-specific APV/LPV availability?
- What is the official current status of Koreasat-6A SBAS payload/service continuity after the 2023 ICAO APAC roadmap?

## See also

- [[Source - KASS]]
- [[Source - SBAS Service Providers]]
- [[Source - ICAO APAC GBAS-SBAS Implementation Forums]]
- [[MSAS]]
- [[BDSBAS]]
- [[GAGAN]]
- [[SouthPAN]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS Source Backlog]]
