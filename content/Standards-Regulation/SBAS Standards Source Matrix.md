---
title: SBAS Standards Source Matrix
description: Institutional standards/source matrix classifying SBAS claims by source family, evidence status, and safe downstream use
tags: [standards, sources, matrix, sbas, integrity, aviation, provenance]
category: standards
created: 2026-05-02
modified: 2026-05-02
status: reviewed
verification_status: public-catalog-reviewed-with-open-source-extraction
---

# SBAS Standards Source Matrix

## Scope

This matrix is the institutional source-routing layer for the SBAS knowledge base. It classifies which source families can support which kinds of claims and identifies documents that earlier drafts used incorrectly.

This page is not an operational standards table. It does not provide procedure minima, aircraft eligibility, crew authorization, service availability, receiver certification status, or alert-limit values. Those require the applicable official standards, regulator material, service-provider documents, AIP/procedure publications, aircraft/avionics documentation, and operator approvals.

## Executive summary

The current source-hardening cycle produced three high-value outcomes:

1. [[Source - RTCA DO-229]] is the strongest current public-product-and-regulatory-signal-reviewed anchor for GPS/SBAS airborne equipment, but it remains a routing note rather than an official-text extraction.
2. [[Source - ICAO Doc 9849]] is the better ICAO GNSS implementation-guidance anchor than the previously cited Doc 9854/9855 pair.
3. [[Source - RTCA DO-242]], [[Source - RTCA DO-289]], [[Source - ICAO Doc 9854]], and [[Source - ICAO Doc 9855]] are now red-flagged as mis-scoped for SBAS technical/integrity claims based on public catalog signals.

The practical consequence is conservative: the KB should continue to explain SBAS concepts clearly, but it should not publish exact numerical operational requirements until each number is tied to the right official source family.

## Source identity and claim-routing matrix

| Source note                                   | Public identity signal reviewed in this cycle                                                                                             | Safe current role in this KB                                                                                                            | Do not use it for                                                                                                                                          |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [[Source - RTCA DO-229]]                      | RTCA GPS/SBAS airborne-equipment MOPS; public RTCA product signal identifies DO-229F as single-frequency GPS/SBAS airborne-equipment MOPS | Airborne receiver/equipment source-family anchor; LPV/LP/LNAV/VNAV equipment-capability routing; receiver-performance extraction target | SBAS ground-system certification, state approval, service availability, procedure minima, aircraft installation/operational approval, or DFMC requirements |
| [[Source - ICAO Doc 9849]]                    | ICAO Global Navigation Satellite System (GNSS) Manual                                                                                     | GNSS/SBAS implementation-guidance anchor for States and GNSS-based services                                                             | Detailed normative SARPs, aircraft equipment MOPS, exact LPV alert limits, direct operational approval                                                     |
| [[Source - ICAO Annex 10 Volume I GNSS SBAS]] | ICAO Annex 10, Volume I, Radio Navigational Aids; public ICAO Store signal identifies GNSS among covered radio-navigation-aid systems     | ICAO SARPs/technical-provisions source-family anchor for GNSS/SBAS claim routing                                                        | Detailed Annex content, numerical SBAS values, procedure minima, aircraft eligibility, or operational approval claims until official text is extracted     |
| PANS-OPS / procedure-design sources           | Not yet represented by a dedicated source note in this KB                                                                                 | Candidate future source family for procedure design and minima concepts                                                                 | Not replaceable by DO-229 or Doc 9849 alone                                                                                                                |
| Service-provider definition documents         | Not yet represented consistently                                                                                                          | Candidate future source family for WAAS/EGNOS/MSAS/GAGAN/KASS/SouthPAN service commitments                                              | Not replaceable by generic SBAS concept pages                                                                                                              |
| Regulator / ANSP / AIP material               | Partly present in regional source backlogs                                                                                                | Candidate source family for operational authorization, published procedures, and state implementation                                   | Not inferable from technical standards alone                                                                                                               |
| [[Source - ICAO Doc 9854]]                    | ICAO Global Air Traffic Management Operational Concept                                                                                    | High-level ATM modernization context only, if directly extracted later                                                                  | SBAS performance testing, SBAS monitoring, LPV, alert limits, protection levels                                                                            |
| [[Source - ICAO Doc 9855]]                    | ICAO public-internet guidance for aeronautical applications                                                                               | Possible internet/aeronautical-applications context only, if directly extracted later                                                   | SBAS technical specifications, GNSS/SBAS architecture, integrity requirements                                                                              |
| [[Source - RTCA DO-242]]                      | RTCA ADS-B / surveillance standard signal                                                                                                 | ADS-B/surveillance provenance only, if needed later                                                                                     | SBAS augmentation-system or integrity claims                                                                                                               |
| [[Source - RTCA DO-289]]                      | RTCA aircraft-surveillance-applications standard signal                                                                                   | Aircraft-surveillance provenance only, if needed later                                                                                  | SBAS performance testing or monitoring                                                                                                                     |

## Claim-type matrix

| Claim type                         | Primary source family needed                                                                     | Current KB posture                                          | Safe publication pattern                                                                                                       |
| ---------------------------------- | ------------------------------------------------------------------------------------------------ | ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| What SBAS is                       | ICAO GNSS implementation guidance; Annex 10 source note; service-provider descriptions           | Conceptually strong, source-scaffold-linked                 | Explain at high level; link to source notes and keep caveats                                                                   |
| SBAS architecture                  | ICAO GNSS guidance; Annex 10; service-provider architecture documentation                        | Conceptually strong, direct-source extraction still pending | Describe chain: GNSS satellites, reference network, processing, uplink, GEO/space broadcast, receiver processing               |
| Airborne SBAS equipment            | RTCA/EUROCAE airborne equipment MOPS; regulator TSOs/ETSO material                               | DO-229 anchor improved with RTCA/FAA/EASA public signals    | Link to DO-229 for source-family routing; avoid class-specific, numerical, installation, or operational claims until extracted |
| LPV operational use                | Equipment MOPS + procedure design + service availability + aircraft/operator/regulator approvals | LPV page is educational and source-disciplined              | State dependency layers; do not publish minima/eligibility as facts                                                            |
| Protection levels and alert limits | Equipment standards + ICAO/RTCA/EUROCAE definitions + procedure/operation-specific material      | Concept pages upgraded but still source-scaffold-linked     | Explain relationship without numerical thresholds                                                                              |
| Performance monitoring             | ICAO GNSS manual / Annex 10 / service-provider performance reports                               | Source family not yet fully built                           | Discuss as a needed source branch, not as a verified table                                                                     |
| Country or regional readiness      | Regulator/ANSP/AIP/service-provider sources; institutional plans                                 | ASEAN branch is cautious synthesis                          | Use readiness categories only with explicit evidence limits                                                                    |
| System comparisons                 | Service definitions and performance reports from each system                                     | Draft/synthesis in many pages                               | Compare source posture first; avoid false precision                                                                            |

## Red-flag correction register

| Earlier draft mapping                                    | Current correction                                                                                | Impact                                                                                 |
| -------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Doc 9855 as SBAS technical specifications                | Public ICAO catalog identifies Doc 9855 as public-internet guidance for aeronautical applications | Remove as SBAS technical source; replace with Doc 9849 / Annex 10 source-building path |
| Doc 9854 as GBAS/SBAS performance testing and monitoring | Public ICAO catalog identifies Doc 9854 as Global ATM Operational Concept                         | Remove as SBAS performance-testing source; keep only as possible ATM concept source    |
| DO-242 as GNSS augmentation-system/integrity source      | Public catalog identifies DO-242 as ADS-B related                                                 | Stop using for SBAS integrity and augmentation claims                                  |
| DO-289 as SBAS performance-testing source                | Public catalog identifies DO-289 as aircraft surveillance applications                            | Stop using for SBAS testing/monitoring claims                                          |

## Recommended source-building sequence

1. Directly extract [[Source - ICAO Annex 10 Volume I GNSS SBAS]] from the official Annex text, including exact edition/amendment baseline and GNSS/SBAS section mapping.
2. Directly extract the official [[Source - RTCA DO-229]] text for equipment classes, LPV/LP/LNAV/VNAV capability, receiver integrity, alerting, and test-method language; map it separately from FAA/EASA installation and operational-approval sources.
3. Directly extract [[Source - ICAO Doc 9849]] sections relevant to GNSS implementation, SBAS introduction, monitoring/assessment/reporting, DFMC GNSS, and interference mitigation.
4. Create procedure-design source notes for the PANS-OPS / PBN side of LPV, LNAV/VNAV, RNAV, and RNP notes.
5. Create service-provider source notes for WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, SouthPAN, and other systems before publishing comparative performance tables.
6. Only after the above, reintroduce numerical thresholds or performance values into concept and aviation pages.

## Documentation rules for downstream pages

When editing downstream pages:

- Use [[Source - RTCA DO-229]] only for airborne GPS/SBAS equipment source-family routing.
- Use [[Source - ICAO Doc 9849]] only for implementation-guidance routing until direct extraction is complete.
- Keep [[Source - RTCA DO-242]], [[Source - RTCA DO-289]], [[Source - ICAO Doc 9854]], and [[Source - ICAO Doc 9855]] visible as red-flag notes so earlier draft confusion remains traceable rather than silently erased.
- Do not create broken wikilinks for future standards notes. Mention future targets in plain text unless creating the note now.
- If a number matters operationally, do not publish it without a direct source anchor and clear applicability conditions.

## See also

- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9849]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[SBAS Integrity]]
- [[LPV-Approach-Procedure]]
- [[SBAS MOC]]
- [[SBAS Knowledge Base Editorial and Source Policy]]
