---
title: ResearchLog 2026-05-02 Institutional Navigation Upgrade
description: Research log for the institutional-grade SBAS homepage, navigation, pillar-page, and link-health upgrade cycle
tags: [log, sbas, quartz, institutional-grade, navigation, documentation-quality]
created: 2026-05-02
modified: 2026-05-02
status: active
verification_status: implementation-log
---

# ResearchLog 2026-05-02 Institutional Navigation Upgrade

## Scope

This cycle upgraded the public first-reader experience of the SBAS Quartz knowledge base. The work focused on navigation reliability, institutional documentation quality, beginner onboarding, and source-discipline language.

The cycle did not attempt to verify every technical or operational claim in the knowledge base. Instead, it strengthened the site architecture so future source-hardening work can proceed from a cleaner public-facing structure.

## Safety and baseline

- A private pre-change backup was created before editing the published Quartz content root.
- The repository baseline was clean before edits.
- The active content root remained the canonical Quartz content directory.

## Files created

- `Concepts/What is SBAS.md`
- `Concepts/SBAS Architecture.md`
- `Concepts/SBAS Architecture Flow.md`
- `Logs/ResearchLog-2026-05-02-Institutional-Navigation-Upgrade.md`

## Files substantially upgraded

- `index.md`
- `MOCs/SBAS MOC.md`
- `MOCs/SBAS-in-Civil-Aviation-MOC.md`
- `MOCs/SBAS-Systems-by-Region-MOC.md`
- `Concepts/SBAS-Terminology.md`

## Files patched for link hygiene

Targeted wikilink cleanup was applied across older pages where links used path-style targets, `.md` suffixes, escaped pipes, or candidate pages that do not yet exist.

Examples of cleanup patterns:

- path-style links were converted to canonical Obsidian-style note links;
- candidate source notes that do not yet exist were left as plain-text future targets;
- nonexistent future system notes such as KASS, SDCM, and A-SBAS were kept as candidate research targets rather than broken links;
- older aviation notes now link to canonical MOC and standards note names.

## Documentation-quality decisions

### Beginner gateway

Created [[What is SBAS]] as the primary reader entry point. This separates institutional explanation from the controlled terminology note and gives new readers a clearer path into architecture, integrity, aviation operations, standards, and ASEAN implementation.

### Architecture pillar

Created [[SBAS Architecture]] as a system-level institutional pillar. The page emphasizes the full augmentation chain:

- GNSS observation;
- reference station monitoring;
- processing and integrity estimation;
- uplink and broadcast;
- receiver-side use;
- operational approval and institutional dependencies.

### Architecture flow

Created [[SBAS Architecture Flow]] with a compact Mermaid diagram. The diagram separates the correction path from the integrity path and warns that broadcast availability, receiver capability, and operational approval are not equivalent.

### Controlled terminology

Reworked [[SBAS-Terminology]] into a controlled terminology page rather than a beginner article. The page now routes beginners to [[What is SBAS]] and preserves source-discipline caveats for accuracy, integrity, availability, operational status, coverage, and readiness.

### Civil aviation map

Reworked [[SBAS in Civil Aviation MOC]] to remove overconfident operational framing and clarify that procedure minima, eligibility, equipage, and service availability must be checked against approved sources.

### Regional systems map

Reworked [[SBAS-Systems-by-Region-MOC]] to avoid unsupported performance-table authority and to frame future systems such as KASS, SDCM, SouthPAN, and ASECNA as source-backed future targets rather than completed pages.

## QA results

Post-edit QA results:

- Quartz build: passed.
- Publication/privacy audit: passed.
- Local/private path scan: passed.
- Bad frontmatter delimiter scan: passed.
- Markdown input files after cycle: 103.
- Broken wikilinks after cycle: 0.

## Source and verification boundary

New and upgraded pages are marked as `synthesis-with-caveats` or `source-scaffold-linked` where appropriate. They improve institutional readability and navigation, but they do not convert draft operational claims into verified standards claims.

Future source-hardening should still use:

- [[SBAS Source Backlog]]
- [[ASEAN SBAS Source Backlog]]
- [[Source - RTCA DO-229]]
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-289]]
- [[Source - ICAO Doc 9854]]
- [[Source - ICAO Doc 9855]]

## Recommended next cycle

The next high-value cycle should upgrade the integrity learning path:

1. strengthen [[SBAS Integrity]] with clearer standards/source anchors;
2. deepen [[Protection Levels]];
3. deepen [[Alert Limits]];
4. patch [[LPV-Approach-Procedure]] to remove or source numerical claims;
5. update [[SBAS in Civil Aviation MOC]] after those child pages are hardened.
