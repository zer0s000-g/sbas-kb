---
title: Source - GNSS-RO Indonesia Empirical Study
description: Starter provenance scaffold for the Indonesian GNSS-RO ionospheric empirical study (April 2026)
tags: [source, indonesia, gnss-ro, empirical, tec, validation, spire, cosmic-2, cdaac, iri-2020, provenance]
source_type: empirical-study
created: 2026-04-26
modified: 2026-04-26
status: starter
verification_status: metadata-pending
---

# Source - GNSS-RO Indonesia Empirical Study

## Scope of this note

This is a starter source scaffold for the Indonesian GNSS Radio Occultation empirical study conducted in April 2026.

Boundary:
- It is not a completed source extraction.
- It does not independently verify the numerical results; it documents what the vault contains.
- It exists to anchor empirical claims in the vault to a recognizable study context.

## Why this source note matters

The vault contains a series of research artifacts (LaTeX papers, analysis scripts, figures, CSV data) produced during a systematic GNSS-RO-based study of Indonesian ionospheric conditions. Without a study-level source scaffold, it is unclear which claims are derived from this dataset versus other sources.

## Study provenance

| Field | Value |
|-------|-------|
| **Conducted** | April 2026 |
| **Data source** | Spire Global constellation via UCAR CDAAC |
| **Period** | 5 representative days (Jan–May 2025); later expanded to 8 stratified days |
| **Region** | Indonesia geofence: −11.0° to 6.0° N, 95.0° to 141.0° E |
| **Software** | Custom Python scripts |
| **Paper series** | ION-style SBAS ionospheric threat papers (V1–V4) |

## Key numerical findings

### Initial 5-day study
- 301 Indonesia occultations from 17,909 source files
- IRI-2020 bias: 66.72 TECU (87.6% mean underestimate)
- RMSE: 94.34 TECU; R²: −0.73

### Expanded 8-day study (V2)
- 463 intersecting profiles → 208 strict tangent-point profiles → 207 QC-valid profiles
- RO TEC p95: 166.0 TECU; p99: 341.1 TECU
- Leave-day-out RMSE: 56.6 TECU; R²: −0.38

### Space-weather upgrade (V3)
- Added GFZ Kp, Kyoto Dst, F10.7, centered-dipole magnetic coordinates
- Best model R²: 0.42; p99 residual: 120.1 TECU (19.5 m L1)

### IGRF upgrade (V4)
- Replaced centered-dipole with IGRF14 dip-latitude
- Best model R²: 0.44; p99 residual: 114.2 TECU (18.5 m L1)

### Post-sunset coverage gap
- 18–21 LT strict profiles: **0** in all iterations
- Flagged as integrity-relevant limitation, not evidence of low risk

## Current in-vault references supported by this scaffold

- [[IRI-2020 vs GNSS-RO Indonesia]] — direct comparison results
- [[SBAS Ionospheric Threat — Empirical Evidence]] — threat quantification
- [[GNSS Radio Occultation]] — technique application
- [[Total Electron Content (TEC)]] — observable statistics
- [[Indonesian SBAS ION Paper Iterations]] — paper series tracking
- [[Indonesia]] — country-specific empirical anchor

## Claims this scaffold does NOT yet support

- Any claim that the findings generalize beyond the sampled days
- Any claim that the sampling is sufficient for operational GIVE design
- Any claim that Spire podTec accuracy is certified for SBAS use
- Any ranking of Indonesia against other equatorial regions

## Immediate audit questions

- Which specific Spire mission(s) and data product version(s) were used?
- Were formal UCAR CDAAC quality-control flags applied uniformly?
- How was the IRI-2020 model invoked (library, API, online tool)?
- What preprocessing was applied to podTec before TEC extraction?
- Which LaTeX/paper version is the primary citation target?

## Suggested downstream cleanup targets

If this scaffold becomes source-backed, revisit:
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[Indonesia]] — empirical claims in the country note

## Extraction template for next cycle

- Exact dataset URLs or DOIs
- Software version and dependency list
- Sample-size justification
- Statistical methodology references
- External validation or peer-review status

## See also

- [[GNSS Radio Occultation]]
- [[Ionospheric Model Validation]]
- [[Total Electron Content (TEC)]]
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[Indonesian SBAS ION Paper Iterations]]
- [[Source - GNSS Radio Occultation Technique]]
- [[Source - IRI-2020 Ionosphere Model]]
- [[Indonesia]]
