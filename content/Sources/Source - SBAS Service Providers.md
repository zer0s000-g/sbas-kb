---
title: Source - SBAS Service Providers
description: Institutional source-family anchor for SBAS service-provider definitions, service commitments, coverage, and system status, with explicit boundaries separating service commitment from equipment MOPS, article approval, procedure design, and operational approval
tags:
  [
    source,
    sbas,
    service-provider,
    waas,
    egnos,
    msas,
    gagan,
    bdsbas,
    kass,
    southpan,
    sdcm,
    coverage,
    availability,
  ]
source_type: service-definition
status: active
verification_status: partial-direct-extraction-for-gagan-msas-southpan-waas-egnos-kass-bdsbas-with-sdcm-development-context
last_service_provider_upgrade: "2026-05-03: dedicated source notes now exist for GAGAN, MSAS, SouthPAN, WAAS, EGNOS, KASS, BDSBAS, and SDCM; SDCM is bounded to GLONASS/IAC plus historical ICAO development-context evidence"
---

# Source - SBAS Service Providers

## Scope of this note

This note is the knowledge base's institutional source-family anchor for SBAS service-provider definitions, service commitments, coverage, and system status.

Service-provider material is distinct from:

- airborne-equipment MOPS (handled by [[Source - RTCA DO-229]]);
- article/equipment approval (handled by [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]]);
- procedure-design material (handled by [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] and [[Source - FAA and EASA Procedure-Design and PBN Material]]);
- ICAO SARPs (handled by [[Source - ICAO Annex 10 Volume I GNSS SBAS]]);
- operational approval, AIP/procedure publication, and crew/operator authorization (covered by regulator/ANSP/AIP material).

This note does **not** provide comparative performance tables, availability percentages, uptime statistics, or coverage maps. Those require official service-provider documents, performance reports, and service definitions.

Important boundary:

- Public service-provider metadata can support system identity, operating agency, service type, and broad scope.
- It cannot support numerical availability figures, coverage boundaries, or comparative performance rankings.
- Use this note for service-provider routing and to keep service-commitment claims separate from equipment, article-approval, and procedure-design claims.

## SBAS service-provider identity signals (public sources)

### WAAS — United States

||| Field | Current public signal |
|||---|---|
||| System | Wide Area Augmentation System (WAAS) |
||| Operating agency | Federal Aviation Administration (FAA), U.S. Department of Transportation |
||| Dedicated source note | [[Source - WAAS]] |
||| Verified extraction status | Official FAA WAAS public page and FAA August 2025 WAAS quick-facts PDF extracted |
||| Core verified signal | FAA public material describes WAAS as serving all classes of aircraft in all phases of flight and supporting vertically guided approaches at qualified NAS locations |
||| Boundary | Real-time status, service-volume limits, aircraft/operator authorization, and runway-specific procedure minima require FAA status/performance/AIP/procedure sources |

### EGNOS — Europe

||| Field | Current public signal |
|||---|---|
||| System | European Geostationary Navigation Overlay Service (EGNOS) |
||| Operating agency | European Union / EUSPA context; ESSP SAS service-provider signal in extracted SDD summary |
||| Dedicated source note | [[Source - EGNOS]] |
||| Verified extraction status | Official EGNOS Safety of Life Service Definition Document page and in-force Issue 3.6 PDF extracted |
||| Core verified signal | Official EGNOS material describes the aviation SoL service as openly provided, freely accessible without direct charge, tailored to safety-critical aviation applications, and compliant with APV-I/CAT-I precision-approach requirements as defined by ICAO Annex 10 |
||| Boundary | Country-specific authorization, AIP procedure publication, receiver approval, Open Service/EDAS/ESMAS claims, and live performance values require separate official sources |

### MSAS — Japan

|| Field | Current public signal |
||---|---|
|| System | MSAS / Michibiki Satellite-based Augmentation Service context |
|| Operating agency | MLIT / JCAB for aviation SBAS signal generation and authorization context; QZSS provides satellite transmission service |
|| Dedicated source note | [[Source - MSAS]] |
|| Verified extraction status | Official QZSS SBAS Transmission Service page and ICAO APAC CNS SG/24 IP15 extracted |
|| Core verified signal | MSAS operated with MTSAT from 27 September 2007 and transitioned to QZS-3/QZSS GEO transmission by March/April 2020 |
|| Boundary | Current post-2023 LPV operational status and airport-specific procedure availability still require later JCAB/MLIT/QZSS/AIP extraction |

### GAGAN — India

|| Field | Current public signal |
||---|---|
|| System | GPS Aided GEO Augmented Navigation (GAGAN) |
|| Operating agency | Airports Authority of India (AAI) and Indian Space Research Organisation (ISRO); DGCA India certification signal in ITF/7 IP05b |
|| Dedicated source note | [[Source - GAGAN SBAS Operation]] |
|| Verified extraction status | ICAO APAC ITF/7 IP05b and AAI public GEO-satellite FAQ extracted |
|| Core verified signal | RNP 0.1 operational certification in 2013 for Indian FIRs; APV I in 2015 for Indian landmass; 23 LPV procedures at 15 airports as of May 2025 |
|| Boundary | Procedure minima, exact service performance, and operational authorization details still require DGCA/AAI/AIP extraction |

### BDSBAS — China

||| Field | Current public signal |
|||---|---|
||| System | BeiDou Satellite-Based Augmentation System (BDSBAS) |
||| Operating agency | China Satellite Navigation Office / BeiDou system context for the official BDSBAS-B1C ICD |
||| Dedicated source note | [[Source - BDSBAS]] |
||| Verified extraction status | Official BDSBAS-B1C Signal In Space Interface Control Document extracted; NAVIGATION 2021 article used only as secondary technical-public context |
||| Core verified signal | Official ICD defines BDSBAS-B1C Single Frequency service signal/interface characteristics and identifies GEO PRNs 144, 143, and 130 |
||| Boundary | Current CAAC aviation operational approval, service declaration, APV/CAT procedure availability, and approach minima remain unverified without aviation-regulator/service-definition sources |

### KASS — South Korea

||| Field | Current public signal |
|||---|---|
||| System | Korea Augmentation Satellite System (KASS) |
||| Operating agency | MOLIT/KARI/KANSC context from KARI and ICAO APAC ITF/5 material |
||| Dedicated source note | [[Source - KASS]] |
||| Verified extraction status | Official KARI KASS page, ICAO APAC ITF/5 IP/09, and bounded contractor-public certification announcement extracted |
||| Core verified signal | ICAO APAC material identifies Service Provider ID 6, PRN 134, MOLIT/KARI/KANSC roles, and GPS L1/APV-I/Incheon FIR planning context; KARI material gives current Korean system/architecture context |
||| Boundary | Korean AIP procedure availability, runway minima, current second-GEO status, and final operational authorization require Korean regulator/provider/AIP extraction |

### SouthPAN — Australia and New Zealand

||| Field | Current public signal |
|||---|---|
||| System | Southern Positioning Augmentation Network (SouthPAN) |
||| Operating agency | Geoscience Australia and Toitū Te Whenua Land Information New Zealand |
||| Dedicated source note | [[Source - SouthPAN]] |
||| Verified extraction status | Official SouthPAN FAQ, early Open Services factsheet, and Signal-In-Space Open Services service-definition document extracted |
||| Core verified signal | Early Open Services available since September 2022; service families L1 SBAS, DFMC SBAS, PVS, and Data Access Services; PRN 122; Safety-of-Life aviation service target 2028 |
||| Boundary | Early Open Services are not certified aviation Safety-of-Life services; LPV/procedure/approval claims require later certified-service and AIP/regulator extraction |

### SDCM — Russia / GLONASS augmentation context

||| Field | Current public signal |
|||---|---|
||| System | System of Differential Corrections and Monitoring (SDCM) |
||| Operating agency / source family | Russian / GLONASS institutional context from GLONASS IAC and historical ICAO material |
||| Dedicated source note | [[Source - SDCM]] |
||| Verified extraction status | GLONASS IAC system-documents page, GLONASS OS PS Edition 2.2, ICAO A37-WP/195, and bounded public comparator material reviewed |
||| Core verified signal | GLONASS OS PS material places SDCM in GLONASS-based-system certification context; ICAO A37-WP/195 identifies SDCM as a GLONASS SBAS development path |
||| Boundary | Current aviation operational service, AIP procedure availability, service-volume commitments, and performance status remain unverified without current Russian service-provider/regulator/AIP evidence |

## What this source-family can currently anchor

Until direct extraction from official service-provider documents is performed, this note can support broad routing statements such as:

- Each SBAS system has a distinct operating agency, service area, and service-delivery model.
- Service commitments, coverage, availability, and system status are provider-specific and must be verified against official service-provider documents.
- Comparative performance claims across SBAS systems require verified service-provider data, not assumptions from equipment standards or generic SBAS concept pages.

## What this source-family must not be used for yet

Do not use this note alone to publish:

- comparative availability or uptime statistics across SBAS systems;
- exact coverage boundaries or service-area maps;
- numerical positioning accuracy or integrity performance figures;
- any claim that one SBAS system is superior to another without verified comparative data;
- interoperability claims without official bilateral/multilateral service-provider agreements.

## Relationship to other source notes in this knowledge base

| Claim type              | Equipment source         | Service-provider source          | Procedure-design source                                     | Article-approval source                                                                |
| ----------------------- | ------------------------ | -------------------------------- | ----------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| SBAS system identity    | —                        | This note                        | —                                                           | —                                                                                      |
| SBAS coverage           | —                        | This note (needs extraction)     | —                                                           | —                                                                                      |
| SBAS availability       | —                        | This note (needs extraction)     | —                                                           | —                                                                                      |
| Airborne SBAS equipment | [[Source - RTCA DO-229]] | —                                | —                                                           | [[Source - FAA TSO-C145e and TSO-C146e]] / [[Source - EASA ETSO-C145e and ETSO-C146e]] |
| LPV procedure           | —                        | This note (service availability) | [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] | —                                                                                      |
| Operational approval    | —                        | —                                | [[Source - FAA and EASA Procedure-Design and PBN Material]] | Regulator-specific                                                                     |

## Downstream pages to connect

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[WAAS]]
- [[EGNOS]]
- [[MSAS]]
- [[GAGAN]]
- [[BDSBAS]]
- [[KASS]]
- [[SouthPAN]]
- [[SDCM]]
- [[Source - WAAS]]
- [[Source - EGNOS]]
- [[Source - BDSBAS]]
- [[Source - KASS]]
- [[Source - SDCM]]
- [[SBAS Operational Validation Dashboard]]
- [[WAAS vs EGNOS]]
- [[MSAS vs GAGAN]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS in Civil Aviation MOC]]

## Extraction template for future direct-source cycles

### WAAS required

- [ ] Direct-text extraction of FAA WAAS service definition and scope
- [ ] Real-time status page signals for availability claims
- [ ] Cross-check against [[Source - FAA TSO-C145e and TSO-C146e]] for FAA-specific SBAS context

### EGNOS required

- [ ] Direct-text extraction of EUSPA/ESA EGNOS service definition
- [ ] Safety of Life service declaration and certification basis
- [ ] Cross-check against [[Source - EASA ETSO-C145e and ETSO-C146e]] for EASA-specific SBAS context

### Other systems required

- [x] WAAS: FAA WAAS public page and FAA August 2025 quick-facts PDF extracted into [[Source - WAAS]]; real-time status, service-volume boundaries, runway-specific procedure availability, and operational authorization still require FAA status/performance/AIP/procedure sources.
- [x] EGNOS: official EGNOS Safety of Life Service Definition Document page and Issue 3.6 PDF extracted into [[Source - EGNOS]]; country-specific authorization, AIP publication, and live performance/status evidence still require additional EGNOS/ANSP/regulator sources.
- [x] MSAS: QZSS service page and ICAO APAC CNS SG/24 IP15 extracted into [[Source - MSAS]]; current post-2023 LPV operational status still needs later JCAB/MLIT/QZSS/AIP extraction.
- [x] GAGAN: ICAO APAC ITF/7 IP05b and AAI GEO-satellite FAQ extracted into [[Source - GAGAN SBAS Operation]]; exact service performance and procedure minima still need DGCA/AAI/AIP extraction.
- [x] BDSBAS: official BDSBAS-B1C ICD extracted into [[Source - BDSBAS]]; CAAC/service-declaration/procedure evidence still required before aviation-operational claims.
- [x] KASS: KARI official page, ICAO APAC ITF/5 IP/09, and bounded contractor-public certification material extracted into [[Source - KASS]]; Korean regulator/AIP/service-performance sources still required before runway/procedure operational claims.
- [x] SouthPAN: Geoscience Australia/LINZ open-service and Signal-In-Space service-definition material extracted into [[Source - SouthPAN]]; certified Safety-of-Life/AIP material still required before aviation-operational claims.
- [x] SDCM: GLONASS IAC system-documents page, GLONASS OS PS Edition 2.2, ICAO A37-WP/195, and bounded public comparator material reviewed into [[Source - SDCM]]; current Russian SDCM service-definition, regulator/AIP, and performance evidence still required before operational aviation claims.
