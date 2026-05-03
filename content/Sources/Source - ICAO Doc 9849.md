---
title: Source - ICAO Doc 9849
description: Source note for ICAO Doc 9849, Global Navigation Satellite System (GNSS) Manual, as an implementation-guidance anchor for GNSS/SBAS context
tags: [source, icao, doc-9849, gnss, sbas, implementation, guidance]
source_type: manual
created: 2026-05-02
modified: 2026-05-03
status: active
verification_status: public-catalog-reviewed-not-source-extracted
---

# Source - ICAO Doc 9849

## Scope of this note

This note introduces ICAO Doc 9849 as the knowledge base's current public-catalog-reviewed anchor for ICAO GNSS implementation guidance. It is not a completed extraction from the manual itself.

Important boundary:

- Public ICAO Store metadata can support document identity and broad purpose.
- It cannot support detailed operational requirements, numerical alert limits, procedure minima, receiver performance thresholds, or state-specific implementation decisions.
- Use this note as an implementation-guidance anchor, not as a substitute for ICAO Annex 10, PANS-OPS, regulator material, service-provider definitions, AIPs, aircraft approvals, or operator approvals.

## Public-catalog identity signal

|| Field | Current ICAO Store signal |
||---|---|
|| Issuing body | ICAO |
|| Document | Doc 9849 |
|| Title | Global Navigation Satellite System (GNSS) Manual |
|| Publication type | Manual |
|| Edition signal | 5th Edition, 2025 |
|| Purpose signal | Provide information on GNSS implementation aspects to assist States in introducing GNSS operations |
|| Companion-source signal | The catalog describes it as used in conjunction with Annex 10, Volume I |
|| New-material signal | Public catalog text mentions DFMC GNSS, GNSS performance monitoring/assessment/reporting, and radiofrequency interference detection/mitigation in the 5th edition |

## Chapter structure signals (from public ICAO sources)

The GNSS Manual has evolved through multiple editions. Public ICAO working papers, workshop materials, and secondary editions provide the following chapter structure signals:

### Chapter 1 — Introduction (from 2nd Ed., 2012)

Signal source: ICAO Doc 9849 2nd Edition (Yumpu advance unedited edition)

General introduction to GNSS and early stages of GNSS implementation in aviation.

### Chapter 2 — Performance Requirements

Signal sources: ICAO PBNICG/11 WP04 (4th Ed. update summary); ICAO Store catalog

Chapter 2 was reviewed in the 4th Edition (2023) for changes related to new DFMC SBAS standards. Section 2.3 now includes guidance material on GNSS performance reporting for GNSS service providers. This chapter establishes the navigation performance framework that underpins GNSS-based operations.

### Chapter 3 — Existing Core Satellite Constellations

Signal source: ICAO PBNICG/11 WP04 (4th Ed. update summary)

Updated in the 4th Edition (2023) to reflect new operational core constellations and new signals for existing constellations. GALILEO and BDS were confirmed as operational and moved into this chapter from the planned-constellations section.

### Chapter 4 — Augmentation Systems

Signal sources: ICAO PBNICG/11 WP04 (4th Ed. update summary); Yumpu 2nd Ed. chapter listing; ICAO EUR/NAT RFI Workshop

Updated in the 4th Edition (2023) to address DFMC SBAS SARPs changes and identify new SBASs included in the SBAS SARPs amendment. Information was added to support SBAS-based operations implementation. The 2nd Edition content identified SBAS (GIVE/ionospheric grid points) and GBAS (datalink, 200 ft DH displacement) as the primary augmentation system topics.

### Chapter 5 — GNSS Vulnerability

Signal sources: ICAO PBNICG/11 WP04 (4th Ed. update summary); ICAO EUR/NAT RFI Workshop (5th Ed. briefing)

Chapter 5 was reorganized in the 4th Edition to better separate interference from environmental effects (ionosphere and troposphere errors). Significant material was added on recent developments in jamming and spoofing. A new Section 5.1.3 was added on characterization of jamming and spoofing, consistent with past NSP papers.

The 5th Edition (2025) was confirmed as retaining the GNSS Vulnerability chapter designation. Public ICAO EUR/NAT workshop materials referencing the 5th Edition explicitly cite Chapter 5 as the location of GNSS Vulnerability guidance.

**Spoofing classification (from Doc 9849 — per ICAO EUR/NAT RFI Workshop):**

- S1: Repeaters — unintentional rebroadcast of genuine GNSS signals with slight delay
- S2: Errant signals — unintentional caused by faulty, misused, or misconfigured equipment
- S3: Collateral spoofers simulators — collateral GNSS simulators emitting artificial signals
- S4: Collateral re-radiating spoofers — collateral re-radiation of real GNSS signal in real-time
- S5: Targeted spoofers — purpose-built transmitters generating false GNSS signals
- S6: Targeted re-radiating spoofers — targeted re-radiation of real GNSS signal in real-time
- S7: Targeted sophisticated spoofers — multiple coordinated signals from different directions

### Chapter 6 — GNSS Evolutions

Signal source: ICAO PBNICG/11 WP04 (4th Ed. update summary)

Updated in the 4th Edition (2023). Section 6.5 was updated to reflect the operational state of GALILEO and BDS plus their planned future evolutions. The GPS paragraph was updated to reflect current planned dates for new services. Section 6.6 (Planned New Core Constellations) was marked reserved as GALILEO and BDS information moved to Chapter 3.

### Chapter 7 — GNSS Implementation

Signal sources: ICAO PBNICG/11 WP04 (4th Ed. update summary); Yumpu 2nd Ed. chapter listing

Chapter 7 is the implementation guidance chapter. The 4th Edition (2023) added or updated:

- Interference monitoring and anomaly reporting
- Space weather advisory
- DFMC-related implementation issues
- Section 7.8.3 (GNSS Performance Assessment): core constellation performance parameters updated; new integrity parameters added
- SBAS-based approach procedure guidance material, pending DO-259 MOPS publication
- Sections 7.8.2, 7.8.3, and 7.8.5: guidance material for States and GNSS service provider organizations regarding regular performance assessment

The 2nd Edition (2012) content covered: Concept of Operations; Business Case; reduced costs/replaceable components; equipage (non-IFR receivers); airspace planning; service provider considerations; ATC/controller actions; procedural mitigations; near-normal service requirements.

### Appendix structure (from 2nd Ed.; confirmed partially in 4th Ed.)

Signal source: Yumpu 2nd Ed.; ICAO PBNICG/11 WP04

|| Appendix | Content signal |
||---|---|
|| Appendix A | Acronyms and abbreviations |
|| Appendix B | References, including RTCA/DO-201A and EUROCAE ED-77 |
|| Appendix C | ANSP regulatory material; core constellation frequency figures (updated in 4th Ed.) |
|| Appendix D | GNSS Spectrum (removed from 4th Ed. — reserved) |
|| Appendix E | Reserved |
|| Appendix F | PBN Roadmap (removed from 4th Ed. — determined adequately covered elsewhere; reserved) |

## What this source can currently anchor

Until direct manual extraction is performed, this note can support broad routing statements such as:

- ICAO Doc 9849 is an ICAO GNSS implementation manual.
- It is relevant to state introduction of GNSS operations and GNSS-based services.
- It is a better high-level ICAO GNSS/SBAS context anchor than the previously mis-scoped Doc 9854 and Doc 9855 references.
- It should be paired with Annex 10, Volume I and operational/regulatory sources before publishing normative aviation requirements.

## What this source must not be used for yet

Do not use this note alone to publish:

- exact LPV minima or alert-limit values;
- receiver MOPS requirements;
- service availability commitments;
- aircraft eligibility or crew authorization statements;
- state approval status;
- procedure-design criteria.

## Relationship to red-flagged documents

| Mis-scoped source in earlier drafts | Current correction                                                                        |
| ----------------------------------- | ----------------------------------------------------------------------------------------- |
| [[Source - ICAO Doc 9854]]          | ATM operational concept, not SBAS performance-testing standard                            |
| [[Source - ICAO Doc 9855]]          | Public-internet guidance for aeronautical applications, not SBAS technical specifications |
| [[Source - RTCA DO-242]]            | ADS-B / surveillance standard signal, not SBAS augmentation-system source                 |
| [[Source - RTCA DO-289]]            | Aircraft surveillance applications signal, not SBAS performance-testing source            |

## Downstream pages to connect

- [[SBAS Standards Source Matrix]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS Integrity]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]

## Extraction template for a future direct-source cycle

### Bibliographic metadata

- issuing body: ICAO
- exact title: Global Navigation Satellite System (GNSS) Manual
- document number: Doc 9849, AN/457
- edition: 5th Edition, 2025
- amendment/update status: incorporates amendments to SARPs; companion document to Annex 10 Volume I
- publication date: 2025
- access path: ICAO Store (store.icao.int)
- relevant chapters: Chapter 2 (Performance Requirements), Chapter 3 (Core Constellations), Chapter 4 (Augmentation Systems), Chapter 5 (GNSS Vulnerability), Chapter 6 (GNSS Evolutions), Chapter 7 (GNSS Implementation)

### Sections to extract cautiously

**From Chapter 2 — Performance Requirements:**

- DFMC SBAS standards and navigation performance framework
- Section 2.3: GNSS performance reporting guidance for service providers
- relationship to Annex 10 Volume I performance requirements

**From Chapter 3 — Existing Core Satellite Constellations:**

- GALILEO and BDS operational status confirmation
- new signals for existing constellations
- relationship to DFMC SBAS requirements

**From Chapter 4 — Augmentation Systems:**

- DFMC SBAS SARPs changes in 4th Edition
- new SBASs added to SBAS SARPs amendment
- SBAS-based operations implementation guidance
- GIVE/ionospheric grid point definitions and parameters
- GBAS datalink and Category I/II/III approach considerations

**From Chapter 5 — GNSS Vulnerability:**

- jamming and spoofing characterization (S1–S7 classification)
- interference detection and mitigation
- ionospheric effects and error characterization
- tropospheric effects and error characterization
- real-time GNSS monitoring and analysis systems
- interference anomaly reporting mechanisms (SIRRS)

**From Chapter 6 — GNSS Evolutions:**

- GALILEO and BDS planned future evolutions
- GPS planned new services and modernization dates
- transition material between current and planned GNSS capabilities

**From Chapter 7 — GNSS Implementation:**

- interference monitoring and anomaly reporting procedures
- space weather advisory integration
- DFMC-related implementation issues
- Section 7.8.2: guidance material for States and service provider organizations
- Section 7.8.3: GNSS Performance Assessment (core constellation performance parameters; new integrity parameters)
- Section 7.8.5: regular performance assessment guidance
- SBAS-based approach procedure guidance (pending DO-259 MOPS publication)
- State implementation responsibilities
- SBAS service introduction and operational considerations

**Explicit boundaries (do not extract as normative requirements):**

- Numerical alert-limit and protection-level values (route to Annex 10 and DO-229)
- Receiver MOPS requirements (route to RTCA DO-229)
- Procedure minima and operational approval criteria (route to PANS-OPS/PBN and regulator sources)

### Downstream claim mapping

- Which concepts can use Doc 9849 as guidance?
- Which claims require Annex 10 rather than Doc 9849?
- Which claims require RTCA/EUROCAE airborne-equipment standards?
- Which claims require regulator, service-provider, AIP, or operator evidence?

## Public sources reviewed

- ICAO Store, Doc 9849 product page: `https://store.icao.int/en/doc-9849-global-navigation-satellite-system-gnss-manual`
- ICAO PBNICG/11 WP04 (Doc 9849 4th Ed. update summary, March 2024): `https://www.icao.int/sites/default/files/APAC/Meetings/2024/2024%20PBNICG-11/3-Working%20Papers/WP04-DOC-9849-GNSS-Manual-Update-Summary-Secretariat.pdf`
- ICAO EUR/NAT MID GNSS RFI Workshop briefing on Chapter 5 GNSS Vulnerability (November 2025): `https://www.icao.int/sites/default/files/MID/MeetingDocs/2025/EURNAT%20-%20MID%20Workshop%20-%20GNSS/Presentations/Day%201/1.2%20ICAO%20EUR%20NAT%20briefing%20on%20GNSS%20RFI.pdf`
- ICAO SRWG/10 WP13 (5th Edition updates and GNSS RFI management, February 2026): `https://www.icao.int/sites/default/files/APAC/Meetings/2026/2026%20SRWG10/3-Working%20Papers/WP13_ICAO-AI.6.2-Updates-on-GNSS-RFI-matters-and-its-future-management.pdf`
- ICAO Doc 9849 2nd Edition advance unedited version (Yumpu, 2012): `https://www.yumpu.com/en/document/view/10363441/global-navigation-satellite-system-gnss-manual-icao`

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[SBAS-Standards-Regulation]]
- [[SBAS MOC]]
