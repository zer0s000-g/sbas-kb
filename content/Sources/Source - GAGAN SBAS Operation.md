---
title: "Source - GAGAN SBAS Operation"
description: Source note for GAGAN (GPS Aided GEO Augmented Navigation) Indian SBAS system, with verified signals from ICAO APAC ITF/7 IP05b (May 2025) and AAI public documentation
tags: [source, gagan, sbas, india, aviation, dgca, isro, aai, operational]
source_type: service-provider-record
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: partially-verified-with-itf7-ip05b
last_extracted_source: "ICAO APAC ITF/7 IP05b — GAGAN SBAS Based LPV Procedure Implementation Update in India (India, GBAS/SBAS ITF/7, 14-16 May 2025)"
---

# Source - GAGAN SBAS Operation

## Scope of this note

This note is the knowledge base's institutional source anchor for GAGAN (GPS Aided GEO Augmented Navigation), India's Satellite-Based Augmentation System.

Boundary:

- This note is not itself an authoritative GAGAN technical specification.
- Exact system performance values, coverage boundaries, and operational approval conditions must be verified against official DGCA India, AAI, and ISRO publications.
- This note extracts and anchors verified signals from the ICAO APAC ITF/7 working context and from AAI public documentation.
- This note does not imply that GAGAN service is available outside Indian FIRs and airspace.

## Primary source

### ICAO APAC ITF/7 IP05b — GAGAN SBAS Based LPV Procedure Implementation Update in India

Source: India presentation to Seventh GBAS/SBAS Implementation Task Force (ITF/7), hosted by ICAO APAC, 14–16 May 2025.

URL: `https://www.icao.int/sites/default/files/APAC/Meetings/2025/2025%20GBASSBAS%20ITF7/4-Information%20Papers/A4-IP05b-GAGAN-SBAS-BASED-LPV-PROCEDURE-IMPLEMENTATION-UPDATE-IN-INDIA.pdf`

Authors: India (presented by AAI/ISRO)

## Verified signals from ITF/7 IP05b

### System certification and operational status

|| Field | Verified signal |
||---|---|
|| Certifying authority | DGCA India |
|| Operational certification date (RNP 0.1) | 2013 |
|| APV I operational certification date | 2015 |
|| Coverage scope | Indian FIRs (RNP 0.1); Indian Landmass (APV I) |
|| Governing standard context | ICAO Annex 10 SARPs |

### Architecture — ground segment

Source signals: ITF/7 IP05b paragraph 1.2

- **Fifteen ground reference stations (INRES)**: Ahmedabad, Bengaluru, Trivandrum, Port Blair, Guwahati, Delhi, Porbandar, Dibrugarh, Jaisalmer, Bhubaneshwar, Kolkata, Gaya, Nagpur, Jammu, Goa
- **Two Master Control Centres (INMCC)**: Bengaluru (GBC) and Delhi (GBM)
- **Three uplink stations (INLUS)**: two at Bengaluru, one at Delhi
- **Upgrade year (frequency standard)**: 2020 — Microsemi 5071A High Precision Frequency Standard (HPFS) installed at all three INLUS
- **Upgrade year (signal generator)**: 2022 — NovAtel GUS Type-I Signal generator installed at all three INLUS
- **Reference station upgrade (receiver)**: Novatel G-III receiver and IBM S914 server installed at all 15 INRES (phased 2020–2024); DFO/DFMC ready

### Architecture — space segment

Source signals: ITF/7 IP05b paragraph 1.2; AAI public FAQ page

- **GSAT-8**: Geostationary satellite, PRN code 127, 55° E longitude
- **GSAT-10**: Geostationary satellite, PRN code 128, 82° E longitude
- **GSAT-15**: Geostationary satellite, PRN code 132 (in-orbit spare), 83° E longitude

### Ionospheric monitoring

Source signal: ITF/7 IP05b paragraph 2.4

- Indian Ionosphere monitoring network upgraded with Septentrio PolaRx5S receiver
- Supports multi-frequency, multi-constellation ionospheric monitoring

### LPV procedure status (as of ITF/7, May 2025)

Source signals: ITF/7 IP05b paragraphs 3.1–3.2

- **ICAO SBAS channel numbers assigned to India**: 53
- **LPV procedures published**: 23 procedures at 15 airports
- **LPV procedures in simulator validation and flight trials**: 12 procedures
- **LPV procedures under design/development**: 18 procedures
- **Published procedure AIP link**: `https://aim-india.aai.aero/eaip-v2-02-2025/index-en-GB.html` (select AD_2 under Part 3 — Aerodromes)
- **ICAO APAC SBAS map**: `https://www.icao.int/APAC/Pages/GBAS-SBAS-MAP.aspx`
- **Flight inspection**: AAI Flight Inspection Unit aircraft certified by DGCA India for GAGAN LPV procedure validation

### Workshop hosting

Source signal: ITF/7 IP05b paragraph 4

- India to host SBAS/GBAS Workshop for Airspace Users in Bengaluru, 14–16 October 2025

## What this source can currently anchor

With ITF/7 IP05b verified as a public ICAO document:

- GAGAN is DGCA India certified, declared operational for RNP 0.1 services (2013) and APV I services (2015)
- GAGAN ground segment consists of 15 INRES, 2 INMCC, 3 INLUS
- GAGAN space segment consists of GSAT-8 (PRN 127), GSAT-10 (PRN 128), GSAT-15 (PRN 132)
- GAGAN reference stations are DFO/DFMC ready as of the upgrade completed 2024
- 23 LPV procedures published at 15 Indian airports as of May 2025
- India is actively developing additional LPV procedures
- India hosts the SBAS/GBAS Workshop for Airspace Users in October 2025

## What this source must not be used for yet

Do not use this note alone to publish:

- GAGAN coverage extent or availability outside Indian FIRs and landmass
- LPV procedure minima, decision heights, or approach eligibility
- Specific DGCA approval conditions or operational authorization details beyond what IP05b states
- Comparative performance claims with other SBAS providers
- Claims about GAGAN's future capacity or expansion plans beyond IP05b

## Source weaknesses and extraction gaps

The following require additional source extraction:

- GAGAN signal-in-space accuracy and integrity performance figures (not yet extracted from official GAGAN performance reports)
- GAGAN service volume or coverage area definition (not yet extracted from AAI service documentation)
- Specific LPV procedure minima at individual airports (requires AIP/procedure chart sources)
- GAGAN operational experience or service disruption history (not yet extracted)
- Comparison with other SBAS providers on performance metrics

## Relationship to other source notes

|| Source note | Relationship to GAGAN source note |
||---|---|
|| [[Source - ICAO Annex 10 Volume I GNSS SBAS]] | Annex 10 SARPs define the SBAS system-level requirements that GAGAN implements |
|| [[Source - RTCA DO-229]] | DO-229F defines airborne equipment requirements for LPV operations that GAGAN supports |
|| [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] | ITF/7 IP05b is the source; ITF is the regional coordination forum |
|| [[Source - SBAS Service Providers]] | [[Source - SBAS Service Providers]] is the service-provider family anchor; this note is its GAGAN-specific child |
|| [[Source - ICAO Doc 9849]] | Doc 9849 provides ICAO GNSS implementation guidance context for GAGAN's role |

## See also

- [[GAGAN]] — in-vault system note (draft; requires source upgrade)
- [[SBAS Service Providers]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - ICAO APAC GBAS-SBAS Implementation Forums]]
- ICAO APAC SBAS map: `https://www.icao.int/APAC/Pages/GBAS-SBAS-MAP.aspx`
- AAI GAGAN page: `https://www.aai.aero/en/content/gagan`
