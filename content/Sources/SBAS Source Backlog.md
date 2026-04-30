---
title: SBAS Source Backlog
description: Prioritized backlog of source notes needed to support existing SBAS claims in the vault
tags: [sources, backlog, provenance, sbas, research]
created: 2026-04-23
modified: 2026-04-23
status: active
verification_status: internal-backlog-only
---

# SBAS Source Backlog

## Purpose
This note tracks high-priority source notes that should be created before draft SBAS claims in the vault are treated as verified research conclusions.

Important boundary:
- This is not itself an authoritative source note.
- It is a provenance-management note built from existing references already mentioned inside the vault.
- External document metadata and scope still need verification against the actual source documents.

## Priority 1 — foundational standards already referenced in the vault

### 1. ICAO Doc 8083
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], [[SBAS-vs-Other-Augmentation-Methods]], and [[SBAS in Civil Aviation MOC]].
- Why this matters: several notes currently use it to support SBAS operational or standards claims.
- Verification need: confirm document title, actual SBAS relevance, and which claims it can legitimately support.
- Candidate future note: [[Source - ICAO Doc 8083]]

### 2. ICAO Doc 9854
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], and [[SBAS-Research-MOC]].
- Why this matters: used as if it supports performance testing and monitoring claims.
- Verification need: confirm exact title, scope, and whether it covers SBAS, GBAS, or both.
- Starter note created: [[Source - ICAO Doc 9854]]
- Current status: title, edition, and scope still require direct verification against the actual document

### 3. ICAO Doc 9855
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], and [[SBAS-Research-MOC]].
- Why this matters: draft notes rely on it for technical specification claims.
- Verification need: confirm exact scope and map which technical claims can be traced to it.
- Starter note created: [[Source - ICAO Doc 9855]]
- Current status: title, edition, and scope still require direct verification against the actual document

### 4. RTCA DO-229
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], [[SBAS in Civil Aviation MOC]], and [[MOCs/SBAS-Systems-by-Region-MOC.md]].
- Why this matters: used as a key airborne equipment reference.
- Verification need: confirm revision, title, and which operational/receiver claims in the vault are actually supported.
- Starter note created: [[Source - RTCA DO-229]]
- Current status: metadata and scope still require direct verification against the actual document

### 5. RTCA DO-242
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], and [[SBAS-Research-MOC]].
- Why this matters: used for augmentation and integrity-related claims.
- Verification need: confirm scope and relationship to SBAS vs broader GNSS augmentation.
- Starter note created: [[Source - RTCA DO-242]]
- Current status: title, revision, and scope still require direct verification against the actual document

### 6. RTCA DO-289
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], and [[SBAS-Research-MOC]].
- Why this matters: draft notes use it for testing/monitoring statements.
- Verification need: confirm title, scope, and whether current references are too broad.
- Starter note created: [[Source - RTCA DO-289]]
- Current status: title, revision, and scope still require direct verification against the actual document

## Priority 2 — regional and European framework references already mentioned indirectly

### 7. EUROCAE ED-52
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], and [[SBAS-Research-MOC]].
- Why this matters: draft notes use it to anchor European SBAS claims.
- Verification need: confirm exact role in EGNOS/SBAS framing.
- Candidate future note: [[Source - EUROCAE ED-52]]

### 8. EUROCAE ED-102
- Current vault usage: cited in [[SBAS-Standards-Regulation]], [[SBAS-vs-Other-Standards]], and [[SBAS-Research-MOC]].
- Why this matters: currently used for interface-specification claims.
- Verification need: confirm exact applicability to SBAS notes in this vault.
- Candidate future note: [[Source - EUROCAE ED-102]]

### 9. EUROCAE ED-142
- Current vault usage: cited in [[SBAS-Standards-Regulation]] and [[SBAS-Research-MOC]].
- Why this matters: draft notes use it in safety-assessment context.
- Verification need: confirm whether current safety-linkage claims are precise or overgeneralized.
- Candidate future note: [[Source - EUROCAE ED-142]]

## Claim clusters that need source support

### Standards mapping
- document titles
- document scope statements
- which documents are system-level vs airborne-equipment vs testing references

### Performance figures
- horizontal/vertical accuracy numbers
- continuity and availability percentages
- alerting or time-to-alarm values
- regional uptime figures

### Operational claims
- LPV/APV capability statements
- regional operational approval statements
- interoperability claims across WAAS/EGNOS/MSAS/GAGAN and other systems

## Suggested execution order
1. [[Source - RTCA DO-229]]
2. [[Source - ICAO Doc 9855]]
3. [[Source - ICAO Doc 9854]]
4. [[Source - RTCA DO-242]]
5. [[Source - RTCA DO-289]]
6. European framework notes after the above
7. [[Source - GNSS Radio Occultation Technique]]
8. [[Source - IRI-2020 Ionosphere Model]]
9. [[Source - GNSS-RO Indonesia Empirical Study]]

## Related notes
- [[SBAS MOC]]
- [[SBAS Research MOC]]
- [[SBAS-Standards-Regulation]]
- [[SBAS-vs-Other-Standards]]
- [[SBAS in Civil Aviation MOC]]
- [[ASEAN SBAS Source Backlog]]
- [[GNSS Radio Occultation]]
- [[IRI-2020 vs GNSS-RO Indonesia]]

## Open questions
- Which cited standards references in the current vault are mis-scoped, outdated, or incorrectly titled?
- Which existing performance figures can be supported by primary standards versus implementation reports?
- Should future source notes separate normative requirements from guidance and operational implementation material?
