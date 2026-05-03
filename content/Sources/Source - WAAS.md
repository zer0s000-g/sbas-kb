---
title: Source - WAAS
description: Institutional source note for official FAA Wide Area Augmentation System public material, used to route WAAS identity, aviation-service, and LP/LPV procedure-count signals without substituting for MOPS, TSO, AIP, or aircraft-approval sources
tags: [source, waas, faa, sbas, aviation, service-provider]
source_type: service-provider-material
status: active
verification_status: official-faa-public-material-extracted
created: 2026-05-03
modified: 2026-05-03
primary_sources:
  - FAA Satellite Navigation - Wide Area Augmentation System page
  - FAA Wide Area Augmentation System quick facts PDF dated August 2025
---

# Source - WAAS

## Scope of this note

This note is the WAAS child source note for the SBAS service-provider family. It is intentionally narrow: it records official FAA public signals for WAAS identity, broad aviation-service role, and FAA-published LP/LPV procedure-count context.

Use this note for WAAS-specific service-provider claims. Use [[Source - SBAS Service Providers]] for cross-system routing. Use [[Source - RTCA DO-229]] and [[Source - FAA TSO-C145e and TSO-C146e]] for equipment/MOPS/article-approval claims.

This note must not become a comparative WAAS performance page. Comparative availability, integrity, or superiority claims require matched official service-provider reports across systems.

## Official source identity

| Field                       | Extracted signal                                                                                                              |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| System                      | Wide Area Augmentation System (WAAS)                                                                                          |
| Issuing/operating authority | Federal Aviation Administration (FAA), U.S. Department of Transportation                                                      |
| Source family               | Official FAA public WAAS service and quick-facts material                                                                     |
| Primary official page       | FAA Satellite Navigation - Wide Area Augmentation System                                                                      |
| Supporting FAA document     | FAA Wide Area Augmentation System quick facts PDF, dated August 2025 in the extracted public file                             |
| Safe source role            | WAAS identity, broad aviation-service role, FAA LP/LPV public procedure-count signals, and FAA-described operational benefits |

## Extracted public FAA signals

The FAA WAAS page states that WAAS is an accurate navigation system developed for civil aviation and that, before WAAS, the U.S. National Airspace System did not have a way to provide horizontal and vertical navigation for approach operations for all users at all locations.

The same FAA page states that WAAS provides service for all classes of aircraft in all phases of flight, including en-route navigation, airport departures, and airport arrivals, and includes vertically guided landing approaches in instrument meteorological conditions at qualified locations throughout the NAS.

The FAA quick-facts PDF describes WAAS as increasing the accuracy, integrity, and availability of GPS. It says LPV procedures take advantage of WAAS accuracy to provide an instrument approach procedure equivalent to a Category I ILS approach in operational form, with minima as low as 200 feet at qualifying airports.

The extracted August 2025 FAA quick-facts text reports:

| FAA public signal               | Extracted value or wording                                                                                                                                    |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| LPV runway-end access statement | WAAS can support access to over 4,100 runway ends in poor weather conditions with minima as low as 200 feet                                                   |
| LPV count signal                | 4,212 LPVs serving 2,035 airports as of August 8, 2025                                                                                                        |
| Non-ILS airport LPV signal      | 1,271 of the LPV-served airports are non-ILS airports                                                                                                         |
| LP count signal                 | 753 LP procedures serving 544 airports as of August 7, 2025                                                                                                   |
| Non-ILS airport LP signal       | 443 of the LP-served airports are non-ILS airports                                                                                                            |
| Equipment caveat                | Older WAAS receivers certified before TSO-C145b/C146b do not necessarily contain LP capability unless upgraded and documented in the flight manual supplement |

## What this source can currently anchor

This note can currently anchor these WAAS-specific statements:

- WAAS is the FAA/U.S. SBAS implementation for civil aviation.
- FAA public material describes WAAS as supporting all classes of aircraft and all phases of flight in the U.S. NAS context.
- FAA public material explicitly connects WAAS with vertically guided landing approaches at qualified locations.
- FAA public quick-facts material provides public LPV and LP procedure-count snapshots for August 2025.
- FAA quick-facts material includes an equipment caveat for LP capability in older WAAS receivers.

## What this source must not be used for yet

Do not use this note alone to publish:

- exact WAAS service-volume boundaries or real-time availability status;
- operational approval for a particular aircraft, operator, route, runway, or procedure;
- AIP procedure minima beyond the FAA quick-facts examples;
- receiver compliance claims beyond the FAA equipment caveat quoted above;
- comparative claims that WAAS is better, more available, or more mature than another SBAS system;
- ICAO SARPs, RTCA MOPS, or FAA TSO requirements.

## Relationship to other source notes

| Related source note                           | Role boundary                                                                       |
| --------------------------------------------- | ----------------------------------------------------------------------------------- |
| [[Source - SBAS Service Providers]]           | Family router for service-provider identity and source maturity across SBAS systems |
| [[Source - RTCA DO-229]]                      | Equipment MOPS; not a WAAS service-status source                                    |
| [[Source - FAA TSO-C145e and TSO-C146e]]      | FAA article-approval source family; not a WAAS coverage/performance source          |
| [[Source - ICAO Annex 10 Volume I GNSS SBAS]] | ICAO SARPs routing; not a U.S. procedure-count source                               |

## Downstream pages to connect

- [[WAAS]]
- [[EGNOS]]
- [[WAAS vs EGNOS]]
- [[Source - SBAS Service Providers]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]

## Future extraction targets

- FAA WAAS Performance Standard or service-volume material, if publicly accessible.
- FAA real-time WAAS satellite/status pages for carefully bounded status-not-commitment signals.
- FAA Charting/AIP-style procedure sources for runway-specific procedure availability and minima.
- FAA operational guidance for aircraft/operator use, separated from service-provider claims.

## See also

- [[WAAS]]
- [[Source - SBAS Service Providers]]
- [[Source - FAA TSO-C145e and TSO-C146e]]
- [[Source - RTCA DO-229]]
- [[SBAS Standards Source Matrix]]
