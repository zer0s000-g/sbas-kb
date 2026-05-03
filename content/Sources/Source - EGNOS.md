---
title: Source - EGNOS
description: Institutional source note for official EGNOS Safety of Life Service Definition material, used to route EGNOS aviation-service claims without substituting for ETSO, procedure-design, AIP, or national operational-approval sources
tags: [source, egnos, euspa, europe, sbas, aviation, service-provider]
source_type: service-definition-document
status: active
verification_status: official-egnos-sol-sdd-extracted
created: 2026-05-03
modified: 2026-05-03
primary_sources:
  - EGNOS Safety of Life Service Definition Document page
  - EGNOS Safety of Life for Aviation Service Definition Document, Issue 3.6, 2024-09-09
---

# Source - EGNOS

## Scope of this note

This note is the EGNOS child source note for the SBAS service-provider family. It records official EGNOS/EUSPA public signals for the EGNOS Safety of Life Service for Aviation and clearly separates those service-definition signals from equipment approval, procedure design, national AIP publication, and operational authorization.

Use this note for EGNOS-specific service-provider and Safety-of-Life service-definition claims. Use [[Source - SBAS Service Providers]] for cross-system routing. Use [[Source - EASA ETSO-C145e and ETSO-C146e]] for article-approval routing and [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] for procedure-design routing.

## Official source identity

| Field                                            | Extracted signal                                                                                                     |
| ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------- |
| System                                           | European Geostationary Navigation Overlay Service (EGNOS)                                                            |
| Service document                                 | EGNOS Safety of Life Service Definition Document                                                                     |
| Published version signal                         | Version 03-06 / Issue 3.6, published 2024-09-09, status In Force                                                     |
| Source owner/context                             | European Union / EUSPA public EGNOS user-support material                                                            |
| Service provider signal in extracted PDF summary | ESSP SAS identified as certified ANSP under the Single European Sky context                                          |
| Segment                                          | Aviation                                                                                                             |
| Safe source role                                 | EGNOS SoL service scope, public access model, APV-I/CAT-I service intent, architecture/service-definition boundaries |

## Extracted official EGNOS signals

The EGNOS Safety of Life Service Definition Document page states that EGNOS augments GPS L1 C/A by providing correction data and integrity information for improving positioning, navigation, and timing services over Europe, with future GPS/Galileo L1/L5 augmentation planned.

The same official page states that the EGNOS Safety of Life Service for Aviation is openly provided, freely accessible without direct charge, and tailored to safety-critical aviation applications.

The official page states that the service is compliant with aviation requirements for APV-I and Category I precision approaches as defined by ICAO Annex 10. It also states that operational use may require specific authorization by relevant authorities.

The service-document page describes the SDD's purpose as giving information on the EGNOS SoL Service for Aviation, including system architecture, Signal-In-Space characteristics, performance achieved, and technical/organizational framework.

The extracted PDF summary reports these additional service-definition signals:

| Official/public signal   | Extracted value or boundary                                                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Service commitment scope | Provision of augmentation signal to GPS SPS with committed performance subject to SDD limitations and disclaimers                                             |
| Intended users           | Aviation users with EGNOS-certified receivers and organizations implementing EGNOS-based procedures, subject to competent authority approval where applicable |
| Service lifetime signal  | Intended minimum 20-year provision from first declaration date, with 6 years advance notice for significant service changes                                   |
| SoL declaration history  | NPA/APV-I declared 2 March 2011; LPV-200 declared September 2015 in SDD v3.0 context                                                                          |
| Service separation       | ESMAS, Open Service, and EDAS are outside this aviation SoL SDD and are described in separate SDDs                                                            |

## What this source can currently anchor

This note can currently anchor these EGNOS-specific statements:

- EGNOS is Europe's SBAS and provides an aviation Safety of Life service definition through official EGNOS/EUSPA material.
- The EGNOS SoL Service for Aviation is described as openly provided and freely accessible without direct charge.
- Official EGNOS material describes the SoL service as tailored for safety-critical aviation applications and compliant with APV-I and Category I precision-approach requirements as defined by ICAO Annex 10.
- Official EGNOS material states that operational use may require authorization by relevant authorities.
- The 2024 in-force SDD page can anchor version/status metadata for the EGNOS SoL Service Definition Document.

## What this source must not be used for yet

Do not use this note alone to publish:

- country-specific authorization, AIP publication, runway minima, or operator approval;
- EASA ETSO or receiver certification requirements;
- procedure-design requirements for LPV, LPV-200, or APV-I;
- exact real-time availability or continuity values outside the extracted SDD context;
- EGNOS superiority or interoperability claims not directly supported by official cross-provider material;
- EGNOS Open Service, EDAS, or maritime ESMAS claims beyond the fact that those services are separate SDD families.

## Relationship to other source notes

| Related source note                                         | Role boundary                                                                       |
| ----------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| [[Source - SBAS Service Providers]]                         | Family router for service-provider identity and source maturity across SBAS systems |
| [[Source - EASA ETSO-C145e and ETSO-C146e]]                 | EASA article-approval routing; not a service-definition source                      |
| [[Source - ICAO Annex 10 Volume I GNSS SBAS]]               | SARPs routing for ICAO requirements; not an EGNOS operating-service page            |
| [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] | Procedure-design routing; not an EGNOS service-commitment source                    |

## Downstream pages to connect

- [[EGNOS]]
- [[WAAS]]
- [[WAAS vs EGNOS]]
- [[Source - SBAS Service Providers]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]

## Future extraction targets

- Direct extraction of the full current EGNOS SoL SDD sections on service area, committed performance, limitations, and receiver/user obligations.
- EASA/ANSP/national AIP sources for country/runway-specific use.
- EGNOS Open Service, EDAS, and ESMAS SDDs only if those non-aviation service families enter the KB scope.
- Official EUSPA/ESSP service notices or performance reports for status/performance claims.

## See also

- [[EGNOS]]
- [[Source - SBAS Service Providers]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[SBAS Standards Source Matrix]]
