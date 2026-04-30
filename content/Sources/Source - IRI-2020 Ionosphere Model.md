---
title: Source - IRI-2020 Ionosphere Model
description: Starter provenance scaffold for the International Reference Ionosphere 2020 model
tags: [source, iri-2020, ionosphere, model, empirical, standard, provenance]
source_type: model
created: 2026-04-26
modified: 2026-04-26
status: starter
verification_status: metadata-pending
---

# Source - IRI-2020 Ionosphere Model

## Scope of this note

This is a starter source scaffold for the International Reference Ionosphere (IRI) 2020 model.

Boundary:
- It is not a completed model evaluation.
- It does not verify the model's formal specifications against the actual IRI codebase or documentation.
- It exists to anchor model-related claims in the vault to an identifiable source.

## Why this source note matters

The vault contains a systematic validation of IRI-2020 against GNSS-RO observations over Indonesia, finding a 66.72 TECU systematic underestimate. Without a model-level source scaffold, it is unclear whether the version tested matches the standard model, and whether the findings generalize.

## Current in-vault references supported by this scaffold

- [[Ionospheric Model Validation]] — methodology
- [[IRI-2020 vs GNSS-RO Indonesia]] — concrete validation results
- [[SBAS Ionospheric Threat — Empirical Evidence]] — model error as threat input

## Current provisional usage in the vault

At present, this scaffold supports the statement that:
- IRI-2020 is an international standard empirical ionospheric model maintained by the IRI Working Group
- It was validated against GNSS-RO data over Indonesia in the vault's empirical study
- The model showed significant systematic underestimation of TEC in the Indonesian equatorial region

It does not yet support:
- Any claim that IRI-2020 is “wrong” in an absolute sense — the findings are regionally and conditionally specific
- Any ranking of IRI-2020 against NeQuick, SAMI3, or physics-based models
- Any claim that IRI-2020 is unsuitable for all SBAS applications globally

## Immediate audit questions

- Which IRI-2020 implementation was used (Python, MATLAB, online)?
- Which model options were active (storm model, F10.7 source, hmF2 model)?
- What are the inherent temporal and spatial resolutions of the model?
- How does IRI-2020 implement the equatorial ionization anomaly (EIA)?
- Which model version is current relative to the vault's study date?

## Suggested downstream cleanup targets

If this scaffold becomes source-backed, revisit and tighten claims in:
- [[Ionospheric Model Validation]]
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]

## Extraction template for next cycle

- Model version and release date
- Implementation language/library
- Active options and default settings tested
- Published validation literature for low-latitude regions
- Relationship between IRI TEC predictions and SBAS ionospheric correction design
- Known limitations for equatorial and post-sunset conditions

## See also

- [[Ionospheric Model Validation]]
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[SBAS Source Backlog]]
