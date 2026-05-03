---
title: Source - MSAS
description: Source note for Japan's MSAS / Michibiki SBAS transmission service using official QZSS and ICAO APAC CNS SG source material
tags: [source, msas, sbas, japan, qzss, jcab, mlit, aviation]
source_type: service-provider-record
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: official-qzss-and-icao-apac-extracted
last_extracted_source: "QZSS SBAS Transmission Service page; ICAO APAC CNS SG/24 IP15 Japan SBAS Status Update in Japan"
---

# Source - MSAS

## Scope of this note

This note is the knowledge base's institutional source anchor for Japan's MSAS / Michibiki SBAS transmission service.

Boundary:

- This note anchors official QZSS service-page signals and ICAO APAC CNS SG/24 information-paper signals.
- It does not verify current post-2023 or post-2025 operational status unless a source explicitly states it.
- It does not provide procedure minima, aircraft eligibility, operational approval, or airport-specific procedure status.
- The 2020 ICAO APAC information paper is valuable for the transition plan and architecture history, but later operational facts require later JCAB/MLIT/QZSS or ICAO APAC sources.

## Primary sources extracted

### QZSS SBAS Transmission Service page

|| Field | Signal |
||---|---|
|| Source owner | QZSS / Cabinet Office Japan public service page |
|| Service | SBAS Transmission Service |
|| Current transmission signal | SBAS signal made by MLIT transmitted from QZS on a GEO using QZSS SBAS transmission service |
|| Start of QZSS transmission service | April 2020 |
|| Previous transmission platform | MTSAT operated by MLIT |
|| Receiver context | SBAS L1Sb receivers |

### ICAO APAC CNS SG/24 IP15 — SBAS Status Update in Japan

|| Field | Signal |
||---|---|
|| Meeting | ICAO APAC CNS SG/24, 30 Nov – 4 Dec 2020 |
|| Agenda item | 5.5 — Other navigation related issues |
|| Presenter | Japan |
|| Subject | SBAS status update in Japan |
|| Main system transition signal | MSAS transition from MTSAT to QZS-3 completed end of March 2020 |

## Verified service identity

|| Field | Verified signal |
||---|---|
|| System | MSAS / Michibiki Satellite-based Augmentation Service context |
|| Operating/government context | MLIT / JCAB for SBAS signal generation and aviation authorization context; QZSS provides satellite transmission service |
|| Original operational date | 27 September 2007 (MSAS operational with MTSAT, per ICAO APAC IP15) |
|| QZSS transmission transition | End of March / April 2020 from MTSAT to QZS-3/QZSS GEO transmission |
|| Current public service page | QZSS SBAS Transmission Service |

## Verified timeline signals

|| Year | Signal |
||---|---|
|| 2007 | MSAS operational with MTSAT on 27 September 2007 |
|| 2017 | QZS-3 GEO launched; L5 DFMC validation signal PRN196 available from 23 September 2017 |
|| 2018 | LPV implementation decision signal in ICAO APAC IP15; QZSS 4-satellite constellation operational |
|| 2020 | MSAS transition from MTSAT to QZS-3 completed end of March; QZSS SBAS transmission service from April 2020 |
|| 2021 | LPV250 trial operation planned using MSAS V2 / QZS-3 only, VMC-only |
|| 2023 | Planned full LPV operation using QZS-3, QZS-6, QZS-7 in the 2020 plan; later verification still required |

## Verified MSAS evolution signals from ICAO APAC IP15

|| Version | Phase | Verified signal |
||---|---|---|
|| MSAS V1 | Initial Performance Phase (2007–2020) | MTSAT-2, 2 Master Control Stations, 6 Ground Monitor Stations; GPS augmentation for RNAV / NPA / RNP 0.3 context |
|| MSAS V2 | System Update Phase (2020–2023) | QZS-3 GEO takeover; replacement ground system with 2 MCS, 13 GMS, 3 Uplink Stations in Japan |
|| MSAS V3 | LPV Performance Phase (planned in 2020 source) | Planned vertical guidance through three QZSS GEOs and ionosphere software for low-latitude/magnetic equatorial regions |
|| MSAS V4 | DFMC Validation Phase | DFMC SBAS validation for ICAO SARPs; GPS, Galileo, QZSS support in experiment context |

## Verified PRN and signal-transition signals

- Legacy MTSAT-2 broadcast in dual PRN mode: PRN 129 and PRN 137.
- Transition to QZSS completed in March 2020, with PRN 129 and PRN 137 transferred from MTSAT-2 to QZS-3.
- PRN 187 was used for L1 SBAS-compatible signal during QZSS GEO pre-operational testing.
- L5 augmentation signal PRN196 from QZS-2 was available for DFMC validation from 23 September 2017.
- Additional L5 validation signals listed in IP15: PRN197 (QZS-3 GEO) and PRN200 (QZS-4 IGSO).

## Verified LPV planning signal

The ICAO APAC IP15 source states Japan planned full-scale LPV operation targeting 83 civilian airports, excluding two military control airports, with existing RNP approaches to be sequentially redesigned to LPV after the full-scale operation phase.

Boundary: this is a 2020 planning signal. It must not be reused as a current operational status claim without later direct source verification.

## What this source can currently anchor

- MSAS historical operational start in 2007
- MSAS transition from MTSAT to QZSS/QZS-3 in March/April 2020
- QZSS SBAS transmission service role: transmitting MLIT-generated SBAS signal from QZS on GEO
- MSAS architecture evolution from V1 to V2 in the 2020 source
- PRN transition and L5 DFMC validation signals in the 2020 source
- LPV implementation planning in Japan as of ICAO APAC CNS SG/24 IP15

## What this source must not be used for yet

Do not use this note alone to publish:

- current post-2023 LPV operational status
- airport-specific LPV procedure availability or minima
- aircraft eligibility or operational authorization
- MSAS performance metrics as current certified values
- Southeast Asia service expansion as an approved or operational service
- equivalence between MSAS and GAGAN/SouthPAN/EGNOS without matched current service-provider sources

## Relationship to other source notes

|| Source note | Relationship |
||---|---|
|| [[Source - SBAS Service Providers]] | Family-level service-provider source anchor |
|| [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] | Regional Asia-Pacific SBAS coordination context |
|| [[Source - ICAO Annex 10 Volume I GNSS SBAS]] | SARPs/source-family routing |
|| [[Source - ICAO Doc 9849]] | GNSS implementation and DFMC evolution context |
|| [[SBAS Standards Source Matrix]] | Claim-routing matrix for separating historical, planning, operational, equipment, and procedure claims |

## Extraction gaps

- Current JCAB/MLIT official MSAS service definition after 2023/2025
- Current LPV procedure publication status and AIP references
- Current MSAS performance reports and service notices
- Current QZSS satellite/PRN assignments for operational MSAS after V3/V4 updates
- Later ICAO APAC or EGNOS/JRANSA technical interchange papers that may update MSAS V3/V4 status

## See also

- [[MSAS]]
- [[Source - SBAS Service Providers]]
- [[Source - ICAO APAC GBAS-SBAS Implementation Forums]]
- [[SBAS Standards Source Matrix]]
- [[Asia-Pacific SBAS Implementation Patterns]]
- [[GAGAN]]
