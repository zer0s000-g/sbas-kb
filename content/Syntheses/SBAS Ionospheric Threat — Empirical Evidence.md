---
title: SBAS Ionospheric Threat — Empirical Evidence
description: Synthesis note reframing GNSS-RO Indonesian empirical results into SBAS ionospheric threat-modeling language
tags: [synthesis, sbas, ionosphere, threat, integrity, indonesia, empirical, gnss-ro]
created: 2026-04-26
modified: 2026-04-26
status: draft
verification_status: empirical-study
---

# SBAS Ionospheric Threat — Empirical Evidence

## Scope status

This note translates GNSS-RO empirical findings over Indonesia into SBAS ionospheric integrity language. It is a bridge note between ionospheric science and SBAS system design, not a design specification.

Boundary:

- It does not prescribe operational GIVE values or protection levels.
- It does not claim that the sampled data is sufficient for certification.
- It frames empirical observations as threat-discovery inputs for pre-operational SBAS assessment.

## Threat categories from Indonesian GNSS-RO data

### Threat 1: Large absolute delay tails

| Statistic        | TECU  | L1 equivalent (m) |
| ---------------- | ----- | ----------------- |
| Median           | 46.9  | 7.6               |
| p95              | 166.0 | 26.9              |
| p99              | 341.1 | 55.4              |
| Maximum observed | 468.4 | 76.1              |

**SBAS interpretation:** Delays of 55+ m at the 99th percentile exceed typical mid-latitude SBAS ionospheric assumptions. Any ASEAN SBAS must account for heavier tails than WAAS/EGNOS mid-latitude experience.

### Threat 2: Spatial gradients

| Statistic | Equivalent L1 gradient (mm/km) |
| --------- | ------------------------------ |
| Median    | 6.6                            |
| p95       | 46.7                           |
| p99       | 81.9                           |
| Maximum   | 208.3                          |

**SBAS interpretation:** Gradient events at the 99th percentile (~82 mm/km) challenge the differential-correction assumption that ionospheric delay varies smoothly over SBAS grid cell scales. Large gradients are known threats to WAAS integrity in convective weather and storm conditions; equatorial post-sunset plasma bubbles may produce comparable or larger gradients.

### Threat 3: Undersampled risk windows

| Risk window                | Profiles available                  |
| -------------------------- | ----------------------------------- |
| Post-sunset 18–21 LT       | **0**                               |
| Storm/disturbed class (V3) | 23 (possibly coincidental sampling) |

**SBAS interpretation:** An integrity threat model built only on available data would systematically underestimate post-sunset risk. This is not a finding of low risk — it is a finding of insufficient data. Operational SBAS certification requires deliberate acquisition of these windows.

### Threat 4: Model underestimate bias

| Metric                   | Value                  |
| ------------------------ | ---------------------- |
| IRI-2020 systematic bias | 66.72 TECU (10.8 m L1) |
| RMSE                     | 94.34 TECU (15.3 m L1) |

**SBAS interpretation:** If an SBAS ionospheric model performs similarly to IRI-2020 in this region, broadcast corrections would systematically understate actual delay. This inflates the residual error budget and can compromise integrity if the GIVE does not overbound the true model error.

## Threat-budget scaffold (pre-operational)

The V3 paper introduced a pre-operational SBAS threat-budget separation:

| Component                                | Source                | Current trust level                 |
| ---------------------------------------- | --------------------- | ----------------------------------- |
| Observed delay-tail proxy                | GNSS-RO               | Moderate (sparse temporal sampling) |
| Leave-day-out temporal-transfer residual | Robust model          | Moderate (R² = 0.44)                |
| Spatial-gradient allowance               | Pairwise RO proxy     | Low (not IPP-domain)                |
| Post-sunset coverage penalty             | Missing data          | Must be explicitly penalized        |
| Storm-time extrapolation penalty         | Limited storm samples | Must be explicitly penalized        |

**Key boundary:** Convert this scaffold into candidate GIVE-like quantization **only after** post-sunset and storm gaps are closed with additional data and ground GNSS/scintillation validation.

## Relationship to the vault

### Parent domain

- [[IRI-2020 vs GNSS-RO Indonesia]] — empirical results being translated
- [[SBAS Integrity]] — integrity concepts receiving empirical input
- [[ASEAN SBAS Deployment Barriers]] — barriers strengthened by empirical findings

### Sibling domain

- [[Indonesian SBAS ION Paper Iterations]] — research evolution tracking
- [[Source - Equatorial Ionosphere and SBAS Feasibility]] — theoretical scaffold now receiving empirical anchor

### Upstream notes

- [[GNSS Radio Occultation]] — technique
- [[Total Electron Content (TEC)]] — observable
- [[Ionospheric Model Validation]] — methodology

## What this note does NOT claim

- That GNSS-RO can directly compute operational SBAS GIVE values
- That the sampled days provide sufficient coverage for certification
- That Indonesia is "worse" than other equatorial regions (no comparative data)
- That the threat budget is ready for operational use

## Recommended operational-design implications

1. **Do not inherit mid-latitude SBAS ionospheric assumptions** for Indonesia or ASEAN.
2. **Stratify threat assessment** by IGRF dip-latitude region, local-time window, and space-weather state.
3. **Combine RO with ground GNSS/scintillation** for operational design — RO alone is insufficient.
4. **Deliberately acquire post-sunset and storm data** before deriving GIVE-like bins.
5. **Use RO as threat-discovery, ground monitoring as operational validation**.

## See also

- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[ASEAN SBAS Deployment Barriers]]
- [[SBAS Integrity]]
- [[GNSS Radio Occultation]]
- [[Total Electron Content (TEC)]]
- [[Ionospheric Model Validation]]
- [[Indonesian SBAS ION Paper Iterations]]
- [[Source - Equatorial Ionosphere and SBAS Feasibility]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[Indonesia]]
