---
title: GNSS Radio Occultation
description: Atomic concept note on GNSS Radio Occultation as an empirical ionospheric sounding technique
tags: [gnss-ro, ionosphere, technique, empirical, satellite, occultation]
created: 2026-04-26
modified: 2026-04-26
status: draft
verification_status: empirical-study
---

# GNSS Radio Occultation

## Definition status

This note defines GNSS Radio Occultation (GNSS-RO) as an empirical satellite-based technique for profiling the Earth's ionosphere using radio signals from Global Navigation Satellite System (GNSS) transmitters observed by low-Earth-orbiting (LEO) receivers.

Boundary:
- This is a technique concept note, not a system-design note.
- It does not cover SBAS correction calculations, GBAS references, or avionics.
- It links to empirical results from GNSS-RO applications in the vault.

## Working definition

GNSS-RO measures phase and amplitude changes of GNSS signals as they pass through the ionosphere during an occultation event — when a LEO satellite sets or rises behind the Earth relative to a GNSS transmitter. From these measurements, vertical profiles of ionospheric electron density and ionospheric total electron content (TEC) can be derived.

### Key technique characteristics

| Characteristic | Description |
|----------------|-------------|
| **Data source** | LEO constellations with GNSS receivers (e.g., COSMIC-2, Spire) |
| **Observable** | Excess phase → bending angle → refractivity → electron density |
| **Vertical resolution** | Typically 200 m – 1 km |
| **Horizontal footprint** | Tangent-point region; hundreds of kilometres along ray path |
| **Coverage** | Global; especially valuable over ocean and data-sparse regions |
| **Limitation** | Spase temporal sampling; post-sunset gaps at low latitudes |

## Relationship to the vault

### Parent domain
- [[Ionospheric Model Validation]] — GNSS-RO provides the empirical ground truth against which models are validated

### Sibling domains
- [[Total Electron Content (TEC)]] — TEC is the primary observable extracted from GNSS-RO profiles
- [[SBAS Integrity]] — GNSS-RO data informs ionospheric threat models that feed integrity design
- [[Source - GNSS Radio Occultation Technique]] — source scaffold for literature and datasets

### Implementation connection
- [[IRI-2020 vs GNSS-RO Indonesia]] — concrete empirical application to Indonesia using Spire/COSMIC-2 podTec data
- [[Indonesian SBAS ION Paper Iterations]] — research paper series using GNSS-RO for SBAS threat screening

## Aviation and SBAS implications

GNSS-RO has two distinct relevance levels for SBAS design:

1. **Threat discovery** — GNSS-RO can characterize ionospheric delay magnitude and spatial variability in regions lacking dense ground-station networks. This is valuable for pre-operational threat-model design.

2. **Operational correction limitation** — GNSS-RO does NOT provide the real-time, high-rate TEC measurements required for service-level SBAS ionospheric correction broadcasting. Ground GNSS receiver networks remain the operational standard for SBAS GIVE computation.

**Critical boundary:** The vault treats GNSS-RO as a threat-discovery and model-validation instrument, not as a direct SBAS correction source.

## Data products referenced in the vault

- **podTec** (phase-derived TEC along occultation ray) — Spire/COSMIC-2 product used in the Indonesian study
- **EUMETSAT/Radio Occultation Meteorology** — operational weather RO; not ionospheric
- **UCAR/CDAAC** — primary archive for COSMIC series RO data

## Current source anchors

- [[Source - GNSS Radio Occultation Technique]] — starter provenance scaffold
- [[Source - GNSS-RO Indonesia Empirical Study]] — study-specific source scaffold

## Open provenance questions

- How does Spire podTec calibration compare to ground GNSS TEC for absolute accuracy?
- What is the relationship between RO-derived TEC along a tangent-point ray and the IPP-domain TEC that SBAS ground segments actually model?
- Should GNSS-RO validation of empirical models be separated from GNSS-RO threat-screening for SBAS?

## See also

- [[Ionospheric Model Validation]]
- [[Total Electron Content (TEC)]]
- [[SBAS Integrity]]
- [[Source - GNSS Radio Occultation Technique]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[Indonesian SBAS ION Paper Iterations]]
- [[ASEAN SBAS Deployment Barriers]]
