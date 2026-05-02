---
title: Source - ICAO Annex 10 Volume I GNSS/SBAS
description: Source note for ICAO Annex 10 Volume I as the public-catalog-reviewed ICAO SARPs and technical-provisions anchor for GNSS and SBAS claim routing
aliases:
  - Source - ICAO Annex 10 Volume I GNSS SBAS
  - ICAO Annex 10 Volume I GNSS/SBAS
  - Annex 10 Volume I GNSS/SBAS
tags: [source, icao, annex-10, volume-i, gnss, sbas, sarps, standards]
source_type: annex
created: 2026-05-02
modified: 2026-05-02
status: active
verification_status: public-catalog-reviewed-not-source-extracted
---

# Source - ICAO Annex 10 Volume I GNSS/SBAS

## Scope of this note

This note establishes ICAO Annex 10, Volume I as the knowledge base's current public-catalog-reviewed source-family anchor for ICAO radio-navigation SARPs and technical provisions relevant to GNSS and SBAS.

It is an institutional source-routing note. It is not a completed extraction from the secured ICAO publication and must not be treated as a substitute for the official Annex text.

Important boundary:

- Public ICAO Store metadata can support document identity, edition/amendment signals, broad scope, and access/licensing constraints.
- Public catalog metadata cannot support detailed SBAS message definitions, numerical performance requirements, alert-limit values, receiver behavior, procedure minima, aircraft eligibility, or operational approval decisions.
- Detailed claims must still be checked against the official Annex 10 text, applicable amendments, ICAO manuals, RTCA/EUROCAE equipment standards, PANS-OPS/PBN sources, regulator/ANSP material, AIP/AIS publications, service-provider documentation, aircraft/avionics approvals, and operator procedures.

## Public-catalog identity signal

| Field                          | Current public signal                                                                       |
| ------------------------------ | ------------------------------------------------------------------------------------------- |
| Issuing body                   | International Civil Aviation Organization (ICAO)                                            |
| Publication family             | Annex 10 — Aeronautical Telecommunications                                                  |
| Volume                         | Volume I                                                                                    |
| Title                          | Radio Navigational Aids                                                                     |
| Edition signal                 | 8th Edition, July 2023                                                                      |
| Amendment signal               | Includes Amendment 94; separate Amendment no. 94 dated 04/08/25 is listed by the ICAO Store |
| Publication type               | Annex                                                                                       |
| Order number                   | AN 10-1                                                                                     |
| Public source reviewed         | ICAO Store product and Annex 10 catalog pages                                               |
| Verification status in this KB | Public catalog reviewed; official source text not extracted                                 |

## Publicly visible scope signal

The ICAO Store describes Annex 10, Volume I as a technical document defining, for international aircraft operations, the systems needed to provide radio navigation aids used by aircraft in all phases of flight.

The public description identifies the volume as containing SARPs and guidance material with essential parameter specifications for radio-navigation aids, including:

- Global Navigation Satellite System (GNSS);
- Instrument Landing System (ILS);
- Microwave Landing System (MLS);
- VHF Omnidirectional Radio Range (VOR);
- Non-Directional Radio Beacon (NDB);
- Distance Measuring Equipment (DME).

The same public description identifies technical-parameter areas such as power requirements, frequency, modulation, signal characteristics, and monitoring.

For this knowledge base, the institutional implication is narrow but important: Annex 10, Volume I is the correct ICAO source family to route GNSS/SBAS SARPs and technical-provisions questions. It is not, by itself, a visible public source for any specific numerical SBAS claim until the official text is extracted and classified.

## Why this source matters for SBAS

SBAS documentation often mixes four different source families:

1. ICAO SARPs and technical provisions;
2. ICAO implementation guidance;
3. airborne equipment standards;
4. operational approval, procedure-design, service-provider, and regulator sources.

Annex 10, Volume I belongs primarily to the first family. It should be used to route questions about the ICAO technical baseline for radio navigation aids, GNSS, and augmentation provisions.

It should be paired with:

- [[Source - ICAO Doc 9849]] for GNSS implementation-guidance context;
- [[Source - RTCA DO-229]] for GPS/SBAS airborne-equipment MOPS routing;
- future procedure-design/PBN source notes for LPV, LNAV/VNAV, RNAV, RNP, and related procedure criteria;
- service-provider and regulator/ANSP/AIP sources for actual operational status, procedure availability, approvals, and service commitments.

## What this source can currently anchor

Until direct official-text extraction is complete, this note can safely anchor only source-family and document-identity statements such as:

- ICAO Annex 10, Volume I is the ICAO Annex volume for Radio Navigational Aids.
- The current public ICAO Store signal identifies the relevant base publication as the 8th Edition, July 2023, including Amendment 94.
- Public ICAO Store metadata explicitly includes GNSS among the radio-navigation-aid systems covered by Volume I.
- Annex 10, Volume I is the appropriate ICAO SARPs/technical-provisions source family to investigate for GNSS/SBAS requirements.
- Concept pages should route normative GNSS/SBAS technical claims to Annex 10 rather than to mis-scoped sources such as Doc 9854, Doc 9855, DO-242, or DO-289.

## What this source must not be used for yet

Do not use this note alone to publish or validate:

- exact SBAS message types, parameter values, or signal specifications;
- exact alert limits, time-to-alert values, continuity, availability, or accuracy requirements;
- receiver mode eligibility, equipment classes, annunciation behavior, or test methods;
- LPV, LNAV/VNAV, RNAV, RNP, or GBAS procedure-design criteria;
- aircraft certification, operational approval, or crew authorization statements;
- country-specific procedure availability or service status;
- service-provider performance commitments or outage/status practices.

Those claims require direct source extraction and, in many cases, more than one source family.

## Relationship to other source notes

| Related source                   | Relationship                                                                                                      |
| -------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| [[SBAS Standards Source Matrix]] | Current routing table for deciding which source family can support which claim type                               |
| [[Source - ICAO Doc 9849]]       | ICAO GNSS implementation manual; complements Annex 10 but does not replace SARPs/technical provisions             |
| [[Source - RTCA DO-229]]         | GPS/SBAS airborne-equipment MOPS source-family anchor; not a substitute for Annex 10 system-level ICAO material   |
| [[Source - ICAO Doc 9854]]       | Red-flag note; ATM operational concept, not an SBAS performance-testing or GNSS/SBAS technical-provisions anchor  |
| [[Source - ICAO Doc 9855]]       | Red-flag note; public-internet guidance for aeronautical applications, not an SBAS technical specification anchor |
| [[Source - RTCA DO-242]]         | Red-flag note; ADS-B/surveillance related, not an SBAS integrity source                                           |
| [[Source - RTCA DO-289]]         | Red-flag note; aircraft surveillance applications related, not an SBAS monitoring/testing source                  |

## Downstream claim-routing rules

When editing downstream SBAS pages:

1. Use this note to identify Annex 10, Volume I as the ICAO SARPs/technical-provisions source family for GNSS/SBAS questions.
2. Do not paraphrase detailed Annex content unless the official text has been extracted, section-referenced, and checked against the edition/amendment baseline.
3. Keep numerical values out of public concept pages unless each value has a visible source, applicability condition, date/revision, and operational context.
4. Route receiver/equipment requirements to RTCA/EUROCAE and regulator material, not to Annex 10 alone.
5. Route procedure minima and design criteria to PANS-OPS/PBN/regulator/AIP sources, not to Annex 10 alone.
6. Route service availability and system-status claims to service-provider, regulator/ANSP, and AIP/AIS sources.

## Extraction template for a future direct-source cycle

### Bibliographic metadata

- exact edition:
- amendment baseline:
- effective/applicability dates:
- access path / institutional library record:
- relevant chapters and attachments:
- relationship to Doc 9849 and other ICAO GNSS guidance:

### Sections to extract cautiously

- GNSS system-level provisions;
- SBAS-specific provisions and definitions;
- signal and message characteristics;
- integrity, monitoring, alerting, and performance language;
- compatibility/interoperability provisions;
- DFMC GNSS/SBAS material, if present in the applicable amendment baseline;
- notes distinguishing SARPs, guidance material, and explanatory text.

### Downstream mapping questions

- Which SBAS architecture claims can be tied directly to Annex 10?
- Which integrity/protection-level/alert-limit statements require Annex 10 plus receiver standards?
- Which LPV statements require procedure-design or regulator material instead of Annex 10?
- Which regional implementation claims require service-provider, ANSP, AIP/AIS, or state-regulator evidence?
- Which claims should remain conceptual until official source text is available?

## Public sources reviewed

- ICAO Store, Annex 10 - Aeronautical Telecommunications - Volume I - Radio Navigational Aids: `https://store.icao.int/en/annex-10-aeronautical-telecommunications-volume-i-radio-navigational-aids`
- ICAO Store, Annex 10 - Aeronautical Telecommunications - Volume I - Radio Navigational Aids, Amendment no. 94 dated 04/08/25: `https://store.icao.int/en/annex-10-aeronautical-telecommunications-volume-i-radio-navigational-aids-amendment-no-94-dated-04-08-25`
- ICAO Store, Annex 10 catalog page: `https://store.icao.int/en/annexes/annex-10`

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[Source - ICAO Doc 9849]]
- [[Source - RTCA DO-229]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[What is SBAS]]
