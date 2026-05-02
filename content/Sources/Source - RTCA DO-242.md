---
title: Source - RTCA DO-242
description: Red-flag source note documenting that public catalog signals identify RTCA DO-242 as ADS-B related, not as a current SBAS augmentation-system anchor
tags: [source, rtca, do-242, ads-b, surveillance, red-flag, provenance]
source_type: standard
created: 2026-04-23
modified: 2026-05-02
status: red-flag
verification_status: public-catalog-mismatch
---

# Source - RTCA DO-242

## Scope of this note

This note preserves a provenance correction. Earlier vault drafts treated RTCA DO-242 as if it were a GNSS augmentation-system or SBAS integrity source. Public catalog signals reviewed in this cycle instead identify RTCA DO-242 as an ADS-B / surveillance-related standard.

Important boundary:

- This note is not a completed extraction from the RTCA document itself.
- The public-catalog signal is strong enough to flag the previous SBAS use as likely mis-scoped.
- Do not use DO-242 as a source anchor for SBAS integrity, LPV, protection levels, alert limits, or augmentation-system requirements unless a later direct source review proves a specific relevant linkage.

## Public-catalog identity signal

| Field | Current public-catalog signal |
|---|---|
| Issuing body | RTCA, Inc. |
| Document | DO-242 / change to DO-242A in the consulted catalog signal |
| Public title signal | Minimum Aviation System Performance Standards for Automatic Dependent Surveillance Broadcast (ADS-B) |
| Publication-date signal | 2006-12-13 for the cataloged current change item |
| Scope signal | Clarifies ADS-B transmitted-position-quality parameters |
| SBAS relevance signal | Not identified as an SBAS augmentation-system standard in the reviewed public catalog material |

## Provenance correction

Previous in-vault wording described DO-242 as a GNSS augmentation systems reference. That wording should be treated as superseded by this correction until direct-source review shows otherwise.

Recommended replacement behavior:

- For airborne GPS/SBAS equipment claims, use [[Source - RTCA DO-229]].
- For GNSS implementation guidance, use [[Source - ICAO Doc 9849]] with Annex 10 / regulator sources still required for normative claims.
- For system-level SBAS SARPs or service-definition claims, create or verify Annex 10, service-provider, and regulator source notes.
- For ADS-B position-quality or surveillance applications, retain DO-242 only as a possible surveillance-system source family, not as an SBAS source.

## Downstream cleanup targets

The following pages should avoid presenting DO-242 as an SBAS integrity or augmentation-system authority:

- [[SBAS-Standards-Regulation]]
- [[SBAS Standards Source Matrix]]
- [[SBAS-vs-Other-Standards]]
- [[SBAS-vs-Other-Augmentation-Methods]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS Source Backlog]]

## What remains uncertain

- Whether older working groups, related RTCA documents, or secondary citations created the initial in-vault confusion.
- Whether a different RTCA document number, not DO-242, was intended as the SBAS augmentation-system anchor.
- Which exact RTCA/EUROCAE/ICAO source should anchor each remaining system-level SBAS claim.

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - RTCA DO-229]]
- [[Source - RTCA DO-289]]
- [[SBAS-Standards-Regulation]]
- [[SBAS MOC]]
