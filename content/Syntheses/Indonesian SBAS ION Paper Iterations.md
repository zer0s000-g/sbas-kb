---
title: Indonesian SBAS ION Paper Iterations
description: Tracking note for the ION-style SBAS ionospheric threat paper series produced from GNSS-RO Indonesian data
tags: [ion, sbas, indonesia, ionosphere, threat, paper, iteration, gnss-ro, igrf, provenance]
created: 2026-04-26
modified: 2026-04-26
status: draft
verification_status: empirical-study
---

# Indonesian SBAS ION Paper Iterations

## Scope status

This note tracks the iterative research paper series that reframed initial IRI-2020 model validation into ION-style SBAS ionospheric threat modeling. It is a meta-research note, not a source note.

Boundary:

- It does not restate the full paper content (that remains in the LaTeX sources).
- It preserves the evolution of research framing across iterations.
- It links empirical results to SBAS integrity implications.

## Iteration timeline

| Version | Date     | Framing shift                                        | Key artifact                                |
| ------- | -------- | ---------------------------------------------------- | ------------------------------------------- |
| V0      | Apr 2026 | IRI-2020 validation only                             | `ionosphere_model_error_indonesia.tex`      |
| V1      | Apr 2026 | SBAS threat discovery framework                      | `ion_indonesia_sbas_ro_threat_paper.tex`    |
| V2      | Apr 2026 | Expanded dataset (5→8 days), QC, coverage gaps       | `ion_indonesia_sbas_ro_threat_paper_v2.tex` |
| V3      | Apr 2026 | Space-weather + magnetic coordinates + threat budget | `ion_indonesia_sbas_ro_threat_paper_v3.tex` |
| V4      | Apr 2026 | IGRF14 magnetic-field upgrade, best model: R²=0.44   | `ion_indonesia_sbas_ro_threat_paper_v4.tex` |

## V1 → methodology correction

The first ION-style paper avoided overclaiming that Spire podTec mean values were certified SBAS vertical ionospheric delays. It consistently labels the observable as an RO-derived occultation TEC proxy.

## V2 → dataset expansion and coverage diagnosis

- Expanded from 5 to 8 stratified 2025 days
- Added explicit quality-control accounting
- Added local-time coverage-gap quantification
- **Key finding:** 18–21 LT post-sunset risk-window strict profiles = 0

## V3 → space-weather and magnetic-coordinate upgrade

- Added GFZ Kp, Kyoto Dst, F10.7
- Added centered-dipole magnetic latitude + magnetic local time
- Replaced sparse geographic model with additive robust Huber regression
- Added pre-operational SBAS threat-budget scaffold

## V4 → IGRF14 magnetic upgrade

- Replaced centered-dipole with `ppigrf`-derived IGRF14 dip latitude
- Added full IGRF field diagnostics
- Best model: RMSE 36.2 TECU, R² 0.44, p99 residual 114.2 TECU (18.5 m L1)

## Persistent integrity finding across all versions

The post-sunset 18–21 LT coverage gap remains **0 profiles** in every iteration. This is treated as:

- An **acquisition priority** for future RO campaigns
- An **integrity penalty** that must be accounted for in any threat budget
- **Not evidence of low risk** — absence of data is not evidence of absence

## Links to concrete results

- [[IRI-2020 vs GNSS-RO Indonesia]] — summary of empirical findings
- [[SBAS Ionospheric Threat — Empirical Evidence]] — threat implications
- [[Source - GNSS-RO Indonesia Empirical Study]] — study provenance scaffold

## Recommended next iteration (V5)

As defined in the V4 paper:

1. Targeted data expansion: acquire days specifically designed to fill 18–21 LT post-sunset coverage
2. Add storm-event days using Kp/Dst-driven selection
3. Build an acquisition diagnostic that selects days by local-time coverage and geomagnetic disturbance before downloading
4. Re-run V4 IGRF pipeline on expanded targeted sample
5. Only then begin candidate GIVE-like regional bin design

## See also

- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[GNSS Radio Occultation]]
- [[Ionospheric Model Validation]]
- [[Total Electron Content (TEC)]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[ASEAN SBAS Deployment Barriers]]
