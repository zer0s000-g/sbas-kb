---
title: Institutional Upgrade Audit 2026-05-01
description: Maturity and quality audit for upgrading the SBAS Quartz knowledge base into an institutional-grade reference
labels: [sbas, audit, institutional-grade, quartz, governance]
tags: [sbas, audit, institutional-grade, quartz, governance]
created: 2026-05-01
modified: 2026-05-01
status: active
verification_status: editorial-control
---

# Institutional Upgrade Audit 2026-05-01

## Audit scope
This audit covers the published Quartz Markdown content and classifies notes by readiness for institutional-grade public use.

The audit checks maturity metadata, source anchoring, note depth, outbound connectivity, broken wikilinks, caveat language, and private/local path exposure.

## Executive finding
The knowledge base is already structurally useful, especially for ASEAN implementation and ionospheric research, but it is not yet fully institutional-grade because many pages remain draft-level, several core pages need source anchors, and broken wikilinks reduce navigation reliability.

## Summary metrics
|Metric|Value|
|---|---:|
|Markdown notes audited|97|
|Institutional candidates|36|
|Reviewed candidates|36|
|Upgrade needed|20|
|Scaffolds|5|
|Notes marked draft|62|
|Notes missing explicit status|14|
|Files with broken wikilinks|22|
|Total broken wikilinks|73|
|Private/local path issues|0|

## Directory maturity profile
|Area|Institutional candidates|Reviewed candidates|Upgrade needed|Scaffolds|
|---|---:|---:|---:|---:|
|ASEAN|14|1|2|0|
|Aviation|0|0|5|0|
|Concepts|3|10|2|2|
|Logs|0|2|1|2|
|MOCs|1|3|1|0|
|Sources|15|7|9|0|
|Standards-Regulation|0|2|0|0|
|Syntheses|3|6|0|0|
|Systems|0|5|0|0|
|index.md|0|0|0|1|

## Highest-priority repairs
These pages should be repaired before broad content expansion because they affect navigation, first impressions, or core concept quality.

|Note|Score|Grade|Status|Verification|Broken|Priority action|
|---|---|---|---|---|---|---|
|[[WorkLog-2026-04-19]]|5.3|scaffold|missing|missing|1|frontmatter, maturity status, verification label, source anchors, wikilink repair|
|[[Communication-Terminology]]|26.4|scaffold|missing|missing|0|maturity status, verification label, source anchors, depth, connectivity, boundary/caveats|
|[[ResearchLog-2026-04-19]]|39.1|scaffold|missing|missing|0|frontmatter, maturity status, verification label, source anchors|
|[[Safety-Terminology]]|42.1|scaffold|missing|missing|0|maturity status, verification label, source anchors, depth|
|[[index]]|44.2|scaffold|missing|missing|12|maturity status, verification label, depth, wikilink repair, boundary/caveats|
|[[SBAS-Terminology]]|46.6|upgrade-needed|missing|missing|3|maturity status, verification label, depth, wikilink repair, boundary/caveats|
|[[ResearchLog-2026-04-23]]|50|upgrade-needed|missing|missing|7|frontmatter, maturity status, verification label, wikilink repair|
|[[GBAS-Approach-Procedure]]|52.0|upgrade-needed|missing|missing|0|maturity status, verification label, source anchors, connectivity|
|[[SBAS MOC]]|56.7|upgrade-needed|active|missing|9|verification label, wikilink repair|
|[[LPV-Approach-Procedure]]|63.0|upgrade-needed|missing|missing|0|maturity status, verification label, source anchors|
|[[RNAV-Approach-Procedure]]|63.2|upgrade-needed|missing|missing|0|maturity status, verification label, source anchors|
|[[Brunei Darussalam]]|63.6|upgrade-needed|draft|mixed-external-scouting-and-synthesis|0|maturity status, source anchors, depth|
|[[LNAV-VNAV-Approach-Procedure]]|63.6|upgrade-needed|missing|missing|0|maturity status, verification label, source anchors|
|[[Myanmar]]|63.7|upgrade-needed|draft|mixed-external-scouting-and-synthesis|0|maturity status, source anchors, depth|
|[[Source - GIPTA GNSS RFI Discussion]]|64.3|upgrade-needed|draft|extracted-local-document|0|maturity status, source anchors|
|[[Source - GNSS Analyzer and SBAS Simulator GIPTA]]|64.3|upgrade-needed|draft|extracted-local-document|0|maturity status, source anchors|
|[[RNP-Approach-Procedure]]|64.5|upgrade-needed|missing|missing|0|maturity status, verification label, source anchors|
|[[Source - GIPTA SBAS Operation]]|64.5|upgrade-needed|draft|extracted-local-document|0|maturity status, source anchors|
|[[Source - GIPTA WRC-27 Aeronautical Agenda]]|64.5|upgrade-needed|draft|extracted-local-document|0|maturity status, source anchors|
|[[Source - GIPTA Non-Aviation SBAS]]|64.6|upgrade-needed|draft|extracted-local-document|0|maturity status, source anchors|

## Pillar-page candidates
These notes are strong candidates for upgrade into institutional reference pages or living-standard pages.

|Note|Score|Grade|Status|Verification|Words|Links|Priority action|
|---|---|---|---|---|---|---|---|
|[[ASEAN SBAS Adoption Landscape]]|90|institutional-candidate|draft|mixed-external-scouting-and-synthesis|1009|43|maturity status|
|[[ASEAN SBAS Deployment Barriers]]|90.0|institutional-candidate|draft|mixed-external-scouting-and-synthesis|798|23|maturity status|
|[[ASEAN SBAS Governance and Institutional Actors]]|90|institutional-candidate|draft|mixed-external-scouting-and-synthesis|940|22|maturity status|
|[[ASEAN SBAS Service-Model Options]]|90|institutional-candidate|draft|mixed-external-scouting-and-synthesis|903|19|maturity status|
|[[SBAS Ionospheric Threat — Empirical Evidence]]|86.9|institutional-candidate|draft|empirical-study|676|18|maturity status|
|[[Indonesian SBAS ION Paper Iterations]]|86.8|institutional-candidate|draft|empirical-study|471|10|maturity status, depth|
|[[Philippines]]|85.7|institutional-candidate|draft|mixed-external-scouting-and-synthesis|629|24|maturity status|
|[[Indonesia]]|84.7|institutional-candidate|draft|mixed-external-scouting-and-synthesis|587|27|maturity status|
|[[IRI-2020 vs GNSS-RO Indonesia]]|84.2|institutional-candidate|draft|empirical-study|569|15|maturity status|
|[[GNSS Radio Occultation]]|83.6|institutional-candidate|draft|empirical-study|545|16|maturity status|
|[[Total Electron Content (TEC)]]|83.1|institutional-candidate|draft|empirical-study|525|19|maturity status|
|[[Ionospheric Model Validation]]|82.5|institutional-candidate|draft|empirical-study|499|16|maturity status, depth|
|[[Thailand]]|81.9|institutional-candidate|draft|mixed-external-scouting-and-synthesis|476|22|maturity status, depth|
|[[Lao PDR]]|80.5|institutional-candidate|draft|mixed-external-scouting-and-synthesis|419|18|maturity status, depth|
|[[Cambodia]]|80.2|institutional-candidate|draft|mixed-external-scouting-and-synthesis|410|18|maturity status, depth|
|[[Malaysia]]|80.2|institutional-candidate|draft|mixed-external-scouting-and-synthesis|408|20|maturity status, depth|
|[[Singapore]]|80.1|institutional-candidate|draft|mixed-external-scouting-and-synthesis|403|20|maturity status, depth|
|[[ASEAN SBAS Operational Demand Drivers]]|80|institutional-candidate|draft|mixed-external-scouting-and-synthesis|807|18|maturity status, wikilink repair|
|[[ASEAN SBAS Readiness Heuristic]]|80|institutional-candidate|draft|mixed-external-scouting-and-synthesis|1208|41|maturity status, wikilink repair|
|[[Viet Nam]]|80.0|institutional-candidate|draft|mixed-external-scouting-and-synthesis|400|20|maturity status, depth|
|[[MSAS vs GAGAN]]|78.8|reviewed-candidate|draft|in-vault-synthesis-only|350|22|maturity status, depth|
|[[SBAS-Standards-Regulation]]|72.1|reviewed-candidate|draft|missing|683|5|maturity status, verification label, boundary/caveats|
|[[EGNOS]]|71.2|reviewed-candidate|draft|in-vault-synthesis-only|449|35|maturity status, depth, wikilink repair|
|[[SBAS Integrity]]|70.6|reviewed-candidate|draft|source-scaffold-linked|424|24|maturity status, depth, wikilink repair|
|[[BDSBAS]]|70.3|reviewed-candidate|draft|in-vault-synthesis-only|412|30|maturity status, depth, wikilink repair|

## Institutional-readiness interpretation
- `institutional-candidate` means a note has useful structure, links, caveats, and enough depth to become public-reference material after source tightening and editorial polish.
- `reviewed-candidate` means the page is promising but needs stronger source anchors, diagrams, or maturity cleanup.
- `upgrade-needed` means the page is useful but too draft-like, under-sourced, under-linked, or technically thin for institutional users.
- `scaffold` means the page should be rewritten, merged, or converted into a more purposeful note.

## Critical gaps
1. Too many pages remain marked as `draft` even where the content is relatively mature.
2. Several older core pages lack explicit `verification_status` metadata.
3. The homepage and main MOCs need link repair and institutional-grade navigation language.
4. Aviation operation pages need direct standards anchors.
5. Core beginner pages need more depth, diagrams, and clearer learning paths.
6. Source notes need a consistent public-source metadata pattern.
7. The site needs comparison matrices and implementation playbooks for professional users.

## Recommended next cycle
The next implementation cycle should focus on navigation and first-reader experience:

1. repair homepage and MOC wikilinks
2. add institutional maturity metadata to core pages
3. create or upgrade the beginner pillar: `What is SBAS?`
4. create the SBAS architecture pillar
5. create one high-quality diagram or architecture flow
6. keep all new claims source-linked or explicitly marked as synthesis

## See also
- [[Institutional SBAS Knowledge Base Upgrade Roadmap]]
- [[SBAS Knowledge Base Editorial and Source Policy]]
- [[SBAS MOC]]
- [[SBAS Source Backlog]]
