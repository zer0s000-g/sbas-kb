---
title: Total Electron Content (TEC)
description: Atomic concept note on TEC as the primary ionospheric observable in SBAS integrity and GNSS-RO studies
tags: [tec, ionosphere, sbas, integrity, observable, empirical]
created: 2026-04-26
modified: 2026-04-26
status: draft
verification_status: empirical-study
---

# Total Electron Content (TEC)

## Definition status

This note defines Total Electron Content (TEC) as the line integral of electron density along the signal path between a GNSS satellite and a receiver. It is measured in TEC units (TECU), where 1 TECU = 10¹⁶ electrons/m².

Boundary:

- This is an observable concept note, not a model or system-design note.
- It does not cover algorithms for real-time SBAS ionospheric correction.
- It links TEC to integrity, validation, and empirical studies in the vault.

## Working definition

TEC quantifies the total number of free electrons in a cylinder with a cross-sectional area of 1 m² along the propagation path. It directly determines the ionospheric delay experienced by GNSS signals through the dispersive nature of the ionospheric plasma.

### TEC-to-delay conversion

At L1 frequency (1575.42 MHz):

| TEC (TECU)               | Equivalent L1 delay (m) |
| ------------------------ | ----------------------- |
| 1                        | 0.162                   |
| 10                       | 1.62                    |
| 50                       | 8.10                    |
| 100                      | 16.2                    |
| 200                      | 32.4                    |
| 341 (p99: Indonesian RO) | 55.4                    |

Conversion formula:  
**delay_L1 = (40.3 × TEC) / f_L1²**

## Relationship to the vault

### Parent domain

- [[GNSS Radio Occultation]] — TEC is the primary observable extracted from RO occultations
- [[Ionospheric Model Validation]] — TEC is the variable used to compute model error metrics

### Sibling domains

- [[SBAS Integrity]] — TEC uncertainty maps to ionospheric correction uncertainty, which impacts protection level and integrity risk
- [[Protection Levels]] — large TEC gradients can inflate protection levels
- [[Alert Limits]] — TEC anomalies may trigger integrity alerts

### Implementation connection

- [[IRI-2020 vs GNSS-RO Indonesia]] — empirical TEC distributions from Indonesian GNSS-RO
- [[SBAS Ionospheric Threat — Empirical Evidence]] — threat quantification from observed TEC tails and gradients
- [[Source - GNSS-RO Indonesia Empirical Study]] — study-specific TEC statistics

## TEC in SBAS context

### Operational perspective

SBAS ground segments estimate ionospheric delay using dual-frequency ground receiver observations and broadcast corrections as gridded ionospheric vertical delays (GIVDs) or equivalent. The quality of these estimates determines:

- **User position accuracy** — corrected versus uncorrected delay
- **Integrity risk** — probability that the actual delay exceeds the broadcast bound (GIVE)
- **System availability** — whether protection levels remain below alert limits

### Empirical perspective

GNSS-RO provides an independent TEC measurement that can:

1. Validate or invalidate empirical ionospheric models (e.g., IRI-2020)
2. Quantify the tail of TEC delay distributions for threat-model design
3. Characterize spatial TEC gradients that threaten differential correction accuracy

**Critical boundary:** GNSS-RO TEC measures a column along one ray path at one time. SBAS GIVE requires spatial interpolation over many ground-receiver IPPs. These are complementary, not interchangeable.

## Current source anchors

- [[Source - GNSS-RO Indonesia Empirical Study]] — empirical TEC distribution from Indonesian RO data
- [[Source - IRI-2020 Ionosphere Model]] — model-predicted TEC for comparison

## Open provenance questions

- What is the relationship between RO-derived TEC at a tangent point and the vertical IPP TEC used in SBAS grid interpolation?
- Should TEC statistics from sparse RO sampling be treated as conservative (overbounding) or biased (undersampling tails)?
- How do TEC conversion factors vary with geometry, receiver type, and signal frequency?

## See also

- [[GNSS Radio Occultation]]
- [[Ionospheric Model Validation]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[Source - IRI-2020 Ionosphere Model]]
