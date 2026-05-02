---
title: ResearchLog 2026-05-02 Standards Source Matrix
description: Research log for the SBAS standards/source matrix and source-mapping correction cycle
tags: [log, sbas, standards, sources, provenance, institutional-grade]
created: 2026-05-02
modified: 2026-05-02
status: active
verification_status: implementation-log
---

# ResearchLog 2026-05-02 Standards Source Matrix

## Scope

This cycle implemented the recommended source-backed standards matrix for the SBAS integrity and aviation documentation path.

Primary focus:

- [[SBAS Standards Source Matrix]]
- [[SBAS-Standards-Regulation]]
- [[SBAS-vs-Other-Standards]]
- [[SBAS-vs-Other-Augmentation-Methods]]
- [[SBAS Source Backlog]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9849]]
- red-flag correction notes for [[Source - RTCA DO-242]], [[Source - RTCA DO-289]], [[Source - ICAO Doc 9854]], and [[Source - ICAO Doc 9855]]

## Safety and baseline

- A private pre-change backup was created before editing the published Quartz content root.
- The repository baseline was clean before edits.
- The active content root remained the canonical Quartz content directory.

## Public catalog signals reviewed

This cycle used public catalog signals, not full proprietary standards extraction. The distinction matters:

- public catalog metadata can verify broad document identity and source-family routing;
- it cannot support detailed numerical requirements, compliance interpretations, or operational authorization;
- official source extraction remains required before publishing precise SBAS requirements.

## Main findings

### RTCA DO-229

[[Source - RTCA DO-229]] remains the strongest current source-family anchor for GPS/SBAS airborne equipment. It was upgraded from a starter note to a public-catalog-reviewed source note, while retaining clear limits against detailed requirement extraction.

### ICAO Doc 9849

[[Source - ICAO Doc 9849]] was added as the current ICAO GNSS implementation-guidance anchor. Public ICAO Store metadata identifies it as the Global Navigation Satellite System (GNSS) Manual and describes its purpose as assisting States with GNSS implementation.

### Mis-scoped references corrected

The following earlier mappings were red-flagged:

- [[Source - RTCA DO-242]]: public catalog signal points to ADS-B / surveillance, not SBAS augmentation-system requirements.
- [[Source - RTCA DO-289]]: public catalog signal points to aircraft surveillance applications, not SBAS performance testing.
- [[Source - ICAO Doc 9854]]: public ICAO Store signal points to Global Air Traffic Management Operational Concept, not SBAS performance testing.
- [[Source - ICAO Doc 9855]]: public ICAO Store signal points to public-internet guidance for aeronautical applications, not SBAS technical specifications.

## Documentation-quality decisions

1. The red-flagged source notes were retained rather than deleted. This preserves provenance and prevents future editors from reintroducing the same mapping errors.
2. The standards overview was rewritten around source families and claim boundaries rather than broad unsupported document lists.
3. The augmentation-method comparison was rewritten to remove unsupported accuracy, coverage, latency, benefit, and LPV/GBAS confusion.
4. The source backlog was reprioritized around the real standards backbone: Annex 10, DO-229, Doc 9849, procedure-design sources, and service-provider documents.
5. No numerical LPV, alert-limit, protection-level, or system-performance values were reintroduced.

## Files created

- `Standards-Regulation/SBAS Standards Source Matrix.md`
- `Sources/Source - ICAO Doc 9849.md`
- `Logs/ResearchLog-2026-05-02-Standards-Source-Matrix.md`

## Files substantially upgraded or corrected

- `Sources/Source - RTCA DO-229.md`
- `Sources/Source - RTCA DO-242.md`
- `Sources/Source - RTCA DO-289.md`
- `Sources/Source - ICAO Doc 9854.md`
- `Sources/Source - ICAO Doc 9855.md`
- `Standards-Regulation/SBAS-Standards-Regulation.md`
- `Standards-Regulation/SBAS-vs-Other-Standards.md`
- `Concepts/SBAS-vs-Other-Augmentation-Methods.md`
- `Sources/SBAS Source Backlog.md`
- `MOCs/SBAS MOC.md`
- `MOCs/SBAS-Research-MOC.md`
- `MOCs/SBAS-in-Civil-Aviation-MOC.md`

## QA requirements

After this log is committed, the cycle should pass:

- Quartz build;
- publication/privacy audit;
- wikilink audit;
- git status review;
- deployment verification for the new source-matrix and source-note pages.

## Recommended next cycle

Create the Annex 10 GNSS/SBAS source note and use it to tighten [[SBAS Architecture]], [[SBAS Integrity]], [[Protection Levels]], and [[Alert Limits]] without introducing operational numerical values until the relevant official text has been extracted and classified.

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[SBAS-Research-MOC]]
- [[SBAS Knowledge Base Editorial and Source Policy]]
