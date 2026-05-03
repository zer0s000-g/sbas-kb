---
title: IRI-2020 vs GNSS-RO Indonesia
description: Synthesis note comparing IRI-2020 model predictions with GNSS-RO empirical observations over Indonesia
tags: [synthesis, iri-2020, gnss-ro, indonesia, tec, validation, error, empirical]
created: 2026-04-26
modified: 2026-04-26
status: draft
verification_status: empirical-study
---

# IRI-2020 vs GNSS-RO Indonesia

## Scope status

This note synthesises the empirical comparison between IRI-2020 model predictions and GNSS Radio Occultation observations over the Indonesian region. It is a comparison note, not a standalone authority on either the model or the technique.

Boundary:

- It does not restate the full IRI model specification.
- It does not claim that the sampled days represent all Indonesian conditions.
- It links empirical findings to SBAS integrity implications in the vault.

## Comparison dimensions

### Overall error summary (initial 5-day study)

| Metric          | Value      | Interpretation                                  |
| --------------- | ---------- | ----------------------------------------------- |
| Bias            | 66.72 TECU | IRI underestimates TEC by 66.72 TECU on average |
| RMSE            | 94.34 TECU | Total error magnitude                           |
| MAE             | 67.01 TECU | Average absolute error                          |
| MAPE            | 87.6%      | Mean percentage error                           |
| Correlation (r) | 0.4146     | Weak positive correlation                       |
| R²              | −0.7309    | Model performs worse than predicting the mean   |

### Monthly variation

| Month    | Bias (TECU) | RMSE (TECU) |
| -------- | ----------- | ----------- |
| January  | 83.7        | 108.7       |
| February | 70.2        | 91.9        |
| March    | 72.5        | 113.2       |
| April    | 75.8        | 102.3       |
| May      | 48.0        | 69.4        |

### Altitude dependence

Errors are largest at lower occultation heights (near the F2 layer peak):

| Altitude (km) | Bias (TECU) |
| ------------- | ----------- |
| 350–400       | 126.0       |
| 400–450       | 77.9        |
| 500–550       | 47.9        |
| 550–600       | 33.8        |

### Spatial variation

| Region                   | Bias (TECU) | RMSE (TECU) |
| ------------------------ | ----------- | ----------- |
| Western (Sumatra/Java)   | 98.0        | 122.7       |
| Central (Kalimantan)     | 114.8       | 148.2       |
| Eastern (Sulawesi/Papua) | 106.6       | 145.3       |

## What this comparison implies

1. **Systematic underestimate, not random scatter** — IRI-2020 consistently underpredicts TEC in the Indonesian equatorial region.
2. **Altitude sensitivity** — The largest errors occur near the F2 peak height, suggesting the model's vertical profile parameterization is misaligned with actual equatorial conditions.
3. **Spatial heterogeneity matters** — Central Indonesia (Kalimantan) shows the largest errors, likely due to EIA crest proximity.
4. **Temporal gaps are integrity-relevant** — No post-sunset (18–21 LT) profiles means the most challenging equatorial conditions are unobserved in this dataset.

## Comparison to SBAS-relevant thresholds

| Quantity         | TECU  | L1 equivalent (m) | SBAS relevance                            |
| ---------------- | ----- | ----------------- | ----------------------------------------- |
| Median RO TEC    | 46.9  | 7.6               | Typical delay                             |
| p95 RO TEC       | 166.0 | 26.9              | Heavy delay, threat discovery             |
| p99 RO TEC       | 341.1 | 55.4              | Extreme delay, overbounding consideration |
| Maximum observed | 468.4 | 76.1              | Tail event, integrity penalty             |
| IRI-2020 bias    | 66.72 | 10.8              | Systematic model error                    |

## Relationship to the vault

### Parent domain

- [[Ionospheric Model Validation]] — generic methodology
- [[GNSS Radio Occultation]] — technique used to produce the RO side of the comparison
- [[Total Electron Content (TEC)]] — primary compared variable

### Sibling domain

- [[SBAS Ionospheric Threat — Empirical Evidence]] — reframes these errors as SBAS threat inputs

### Upstream notes

- [[Source - IRI-2020 Ionosphere Model]] — model provenance
- [[Source - GNSS-RO Indonesia Empirical Study]] — data provenance

## What this comparison does NOT justify

- That IRI-2020 is globally invalid (findings are regional and conditional)
- That GNSS-RO can replace ground GNSS for operational SBAS correction
- That the sampled days represent all Indonesian conditions
- That the post-sunset gap proves low risk (absence of data ≠ absence of risk)

## Open questions

- How do these errors translate to SBAS protection level inflation?
- What additional ground-station density would be needed to bound these conditions operationally?
- Would NeQuick or a physics-based model perform differently in the same region?

## See also

- [[Ionospheric Model Validation]]
- [[GNSS Radio Occultation]]
- [[Total Electron Content (TEC)]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[Indonesian SBAS ION Paper Iterations]]
- [[Source - IRI-2020 Ionosphere Model]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[Indonesia]]
- [[ASEAN SBAS Deployment Barriers]]
