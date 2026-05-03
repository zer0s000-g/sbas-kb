---
title: Source - GNSS Radio Occultation Technique
description: Starter provenance scaffold for GNSS Radio Occultation as a technique for ionospheric sounding
tags: [source, gnss-ro, technique, ionosphere, satellite, spire, cosmic-2, cdaac, provenance]
source_type: technique
created: 2026-04-26
modified: 2026-04-26
status: starter
verification_status: metadata-pending
---

# Source - GNSS Radio Occultation Technique

## Scope of this note

This is a starter source scaffold for GNSS Radio Occultation as an ionospheric observational technique.

Boundary:

- It is not a completed literature review.
- It does not verify the accuracy, calibration, or operational readiness of any specific RO constellation.
- It exists to anchor technique claims in the vault to identifiable datasets and literature.

## Why this source note matters

The vault contains empirical ionospheric analysis derived from GNSS-RO data. Without a technique-level source scaffold, it is unclear which data products, constellations, and processing pipelines support the claims.

## Current in-vault references supported by this scaffold

- [[GNSS Radio Occultation]] — technique definition
- [[Source - GNSS-RO Indonesia Empirical Study]] — specific application
- [[IRI-2020 vs GNSS-RO Indonesia]] — validation comparison
- [[ASEAN SBAS Deployment Barriers]] — ionospheric barrier framing

## Current provisional usage in the vault

At present, this scaffold supports only the statement that:

- GNSS Radio Occultation provides an independent empirical measurement of ionospheric TEC from low-Earth-orbiting satellites
- Spire/COSMIC-2 podTec data from UCAR CDAAC was used for the Indonesian empirical study
- RO-based TEC is a threat-discovery proxy, not a certified SBAS correction source

It does not yet support:

- Any claim that RO TEC is interchangeable with ground GNSS IPP TEC
- Any quantified accuracy specification for Spire podTec vs other datasets
- Any operational readiness assessment for RO-based SBAS service

## Immediate audit questions

- Which Spire data product version was used (Level 1, 2, or higher)?
- What is the published calibration accuracy of podTec versus ground-truth TEC?
- How do UCAR CDAAC quality-control flags affect the usable profile count?
- What is the spatial footprint of a single RO tangent point relative to SBAS grid cell size?

## Suggested downstream cleanup targets

If this scaffold becomes source-backed, revisit and tighten claims in:

- [[GNSS Radio Occultation]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[ASEAN SBAS Deployment Barriers]]

## Extraction template for next cycle

- Verified dataset/product name and version
- Constellation and instrument specifications
- Data provider and access path
- Published accuracy/bias specifications
- Quality-control flag definitions
- Relationship between RO TEC geometry and SBAS IPP geometry

## See also

- [[GNSS Radio Occultation]]
- [[Source - GNSS-RO Indonesia Empirical Study]]
- [[Source - IRI-2020 Ionosphere Model]]
- [[IRI-2020 vs GNSS-RO Indonesia]]
- [[ASEAN SBAS Deployment Barriers]]
- [[ASEAN SBAS Source Backlog]]
