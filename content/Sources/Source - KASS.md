---
title: Source - KASS
description: Institutional source note for Korea Augmentation Satellite System official KARI, ICAO APAC, and contractor-public certification signals, with boundaries for KASS aviation-service and architecture claims
tags: [source, kass, kari, molit, korea, sbas, aviation, service-provider]
source_type: service-provider-material
status: active
verification_status: official-kari-icao-apac-material-extracted
created: 2026-05-03
modified: 2026-05-03
primary_sources:
  - KARI Korea Augmentation Satellite System page
  - ICAO APAC GBAS/SBAS ITF/5 IP/09 Korean SBAS KASS Development and Implementation Status
  - Thales Alenia Space public certification and operational-service announcement
---

# Source - KASS

## Scope of this note

This note is the KASS child source note for the SBAS service-provider family. It records official/public KASS identity, governance, architecture, and status signals from KARI and ICAO APAC material, with contractor-public certification context from Thales Alenia Space.

Use this note for KASS-specific system identity, Korean institutional context, and high-level architecture/source-status claims. Do not use it as a substitute for Korean AIP procedure publication, aircraft/operator approval, MOPS, SARPs, or exact service-performance commitments.

## Official source identity

| Field                               | Extracted signal                                                                                                                     |
| ----------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| System                              | Korea Augmentation Satellite System (KASS)                                                                                           |
| State/system context                | Republic of Korea SBAS implementation                                                                                                |
| Government/program authority signal | Ministry of Land, Infrastructure and Transport (MOLIT) in ICAO APAC ITF/5 IP/09                                                      |
| KARI role signal                    | KARI as project manager/official agency context in KARI public material                                                              |
| ICAO APAC source                    | GBAS/SBAS ITF/5 IP/09, Korean SBAS KASS Development and Implementation Status, Tokyo, 21-23 June 2023                                |
| Contractor-public source            | Thales Alenia Space announcement that KASS was certified by Korean national authorities and entered operational service, 2024-01-29  |
| Safe source role                    | KASS identity, Korean governance/architecture signals, SBAS PRN/service-provider identifiers, and bounded operational-status context |

## Extracted KARI public signals

KARI states that Korea developed KASS to correct GPS signal errors and provide high-precision location data. KARI describes KASS as Korea's independent SBAS, developed under MOLIT with KARI as project manager since October 2014.

KARI states that KASS uses geostationary satellites to provide high-precision, high-reliability location services across the Korean peninsula. KARI also states that Korea became the fifth country, after the United States, the European Union, Japan, and India, to operate an SBAS system for aviation.

KARI public material gives a high-level KASS architecture:

| Component                               | KARI public signal                                                                |
| --------------------------------------- | --------------------------------------------------------------------------------- |
| Reference stations                      | 7 domestic locations receive GPS and SBAS signals and extract navigation messages |
| Central processing/integration stations | 2 locations calculate GPS errors and generate correction/integrity data           |
| Satellite communication stations        | 2 locations generate SBAS messages and transmit them to geostationary satellites  |
| Space segment                           | Leased SBAS satellite broadcasting corrected SBAS signals throughout the country  |

KARI also states that KARI was designated in December 2022 as the official agency responsible for managing and operating KASS as a radio navigation safety facility, that a service agreement was signed with the Office of Air Traffic in March 2023, and that KASS was transferred to the government in February 2024 after development and deployment.

## Extracted ICAO APAC ITF/5 signals

ICAO APAC GBAS/SBAS ITF/5 IP/09, presented by the Republic of Korea, states that KASS is a Korean SBAS program led by MOLIT and initiated in October 2014.

The paper states that KASS will comply with ICAO Annex 10 SARPs and the corresponding SBAS MOPS published by RTCA. It also states that KASS initially targets GPS L1 augmentation and APV-I approach services in the Incheon FIR.

The paper gives these governance and architecture signals:

| Field                                         | ICAO APAC ITF/5 extracted signal                                                                    |
| --------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| System owner/operator/certification authority | MOLIT                                                                                               |
| Program management                            | KARI / KPO                                                                                          |
| KASS service provider                         | KANSC, established February 2021 under MOLIT                                                        |
| SBAS Service Provider ID                      | 6, introduced for KASS by ICAO SARPs Amendment 92 in July 2020                                      |
| KASS reference stations                       | 7 KRS                                                                                               |
| Processing stations                           | 2 KPS                                                                                               |
| Control stations                              | 2 KCS                                                                                               |
| Uplink stations                               | 3 KUS at 2 sites                                                                                    |
| First GEO                                     | Measat-3D at 91.5 degrees E, PRN 134, launched 2022                                                 |
| Second GEO roadmap in 2023 paper              | Koreasat-6A planned for H1 2025                                                                     |
| Initial SoL roadmap in 2023 paper             | December 2023 Safety of Life start across Incheon FIR, stated as future roadmap in that 2023 source |

## Extracted contractor-public certification signal

Thales Alenia Space announced on 2024-01-29 that KASS, developed by Thales Alenia Space as prime contractor under contract with KARI for MOLIT, had received official national certification and entered operational service.

Because this is contractor-public material rather than a Korean regulator/AIP source, it can support a bounded certification/status signal but should not be used alone for runway-specific procedure availability or operational authorization.

## What this source can currently anchor

This note can currently anchor these KASS-specific statements:

- KASS is the Republic of Korea's SBAS implementation.
- KARI and ICAO APAC material associate KASS with MOLIT-led Korean SBAS governance.
- ICAO APAC ITF/5 IP/09 provides KASS architecture, PRN 134, Service Provider ID 6, and initial GPS L1/APV-I/Incheon FIR planning signals.
- KARI public material describes KASS management/operation and high-level domestic architecture.
- Contractor-public material supports a bounded statement that KASS was announced as nationally certified and operational in January 2024.

## What this source must not be used for yet

Do not use this note alone to publish:

- KASS runway-specific LPV/APV procedure availability;
- Korean AIP procedure minima or operational authorization;
- exact service-volume, availability, continuity, or integrity-performance values;
- claims that KASS fully meets all Annex 10 or RTCA requirements without direct standards and certification evidence;
- current Koreasat-6A operational status after the 2023 roadmap without later official confirmation;
- comparative claims about KASS versus MSAS, GAGAN, WAAS, EGNOS, BDSBAS, or SouthPAN.

## Relationship to other source notes

| Related source note                                    | Role boundary                                                                                                 |
| ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| [[Source - SBAS Service Providers]]                    | Family router for service-provider identity and source maturity across SBAS systems                           |
| [[Source - ICAO Annex 10 Volume I GNSS SBAS]]          | SARPs routing; not a KASS procedure-status source                                                             |
| [[Source - RTCA DO-229]]                               | SBAS MOPS routing; not a Korean service-provider source                                                       |
| [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] | Regional APAC implementation-paper family; KASS-specific extracted signals are routed here in this child note |

## Downstream pages to connect

- [[KASS]]
- [[MSAS]]
- [[BDSBAS]]
- [[Source - SBAS Service Providers]]
- [[SBAS Standards Source Matrix]]
- [[ASEAN SBAS Source Backlog]]
- [[SBAS Source Backlog]]

## Future extraction targets

- MOLIT/Korean aviation authority public service-definition, certification, or AIP source material.
- Current KASS service notices or performance reports from KANSC/MOLIT/KARI.
- Official confirmation of second-GEO operational status after the 2023 ICAO APAC roadmap.
- Korean AIP/procedure evidence before publishing airport/runway-specific APV/LPV claims.

## See also

- [[KASS]]
- [[Source - SBAS Service Providers]]
- [[Source - ICAO APAC GBAS-SBAS Implementation Forums]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[SBAS Standards Source Matrix]]
