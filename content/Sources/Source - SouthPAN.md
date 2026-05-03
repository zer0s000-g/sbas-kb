---
title: Source - SouthPAN
description: Source note for SouthPAN (Southern Positioning Augmentation Network), using official Geoscience Australia and LINZ public service-definition material
tags:
  [source, southpan, sbas, australia, new-zealand, geoscience-australia, linz, service-definition]
source_type: service-provider-record
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: official-service-definition-extracted
last_extracted_source: "SouthPAN Service Definition Document for Signal-In-Space Open Services, SBAS-STN-0001 Rev 03, effective 14 February 2024"
---

# Source - SouthPAN

## Scope of this note

This note is the knowledge base's institutional source anchor for SouthPAN (Southern Positioning Augmentation Network), the Australia–New Zealand SBAS capability.

Boundary:

- This note anchors official open-service and service-definition claims only.
- It does not verify aviation Safety-of-Life certification, LPV procedure publication, aircraft operational approval, or airport-specific minima.
- Performance values below are quoted only in the context of SouthPAN early Open Services, not certified aviation Safety-of-Life service.
- Operational aviation claims must wait for the applicable certified Safety-of-Life service definition, regulator material, AIP/procedure sources, and operator/aircraft approval context.

## Primary official sources extracted

### SouthPAN Service Definition Document for Signal-In-Space Open Services

|| Field | Signal |
||---|---|
|| Issuing program | SouthPAN |
|| Document code | SBAS-STN-0001 |
|| Revision | 03 |
|| Effective date | 14 February 2024 |
|| Classification | OFFICIAL (AU) / UNCLASSIFIED (NZ) |
|| Source owner | Geoscience Australia / Toitū Te Whenua Land Information New Zealand |
|| Scope | Signal-In-Space Open Services, system architecture, RF signal characteristics, navigation message structures, indicative Open Service performance |

### SouthPAN early Open Services factsheet

|| Field | Signal |
||---|---|
|| Issuing body | Geoscience Australia |
|| Scope | Factsheet for GNSS users accessing SouthPAN early Open Services |
|| Status signal | Early Open Services available since September 2022 |
|| Aviation signal | Certified Safety-of-Life Service planned for 2028 |

### SouthPAN FAQ

|| Field | Signal |
||---|---|
|| Issuing body | Geoscience Australia |
|| Page updated | 28 November 2023 |
|| Scope | SouthPAN service overview, available services, PRN code, delivery organizations, user compatibility |

## Verified service identity

|| Field | Verified signal |
||---|---|
|| System | Southern Positioning Augmentation Network (SouthPAN) |
|| Providers | Geoscience Australia and Toitū Te Whenua Land Information New Zealand |
|| Operating/delivery organizations | Lockheed Martin Australia, GMV, Inmarsat Australia (delivery role per FAQ signal) |
|| Service model | Free and open-access early Open Services |
|| Early Open Services start | September 2022 |
|| Full Operating Capability target | 2028 |
|| Safety-of-Life aviation service | Planned/certified aviation service target in 2028; not yet available as certified aviation service in the extracted sources |
|| PRN code | 122 |

## Verified service types

|| Service | Signal | Current boundary |
||---|---|---|
|| L1 SBAS Open Service (OS-L1) | Augments GPS L1 C/A; uses L1 frequency 1,575.42 MHz | Open Service, not Safety-of-Life during early service phase |
|| DFMC SBAS Open Service (OS-DFMC) | Augments GPS L1 C/A, GPS L5, Galileo E1, Galileo E5a; signal on L5 | Open Service, next-generation DFMC context; not a certified aviation claim by itself |
|| PPP via SouthPAN (OS-PVS) | PPP corrections for GPS/Galileo; more accurate than OS-DFMC; delivered via L5 and internet | Open Service, not SBAS aviation Safety-of-Life operation |
|| Data Access Services | Same navigation messages delivered through internet instead of satellite broadcast | Data channel; not itself a satellite-broadcast aviation authorization |

## Verified coverage signals

|| Service | Coverage signal from official material |
||---|---|
|| OS-L1 | Mainland Australia and New Zealand |
|| OS-DFMC | Australia and New Zealand Exclusive Economic Zones (EEZs) |
|| OS-PVS | Australia and New Zealand Exclusive Economic Zones (EEZs) |

Coverage depends on satellite visibility, receiver environment, user equipment, and service area. Internet-delivered corrections may be technically accessible outside the region, but the correction data is relevant to the defined SouthPAN service area.

## Verified early Open Service performance signals

These values are for SouthPAN early Open Services only. They must not be reused as aviation Safety-of-Life performance commitments.

|| Service | Horizontal signal | Vertical signal | Notes |
||---|---|---|---|
|| L1 SBAS Open Service | better than or equal to 3 m, 95% confidence interval | better than or equal to 4 m, 95% confidence interval | Open Service factsheet |
|| DFMC SBAS Open Service | better than or equal to 1.5 m, 95% confidence interval | better than or equal to 2.5 m, 95% confidence interval | Open Service factsheet |
|| PVS Open Service | better than or equal to 0.40 m, 95% confidence interval | better than or equal to 0.55 m, 95% confidence interval | After convergence; convergence better than 80 minutes during early Open Service |

## Verified signal and message characteristics

- SouthPAN early Open Services are broadcast from the Inmarsat 4F2 geostationary satellite at 143.5° East longitude.
- PRN code: 122.
- L1 frequency: 1,575.42 MHz.
- L5 frequency: 1,176.45 MHz.
- L1 SBAS navigation message includes Message Type 0 (`Do not use for safety applications`) during the early Open Service phase.
- Service Provider ID bits of Message Type 17 are set to 8 to indicate SouthPAN navigation messages.
- SouthPAN transmits Message Type 27 (`SBAS Service Message`).
- SouthPAN does not expect to transmit Message Type 28 (`Clock-Ephemeris Covariance Matrix Message`) in the near term, per the extracted factsheet signal.

## Verified limitation signal

The Signal-In-Space Open Services service-definition document explicitly flags atmospheric/ionospheric activity north of 20°S as a limitation for maintaining lock on GNSS space vehicles and for large localized gradients, especially relevant to single-frequency and Safety-of-Life services.

This signal is important for ASEAN analysis because it reinforces that low-latitude ionospheric behavior is not a generic footnote; it is an explicit service-definition limitation in a regional SBAS system operating near the Asia-Pacific equatorial anomaly environment.

## What this source can currently anchor

- SouthPAN identity, providers, and public service scope
- Early Open Services start date and FOC target
- Service families: L1 SBAS, DFMC SBAS, PVS, Data Access Services
- Early Open Service coverage areas and open-service performance targets
- PRN 122 and Inmarsat 4F2 at 143.5° East as broadcast signal context
- Explicit non-Safety-of-Life boundary for early Open Service use
- Ionospheric limitation statement north of 20°S

## What this source must not be used for yet

Do not use this note alone to publish:

- certified aviation Safety-of-Life operational availability
- LPV procedure availability or minima in Australia or New Zealand
- aircraft eligibility, operator authorization, or regulator approval
- comparisons with WAAS/EGNOS/GAGAN on certified aviation performance
- ASEAN adoption feasibility claims without additional ASEAN-region evidence

## Relationship to other source notes

|| Source note | Relationship |
||---|---|
|| [[Source - SBAS Service Providers]] | Family-level service-provider source anchor |
|| [[Source - ICAO Annex 10 Volume I GNSS SBAS]] | SARPs/source-family routing for SBAS system-level requirements |
|| [[Source - ICAO Doc 9849]] | GNSS implementation guidance context, including DFMC and vulnerability topics |
|| [[Source - ICAO APAC GBAS-SBAS Implementation Forums]] | Regional Asia-Pacific coordination context |
|| [[SBAS Standards Source Matrix]] | Claim-routing matrix for separating Open Service, Safety-of-Life, equipment, procedure, and operational claims |

## See also

- [[SouthPAN]]
- [[Source - SBAS Service Providers]]
- [[SBAS-Systems-by-Region-MOC]]
- [[Asia-Pacific SBAS Implementation Patterns]]
- [[ASEAN SBAS Deployment Barriers]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
