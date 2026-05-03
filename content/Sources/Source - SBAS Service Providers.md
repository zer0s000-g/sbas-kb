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
    bdbsas,
    kass,
    southpan,
    coverage,
    availability,
  ]
source_type: service-definition
status: active
verification_status: public-catalog-reviewed-not-source-extracted
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

| Field              | Current public signal                                                                                                                                 |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| System             | Wide Area Augmentation System (WAAS)                                                                                                                  |
| Operating agency   | Federal Aviation Administration (FAA), U.S. Department of Transportation                                                                              |
| Service type       | SBAS for aviation safety-of-life                                                                                                                      |
| Public source page | https://www.faa.gov/about/office_org/headquarters_offices/ato/service_units/techops/navservices/gnss/waas                                             |
| Scope signal       | "WAAS provides service for all classes of aircraft in all phases of flight — including en-route navigation, airport departures, and airport arrivals" |
| Real-time status   | https://www.nstb.tc.faa.gov/rt_waassatellitestatus.htm                                                                                                |
| Important signal   | WAAS is the U.S. implementation of SBAS; the term "WAAS" appears in FAA TSO and DO-229 scope text as the U.S. SBAS example                            |

### EGNOS — Europe

| Field              | Current public signal                                                                                                                                         |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| System             | European Geostationary Navigation Overlay Service (EGNOS)                                                                                                     |
| Operating agency   | European Union Agency for the Space Programme (EUSPA); developed by European Space Agency (ESA)                                                               |
| Service type       | SBAS for aviation safety-of-life and other applications                                                                                                       |
| Public source page | https://egnos.gsc-europa.eu/egnos-system/about-egnos                                                                                                          |
| Scope signal       | "EGNOS is Europe's regional satellite-based augmentation system (SBAS). It is used to improve the performance of global navigation satellite systems (GNSSs)" |
| Additional signal  | EGNOS Safety of Life service declared available for aviation on 2 March 2011 (per ESA)                                                                        |
| Important signal   | EGNOS is the European SBAS implementation; it is referenced in EASA ETSO context                                                                              |

### MSAS — Japan

| Field                 | Current public signal                                                                                |
| --------------------- | ---------------------------------------------------------------------------------------------------- |
| System                | MTSAT Satellite-based Augmentation System (MSAS) / Michibiki Satellite-based Augmentation Service    |
| Operating agency      | Japan Civil Aviation Bureau (JCAB), Ministry of Land, Infrastructure, Transport and Tourism          |
| Service type          | SBAS for aviation                                                                                    |
| Public source signals | ESA Navipedia; UNOOSA ICG presentations; JCAB/EGNOS GSC presentations                                |
| Scope signal          | GPS augmentation system for aviation use in Japan                                                    |
| Important signal      | JCAB is evaluating MSAS for LPV operation; system evolution linked to Michibiki (QZSS) constellation |

### GAGAN — India

| Field              | Current public signal                                                                                                                                                                |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| System             | GPS Aided GEO Augmented Navigation (GAGAN)                                                                                                                                           |
| Operating agency   | Airports Authority of India (AAI) and Indian Space Research Organisation (ISRO)                                                                                                      |
| Service type       | SBAS for aviation safety-of-life                                                                                                                                                     |
| Public source page | https://www.aai.aero/en/content/what-gagan                                                                                                                                           |
| Scope signal       | "GAGAN is the acronym for GPS Aided GEO Augmented Navigation. The GAGAN uses a system of ground stations to provide necessary augmentations to the GPS standard positioning service" |
| Additional signal  | ISRO page confirms GAGAN as "Satellite Based Augmentation System (SBAS) implemented jointly with Airport Authority of India"                                                         |
| Important signal   | GAGAN is the Indian SBAS implementation                                                                                                                                              |

### BDSBAS — China

| Field                 | Current public signal                                                                                              |
| --------------------- | ------------------------------------------------------------------------------------------------------------------ |
| System                | BeiDou Satellite-Based Augmentation System (BDSBAS)                                                                |
| Operating agency      | China Satellite Navigation Office                                                                                  |
| Service type          | SBAS integrated with BeiDou Navigation Satellite System (BDS)                                                      |
| Public source signals | BeiDou official site (en.beidou.gov.cn); ION Navigation journal; ICG presentations                                 |
| Scope signal          | BDSBAS provides SBAS services as part of the BeiDou system; initially single-frequency, developing DFMC capability |
| Important signal      | BDSBAS is the Chinese SBAS implementation; formerly known as Satellite Navigation Augmentation System (SNAS)       |

### KASS — South Korea

| Field              | Current public signal                                                                                                         |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| System             | Korea Augmentation Satellite System (KASS)                                                                                    |
| Operating agency   | Korea Aerospace Research Institute (KARI)                                                                                     |
| Service type       | SBAS for aviation                                                                                                             |
| Public source page | https://www.kari.re.kr/eng/contents/200                                                                                       |
| Scope signal       | "KASS utilizes Satellite-Based Augmentation System (SBAS) technology to reduce GPS positioning errors to within three meters" |
| Additional signal  | KASS certified by Korean national authorities and declared operational (per Thales Alenia Space and GPS World reporting)      |
| Important signal   | KASS is the Korean SBAS implementation; developed with Thales Alenia Space as prime contractor                                |

### SouthPAN — Australia and New Zealand

| Field              | Current public signal                                                                                                                         |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| System             | Southern Positioning Augmentation Network (SouthPAN)                                                                                          |
| Operating agency   | Geoscience Australia and Toitū Te Whenua Land Information New Zealand                                                                         |
| Service type       | SBAS for aviation and other positioning applications                                                                                          |
| Public source page | https://www.ga.gov.au/scientific-topics/positioning-navigation/positioning-australia/about-the-program/southpan                               |
| Scope signal       | "SouthPAN delivers three services: L1 SBAS, Dual Frequency Multi-Constellation (DFMC) SBAS, and Precise Point Positioning Via SouthPAN (PVS)" |
| Additional signal  | Early Open Services available; 99.5% accuracy service milestone reported                                                                      |
| Important signal   | SouthPAN is the Australian/New Zealand SBAS implementation                                                                                    |

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

- [ ] MSAS: JCAB service definition and LPV evaluation status
- [ ] GAGAN: AAI/ISRO service definition and certification basis
- [ ] BDSBAS: BeiDou official SBAS service signal and DFMC development status
- [ ] KASS: KARI service definition and certification basis
- [ ] SouthPAN: Geoscience Australia service definition and DFMC service status
