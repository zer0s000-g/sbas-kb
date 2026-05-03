---
title: Ionospheric Model Validation
description: Atomic concept note on the methodology for validating empirical ionospheric models against independent observations
tags: [ionosphere, validation, model, iri-2020, empirical, gnss-ro, methodology]
created: 2026-04-26
modified: 2026-04-26
status: draft
verification_status: empirical-study
---

# Ionospheric Model Validation

## Definition status

This note defines ionospheric model validation as the systematic comparison of empirical or physics-based ionospheric model predictions against independent observational data to quantify model accuracy, identify systematic biases, and assess regional or conditional validity.

Boundary:

- This is a methodology concept note, not a specific model evaluation.
- It does not advocate for one model over another.
- It captures the generic validation framework applied in the Indonesian GNSS-RO study.

## Working definition

Model validation proceeds by:

1. Computing model predictions for the same spatial, temporal, and geometric conditions as the observations
2. Calculating error metrics between predicted and observed values
3. Stratifying errors by relevant conditions (altitude, local time, season, geomagnetic state)
4. Interpreting whether errors are systematic (bias), random (variance), or conditional (state-dependent)

## Standard error metrics

| Metric              | Formula                    | Interpretation                                  |
| ------------------- | -------------------------- | ----------------------------------------------- |
| **Bias**            | mean(observed − predicted) | Systematic over/under-estimation                |
| **RMSE**            | √(mean((obs−pred)²))       | Total error magnitude                           |
| **MAE**             | mean(\|obs − pred\|)       | Average absolute error                          |
| **Correlation (r)** | Pearson correlation        | Linear relationship strength                    |
| **R²**              | 1 − (SS_res / SS_tot)      | Explained variance (negative = worse than mean) |

## Relationship to the vault

### Parent domain

- [[GNSS Radio Occultation]] — RO provides the independent observations used for validation
- [[Total Electron Content (TEC)]] — TEC is the primary validated variable

### Sibling domains

- [[SBAS Integrity]] — model errors translate to correction uncertainty, impacting integrity
- [[Source - IRI-2020 Ionosphere Model]] — specific model that has been validated in the vault

### Implementation connection

- [[IRI-2020 vs GNSS-RO Indonesia]] — concrete validation study: IRI-2020 vs Spire/COSMIC-2 GNSS-RO over Indonesia
- [[Indonesian SBAS ION Paper Iterations]] — ION-style papers that reframe validation into threat-modeling

## Methodological considerations

### Spatial representativeness

A validation result at one location does not automatically generalize to another. The Indonesian study specifically found:

- Western Indonesia (Sumatra/Java): bias 98.0 TECU
- Central Indonesia (Kalimantan): bias 114.8 TECU
- Eastern Indonesia (Sulawesi/Papua): bias 106.6 TECU

### Temporal coverage

Sparse sampling (e.g., 5 or 8 days) captures seasonal snapshots but may miss:

- Post-sunset equatorial irregularity events
- Geomagnetic storm responses
- Solar-cycle variation

The vault explicitly flags the post-sunset gap (18–21 LT) in the Indonesian dataset as an integrity-relevant limitation, not an evidence of low risk.

### Model scope

IRI is a monthly-median empirical model. It does not predict day-to-day variability or storm conditions. Comparing IRI to instantaneous RO measurements is methodologically valid for assessing climatological bias, but not for evaluating operational forecast skill.

## Current source anchors

- [[Source - IRI-2020 Ionosphere Model]] — model provenance scaffold
- [[Source - GNSS-RO Indonesia Empirical Study]] — validation data provenance scaffold

## Open provenance questions

- Should model validation studies separate climatological accuracy from operational real-time accuracy?
- How should validation results be aggregated across spatially and temporally heterogeneous regions?
- What is the appropriate baseline for "acceptable" model error in an SBAS context?

## See also

- [[GNSS Radio Occultation]]
- [[Total Electron Content (TEC)]]
- [[SBAS Integrity]]
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[Indonesian SBAS ION Paper Iterations]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[Source - IRI-2020 Ionosphere Model]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
