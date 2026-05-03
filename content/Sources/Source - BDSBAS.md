---
title: Source - BDSBAS
description: Institutional source note for BeiDou Satellite-Based Augmentation System official ICD and technical-public signals, with strict boundaries for BDSBAS signal-interface and aviation-service claims
tags: [source, bdsbas, beidou, china, sbas, aviation, service-provider]
source_type: signal-interface-and-technical-public-material
status: active
verification_status: official-bdsbas-icd-extracted-with-secondary-technical-context
created: 2026-05-03
modified: 2026-05-03
primary_sources:
  - China Satellite Navigation Office BDSBAS-B1C Signal In Space Interface Control Document Version 1.0, July 2020
  - NAVIGATION journal Development of BeiDou Satellite-Based Augmentation System, 2021
---

# Source - BDSBAS

## Scope of this note

This note is the BDSBAS child source note for the SBAS service-provider family. It records official China Satellite Navigation Office BDSBAS-B1C Signal-In-Space Interface Control Document signals and bounded technical-public context from a 2021 NAVIGATION journal article.

This note is deliberately conservative. The official ICD can anchor signal-interface, PRN, timing, coordinate, and message-structure claims. It does not by itself prove current civil-aviation operational approval, airport procedure availability, APV-I service declaration, or regulator authorization.

Use [[Source - SBAS Service Providers]] for cross-system routing. Use [[Source - ICAO Annex 10 Volume I GNSS SBAS]] for ICAO SARPs routing and [[Source - RTCA DO-229]] for MOPS routing.

## Official source identity

| Field                      | Extracted signal                                                                                                                              |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| System                     | BeiDou Satellite-Based Augmentation System (BDSBAS)                                                                                           |
| Official source            | BDSBAS-B1C Signal In Space Interface Control Document, Version 1.0                                                                            |
| Document identifier        | BDS-SIS-ICD-BDSBAS-B1C-1.0                                                                                                                    |
| Issuing authority          | China Satellite Navigation Office                                                                                                             |
| Publication date           | July 2020                                                                                                                                     |
| Safe source role           | BDSBAS-B1C signal characteristics, GEO PRN assignments, BDSBAS network time and coordinate reference signals, and message-interface structure |
| Secondary technical source | Liu et al., Development of BeiDou Satellite-Based Augmentation System, NAVIGATION, 2021                                                       |

## Extracted official BDSBAS ICD signals

The China Satellite Navigation Office ICD states that the BeiDou Satellite Based Augmentation System is an important part of BDS and provides Single Frequency service through BDSBAS-B1C. The extracted source says the BDSBAS-B1C signal is provided in accordance with ICAO SARPs, Annex 10, Volume I.

The ICD identifies future DFMC service using BDSBAS-B2a. The future-service statement should be treated as an interface/roadmap signal, not as proof of operational aviation service availability.

The ICD gives these space-segment and interface signals:

| Field                                     | Extracted official ICD signal                                                                                                             |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| GEO orbital slots                         | 80 degrees E, 110.5 degrees E, and 140 degrees E                                                                                          |
| GEO PRNs                                  | PRN 144 at 80 degrees E; PRN 143 at 110.5 degrees E; PRN 130 at 140 degrees E                                                             |
| B1C carrier frequency                     | 1575.42 MHz                                                                                                                               |
| Signal modulation                         | BPSK(1) with 1023-bit PRN code and 500 symbols per second after rate 1/2 convolutional encoding                                           |
| Message size                              | 250-bit messages broadcast in 1 second                                                                                                    |
| Time reference                            | BeiDou Navigation Satellite System Time (BDT); BDSBAS Network Time equals BDT plus 14 seconds for SF service in the extracted ICD context |
| Coordinate reference in extracted summary | WGS-84 in the ICD summary extracted during this cycle                                                                                     |

## Extracted secondary technical-public context

The 2021 NAVIGATION article states that China is developing BDSBAS in accordance with international standards and had provided initial Single Frequency and DFMC services since July 2020. It states that BDSBAS augments GNSS services for aviation and other applications in China and surrounding areas.

The article reports that BDSBAS began broadcasting signals on 2018-11-09 and that BDS was formally commissioned on 2020-07-31. It describes BDSBAS as targeting APV-I capability for Single Frequency service and CAT-I precision approach capability for DFMC service, while also noting civil-aviation testing and certification steps.

Because this is a technical journal article rather than a civil-aviation regulator service declaration, those statements should be used as development/status context, not as final operational approval evidence.

## What this source can currently anchor

This note can currently anchor these BDSBAS-specific statements:

- BDSBAS is the BeiDou Satellite-Based Augmentation System and part of the BeiDou system context.
- The official BDSBAS-B1C ICD defines a Single Frequency BDSBAS service signal and interface characteristics.
- The official ICD identifies GEO orbital slots and PRN assignments for BDSBAS-B1C: PRNs 144, 143, and 130.
- The official ICD provides signal, timing, and message-interface details for BDSBAS-B1C.
- The NAVIGATION article can support bounded technical-development context for SF/DFMC development and APV-I/CAT-I targets, but not final operational approval.

## What this source must not be used for yet

Do not use this note alone to publish:

- current BDSBAS aviation operational-service declaration;
- CAAC procedure publication, airport/runway availability, or approach minima;
- exact current coverage boundaries or service-volume commitments;
- claims that BDSBAS currently supports APV-I or CAT-I operational approaches unless backed by later CAAC/official aviation service material;
- comparative performance or maturity claims against WAAS, EGNOS, MSAS, GAGAN, KASS, or SouthPAN;
- complete ICAO/RTCA compliance conclusions beyond the interface statements in the extracted sources.

## Relationship to other source notes

| Related source note                                    | Role boundary                                                                       |
| ------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| [[Source - SBAS Service Providers]]                    | Family router for service-provider identity and source maturity across SBAS systems |
| [[Source - ICAO Annex 10 Volume I GNSS SBAS]]          | SARPs routing; not a BDSBAS service declaration                                     |
| [[Source - RTCA DO-229]]                               | MOPS/equipment routing; not a BDSBAS provider source                                |
| [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] | APAC implementation-paper routing; not the official BDSBAS ICD                      |

## Downstream pages to connect

- [[BDSBAS]]
- [[KASS]]
- [[MSAS]]
- [[GAGAN]]
- [[Source - SBAS Service Providers]]
- [[SBAS Standards Source Matrix]]
- [[ASEAN SBAS Source Backlog]]
- [[SBAS Source Backlog]]

## Future extraction targets

- CAAC or official Chinese civil-aviation source for operational approval, service declaration, and procedure publication.
- Current BeiDou/CSNO service notices, performance standards, or service-volume definitions.
- Official BDSBAS-B2a/DFMC interface and service-definition material if the DFMC branch enters scope.
- ICAO/ICG presentations only as secondary implementation signals unless they reproduce official source status.

## See also

- [[BDSBAS]]
- [[Source - SBAS Service Providers]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - RTCA DO-229]]
- [[SBAS Standards Source Matrix]]
