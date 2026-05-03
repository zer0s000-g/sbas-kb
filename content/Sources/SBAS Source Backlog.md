---
title: SBAS Source Backlog
description: Prioritized source-building backlog for source-disciplined SBAS knowledge-base claims
tags: [sources, backlog, provenance, sbas, research]
created: 2026-04-23
modified: 2026-05-03
status: active
verification_status: internal-backlog-with-public-catalog-corrections
---

# SBAS Source Backlog

## Purpose

This note tracks high-priority source notes needed before draft SBAS claims in the vault are treated as verified research conclusions.

Important boundary:

- This is not itself an authoritative source note.
- It is a provenance-management note built from current vault usage and public-catalog review signals.
- External standards and guidance must still be checked against official source documents before numerical or operational requirements are published.

## 2026-05-02 source-matrix correction

The standards branch now has a dedicated routing page: [[SBAS Standards Source Matrix]].

Public catalog review produced several corrections:

| Reference                                   | Current disposition                                                                                                                                    |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [[Source - RTCA DO-229]]                    | Keep as active GPS/SBAS airborne-equipment source-family anchor; FAA/EASA approval-source notes now split out; official-text extraction still required |
| [[Source - FAA TSO-C145e and TSO-C146e]]    | Active FAA regulator/article-approval routing note; direct TSO text extraction still required                                                          |
| [[Source - EASA ETSO-C145e and ETSO-C146e]] | Active EASA regulator/article-approval routing note with extracted public PDF signals; official section mapping still required                         |
| [[Source - ICAO Doc 9849]]                  | Add as active ICAO GNSS implementation-guidance anchor; direct extraction still required                                                               |
| [[Source - RTCA DO-242]]                    | Red-flag as ADS-B/surveillance related; do not use for SBAS integrity or augmentation claims                                                           |
| [[Source - RTCA DO-289]]                    | Red-flag as aircraft-surveillance related; do not use for SBAS performance-testing or monitoring claims                                                |
| [[Source - ICAO Doc 9854]]                  | Red-flag as Global ATM Operational Concept; do not use for SBAS performance-testing claims                                                             |
| [[Source - ICAO Doc 9855]]                  | Red-flag as public-internet guidance for aeronautical applications; do not use for SBAS technical specifications                                       |

## Priority 1 — build the real standards backbone

### 1. ICAO Annex 10, Volume I GNSS/SBAS material

- Current vault usage: now represented by [[Source - ICAO Annex 10 Volume I GNSS SBAS]] as a public-catalog-reviewed source-family anchor.
- Why this matters: Annex 10, Volume I is the necessary ICAO technical/SARPs source family to investigate for many GNSS/SBAS claims.
- Verification need: move beyond public catalog metadata by extracting the official Annex text, exact edition/amendment baseline, GNSS/SBAS sections, and downstream claim boundaries.
- Current status: Chapter structure from public ICAO presentations added to source note (Chapter 3, Section 3.5 SBAS, Section 3.6 GBAS, Appendix B GNSS technical specifications). Direct extraction of official 8th Edition with Amendment 94 still required.
- Current editorial rule: use the source note for routing only; do not publish detailed Annex-derived requirements until direct extraction is complete.

### 2. [[Source - RTCA DO-229]]

- Current vault usage: airborne GPS/SBAS equipment, LPV-capable equipment context, integrity/protection/alert-limit pages, aviation MOC.
- Why this matters: it is currently the strongest public-product-and-regulatory-signal-reviewed source-family anchor for GPS/SBAS airborne equipment.
- Verification need: direct extraction of official revision-specific equipment classes, intended functions, alerting/integrity language, test methods, exclusions, and the relationship between DO-229F, DO-229E, [[Source - FAA TSO-C145e and TSO-C146e]], and [[Source - EASA ETSO-C145e and ETSO-C146e]].
- Current editorial rule: use DO-229 for receiver/equipment routing only; do not infer installation approval, operational approval, procedure minima, service status, or DFMC requirements.

### 3. FAA/EASA TSO/ETSO approval-source notes

- Current vault usage: now represented by [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]].
- Why this matters: DO-229 equipment-MOPS statements must be separated from jurisdiction-specific article approval, installation approval, and operational approval.
- Verification need: direct FAA TSO-C145e/C146e extraction and deeper EASA section-level mapping before publishing class-specific approval claims.
- Current editorial rule: use these notes for article-approval routing only; do not infer aircraft installation, operational use, procedure availability, or regulator equivalence.

### 4. [[Source - ICAO Doc 9849]]

- Current vault usage: newly added GNSS implementation-guidance anchor.
- Why this matters: it appears to be the appropriate ICAO manual for state GNSS implementation context, replacing several earlier mis-scoped draft references.
- Verification need: direct extraction of SBAS implementation, monitoring/assessment/reporting, DFMC GNSS, RFI mitigation, and Annex 10 relationship language.

### 5. Procedure-design and PBN source family

- Current vault usage: LPV, LNAV/VNAV, RNAV, RNP, and GBAS procedure notes now link to [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] and [[Source - FAA and EASA Procedure-Design and PBN Material]].
- Why this matters: procedure design is now represented by dedicated source notes separating it from equipment MOPS, article approval, and service-provider commitment.
- Verification need: direct extraction of Doc 8168 Vol II (procedure-design criteria), Doc 9613 (RNP navigation specifications), FAA Order 8260.3G/8260.58D (U.S. TERPS/PBN criteria), and EASA AMC/GM (European PBN operational approval).
- Current editorial rule: use these notes for procedure-design routing only; do not infer procedure minima, obstacle-clearance values, or airport/runway eligibility without official text extraction.

### 6. Service-provider source family

- Current vault usage: WAAS, EGNOS, MSAS, GAGAN, BDSBAS regional system pages now link to [[Source - SBAS Service Providers]].
- Why this matters: service commitments, coverage, availability, and system status are provider-specific.
- Verification need: direct extraction of official service-provider documents for each SBAS system before publishing comparative tables.
- Current editorial rule: use [[Source - SBAS Service Providers]] for service-provider routing only; do not infer comparative performance, availability percentages, or interoperability without official service-provider extraction.

## Priority 2 — regional and European framework references

- EUROCAE ED references remain candidates but need exact title/scope verification before being used for EGNOS/SBAS claims.
- APAC, APANPIRG, CNS SG, AIP/AIS, regulator, and ANSP source notes remain important for ASEAN implementation analysis.
- Country-specific readiness claims should continue to use cautious evidence categories unless direct institutional sources support stronger statements.

## Claim clusters that still need direct source support

### Standards mapping

- document titles and editions;
- document scope statements;
- whether a source is airborne-equipment, system-level, procedure-design, service-provider, regulator/ANSP, or implementation guidance;
- whether source material is normative, guidance, catalog metadata, or secondary commentary.

### Performance figures

- horizontal/vertical accuracy numbers;
- continuity and availability percentages;
- alerting or time-to-alert values;
- regional uptime and service-performance figures.

### Operational claims

- LPV/APV capability statements;
- aircraft/equipment eligibility;
- regional operational approval statements;
- procedure availability;
- interoperability claims across WAAS/EGNOS/MSAS/GAGAN and other systems.

## Suggested execution order

1. Directly extract [[Source - ICAO Annex 10 Volume I GNSS SBAS]] from the official Annex text and classify GNSS/SBAS claims by section and amendment baseline.
2. Directly extract the official [[Source - RTCA DO-229]] text and direct FAA TSO-C145e/C146e text; deepen [[Source - EASA ETSO-C145e and ETSO-C146e]] section mapping before publishing class-specific approval statements.
3. Directly extract [[Source - ICAO Doc 9849]].
4. ~~Build procedure-design/PBN source notes.~~ **Completed 2026-05-03**: [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] and [[Source - FAA and EASA Procedure-Design and PBN Material]] now exist as routing anchors; direct text extraction still required.
5. ~~Build service-provider source notes for major SBAS systems.~~ **Completed 2026-05-03**: [[Source - SBAS Service Providers]] now exists as a routing anchor; direct extraction of WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, SouthPAN service definitions still required.
6. Revisit [[SBAS Integrity]], [[Protection Levels]], [[Alert Limits]], and procedure pages with numerical values only after the above source anchors are directly extracted.
7. Continue ASEAN/regional source hardening through [[ASEAN SBAS Source Backlog]].

## Related notes

- [[SBAS Standards Source Matrix]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - FAA TSO-C145e and TSO-C146e]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[SBAS MOC]]
- [[SBAS-Research-MOC]]
- [[SBAS-Standards-Regulation]]
- [[SBAS-vs-Other-Standards]]
- [[SBAS in Civil Aviation MOC]]
- [[ASEAN SBAS Source Backlog]]
