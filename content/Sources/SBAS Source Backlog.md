---
title: SBAS Source Backlog
description: Prioritized source-building backlog for source-disciplined SBAS knowledge-base claims
tags: [sources, backlog, provenance, sbas, research]
created: 2026-04-23
modified: 2026-05-04
status: active
verification_status: internal-backlog-with-public-catalog-corrections-and-second-layer-core-routing
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

## 2026-05-03 core-knowledge routing update

The core SBAS layer now has a dedicated routing note: [[SBAS Core Claim Routing]].

This update intentionally skipped new FAA-specific extraction per user instruction. Existing FAA-related source notes remain in the vault as historical/routing anchors where already present, but the current core-solidification block did not deepen FAA procedure, TSO, NFDC, or service-provider evidence.

Core concept pages should now use this ownership model:

| Claim family                             | Owner note                                                     | Editorial boundary                                                                    |
| ---------------------------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| SBAS definition and beginner orientation | [[What is SBAS]]                                               | High-level explanation only; no numerical operational requirements                    |
| Architecture                             | [[SBAS Architecture]] and [[SBAS Architecture Flow]]           | System chain only; standards/service-provider details stay in source notes            |
| Signal/message flow                      | [[SBAS Signal and Message Flow]]                               | Flow explanation only; no message-number or bit-field claims without Annex extraction |
| Correction versus integrity              | [[SBAS Corrections and Integrity Separation]]                  | Accuracy-improvement claims must not be treated as safety/approval claims             |
| Ground versus airborne responsibility    | [[SBAS Ground Segment and Airborne Receiver Responsibilities]] | Separate service, receiver, procedure, aircraft, and operator layers                  |
| Protection and alerting                  | [[Protection Levels]], [[Alert Limits]], [[SBAS Integrity]]    | Explain relationships without unsupported numerical thresholds                        |
| Service performance concepts             | [[SBAS Service Performance Concepts]]                          | Separate accuracy, integrity, availability, continuity, coverage, and commitments     |
| Service volume and coverage              | [[SBAS Service Volume and Coverage]]                           | Coverage is not procedure publication, aircraft eligibility, or operator approval     |
| Approach capability labels               | [[SBAS Approach Capability Taxonomy]]                          | LP/LPV/LNAV/VNAV labels are not operational proof by themselves                       |
| Standards-to-operations escalation       | [[SBAS Standards to Operations Evidence Ladder]]               | Each evidence layer must be sourced before moving upward                              |
| Receiver modes and annunciation          | [[SBAS Receiver Modes and Annunciation]]                       | No cockpit, MOPS, timing, or pilot-action details without direct source extraction    |

## 2026-05-04 second-layer core-routing update

The second core-solidification pass added five routing notes to close remaining conceptual gaps without using long reference-website expansion:

- [[SBAS Service Performance Concepts]]
- [[SBAS Service Volume and Coverage]]
- [[SBAS Approach Capability Taxonomy]]
- [[SBAS Standards to Operations Evidence Ladder]]
- [[SBAS Receiver Modes and Annunciation]]

This update intentionally keeps the new pages at concept/routing level. It does not add numerical service-performance values, message tables, alerting timing, cockpit actions, receiver algorithms, procedure minima, or state-specific operational claims.

The pass also hardened [[SBAS Ionospheric Threat — Empirical Evidence]] so empirical GNSS-RO/TEC evidence remains threat-discovery evidence rather than operational correction, GIVE, service-volume, or approval evidence.

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
- Current status: Chapter/section structure added to source note (Section 1 general requirements, Section 2 Class Beta/Gamma/Delta equipment standards, avionics Class 1–4 capability table, DFMC boundary, PRN code expansion context, ICAO Annex 10 cross-reference). Direct extraction of official RTCA DO-229F text still required.

### 3. FAA/EASA TSO/ETSO approval-source notes

- Current vault usage: now represented by [[Source - FAA TSO-C145e and TSO-C146e]] and [[Source - EASA ETSO-C145e and ETSO-C146e]].
- Why this matters: DO-229 equipment-MOPS statements must be separated from jurisdiction-specific article approval, installation approval, and operational approval.
- Verification need: direct FAA TSO-C145e/C146e extraction and deeper EASA section-level mapping before publishing class-specific approval claims.
- Current editorial rule: use these notes for article-approval routing only; do not infer aircraft installation, operational use, procedure availability, or regulator equivalence.

### 4. [[Source - ICAO Doc 9849]]

- Current vault usage: newly added GNSS implementation-guidance anchor.
- Why this matters: it appears to be the appropriate ICAO manual for state GNSS implementation context, replacing several earlier mis-scoped draft references.
- Verification need: direct extraction of SBAS implementation, monitoring/assessment/reporting, DFMC GNSS, RFI mitigation, and Annex 10 relationship language.
- Current status: Chapter structure added from 5 public ICAO sources (Chapter 1–7 from 2nd Ed.; confirmed/revised for 4th Ed./5th Ed.; Chapter 5 GNSS Vulnerability confirmed in 5th Ed.; S1–S7 spoofing classification confirmed; GALILEO/BDS confirmed operational in 4th Ed. Chapter 3). Direct extraction of official 5th Edition text still required.

### 5. Procedure-design and PBN source family

- Current vault usage: LPV, LNAV/VNAV, RNAV, RNP, and GBAS procedure notes now link to [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] and [[Source - FAA and EASA Procedure-Design and PBN Material]].
- Why this matters: procedure design is now represented by dedicated source notes separating it from equipment MOPS, article approval, and service-provider commitment.
- Verification need: direct extraction of Doc 8168 Vol II (procedure-design criteria), Doc 9613 (RNP navigation specifications), FAA Order 8260.3G/8260.58D (U.S. TERPS/PBN criteria), and EASA AMC/GM (European PBN operational approval).
- Current editorial rule: use these notes for procedure-design routing only; do not infer procedure minima, obstacle-clearance values, or airport/runway eligibility without official text extraction.

### 6. Service-provider source family

- Current vault usage: WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, SouthPAN, and SDCM regional system pages now link to [[Source - SBAS Service Providers]]. Dedicated child source notes now exist for [[Source - WAAS]], [[Source - EGNOS]], [[Source - GAGAN SBAS Operation]], [[Source - MSAS]], [[Source - BDSBAS]], [[Source - KASS]], [[Source - SouthPAN]], and [[Source - SDCM]]. Use [[SBAS Operational Validation Dashboard]] before upgrading any service-provider evidence into operational aviation claims.
- Why this matters: service commitments, coverage, availability, and system status are provider-specific.
- Verification need: continue deeper official service-provider/regulator/AIP extraction before publishing comparative tables, service-volume boundaries, procedure availability, or operational-approval claims.
- Current status: Partial direct extraction completed for WAAS (FAA WAAS page + August 2025 quick facts), EGNOS (official SoL SDD page + Issue 3.6 PDF), GAGAN (ICAO APAC ITF/7 IP05b + AAI GEO FAQ), MSAS (QZSS service page + ICAO APAC CNS SG/24 IP15), SouthPAN (official FAQ, early Open Services factsheet, Signal-In-Space service definition), BDSBAS (official BDSBAS-B1C ICD + bounded technical-public context), KASS (KARI official page + ICAO APAC ITF/5 IP/09 + bounded contractor-public certification signal), and SDCM (GLONASS IAC / OS PS source posture plus historical ICAO development-context evidence).
- Current editorial rule: use [[Source - SBAS Service Providers]] for service-provider routing; use dedicated child source notes only within their stated boundaries; do not infer comparative performance, availability percentages, interoperability, operational approval, or procedure minima without official service-provider/regulator/AIP extraction.

### 7. Core SBAS concept routing

- Current vault usage: [[What is SBAS]], [[SBAS Architecture]], [[SBAS Architecture Flow]], [[SBAS Signal and Message Flow]], [[SBAS Corrections and Integrity Separation]], [[SBAS Ground Segment and Airborne Receiver Responsibilities]], [[SBAS Service Performance Concepts]], [[SBAS Service Volume and Coverage]], [[SBAS Approach Capability Taxonomy]], [[SBAS Standards to Operations Evidence Ladder]], [[SBAS Receiver Modes and Annunciation]], [[SBAS Integrity]], [[Protection Levels]], [[Alert Limits]], [[Ionospheric Model Validation]], [[Total Electron Content (TEC)]], and [[SBAS Ionospheric Threat — Empirical Evidence]].
- Why this matters: core concept pages are high-traffic entry points; if they duplicate standards, service-provider, procedure, or operational claims, the KB will accumulate overlapping and stale knowledge.
- Verification need: direct Annex 10 / DO-229 / Doc 9849 extraction before adding exact message, integrity, alerting, protection-level, or operational threshold values.
- Current status: [[SBAS Core Claim Routing]] now owns the editorial routing model for core claims. Core notes now cover message flow, correction/integrity separation, ground/airborne responsibility separation, service-performance concepts, service volume/coverage, approach-capability taxonomy, standards-to-operations escalation, and receiver modes/annunciation.
- Current editorial rule: keep concept pages explanatory and source-routed; never promote a concept explanation into procedure availability, aircraft eligibility, service commitment, or numerical requirement without the primary source family.

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
2. Directly extract the official [[Source - RTCA DO-229]] text and deepen non-FAA article-approval routing where needed; direct FAA extraction and long reference-website expansion are skipped in the current core-solidification scope.
3. Directly extract [[Source - ICAO Doc 9849]].
4. ~~Build procedure-design/PBN source notes.~~ **Completed 2026-05-03**: [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]] and [[Source - FAA and EASA Procedure-Design and PBN Material]] now exist as routing anchors; direct text extraction still required.
5. ~~Build service-provider source notes for major SBAS systems.~~ **Substantially completed 2026-05-03 for the current major-system set**: [[Source - SBAS Service Providers]] exists as the family routing anchor; direct child-source extraction/source-posture notes now exist for [[Source - WAAS]], [[Source - EGNOS]], [[Source - GAGAN SBAS Operation]], [[Source - MSAS]], [[Source - BDSBAS]], [[Source - KASS]], [[Source - SouthPAN]], and [[Source - SDCM]]. Remaining work is deeper service-provider/regulator/AIP extraction, not first-layer child-source creation. Use [[SBAS Operational Validation Dashboard]] to prevent child source notes from being misused as operational approval evidence.
6. Use [[SBAS Core Claim Routing]] before editing core concept pages; keep architecture, signal/message flow, correction/integrity separation, ground/airborne responsibility, protection-level, and alert-limit claims atomic and non-overlapping.
7. Revisit [[SBAS Integrity]], [[Protection Levels]], [[Alert Limits]], and procedure pages with numerical values only after the above source anchors are directly extracted.
8. Continue ASEAN/regional source hardening through [[ASEAN SBAS Source Backlog]].

## Related notes

- [[SBAS Standards Source Matrix]]
- [[SBAS Core Claim Routing]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - FAA TSO-C145e and TSO-C146e]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[Source - WAAS]]
- [[Source - EGNOS]]
- [[Source - BDSBAS]]
- [[Source - KASS]]
- [[Source - SDCM]]
- [[SBAS Operational Validation Dashboard]]
- [[SBAS MOC]]
- [[SBAS-Research-MOC]]
- [[SBAS-Standards-Regulation]]
- [[SBAS-vs-Other-Standards]]
- [[SBAS in Civil Aviation MOC]]
- [[ASEAN SBAS Source Backlog]]
