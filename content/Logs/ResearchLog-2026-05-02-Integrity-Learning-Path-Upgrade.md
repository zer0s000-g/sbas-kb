---
title: ResearchLog 2026-05-02 Integrity Learning Path Upgrade
description: Research log for the institutional-grade SBAS integrity, protection-level, alert-limit, and LPV documentation upgrade cycle
tags: [log, sbas, integrity, lpv, aviation, institutional-grade, source-discipline]
created: 2026-05-02
modified: 2026-05-02
status: active
verification_status: implementation-log
---

# ResearchLog 2026-05-02 Integrity Learning Path Upgrade

## Scope

This cycle upgraded the SBAS integrity learning path into a more institutional-grade documentation layer.

Primary focus:

- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]

The cycle did not verify exact numerical thresholds against primary standards. Instead, it removed or quarantined unsupported operational numbers and replaced them with source-disciplined conceptual explanations suitable for public institutional reading.

## Safety and baseline

- A private pre-change backup was created before editing the published Quartz content root.
- The repository baseline was clean before edits.
- The active content root remained the canonical Quartz content directory.

## Files substantially upgraded

- `Concepts/SBAS Integrity.md`
- `Concepts/Protection Levels.md`
- `Concepts/Alert Limits.md`
- `Aviation/LPV-Approach-Procedure.md`

## Files patched

- `MOCs/SBAS-in-Civil-Aviation-MOC.md`

## Documentation-quality decisions

### Integrity page

[[SBAS Integrity]] was rewritten as the top-level safety-function concept page. It now clearly distinguishes accuracy from integrity and explains that SBAS must support use-or-non-use decisions, not merely improve estimated position.

### Protection-level page

[[Protection Levels]] was rewritten as the bounded-error concept page. It now explains that a protection level is not actual error and should not be confused with an accuracy estimate.

### Alert-limit page

[[Alert Limits]] was rewritten as the operation-specific threshold concept page. It now explains the relationship between protection levels and alert limits without publishing unsourced values.

### LPV page

[[LPV-Approach-Procedure]] was converted from an overconfident procedure-style draft into a source-disciplined institutional learning page. Unsupported numerical performance values, generic minima, training-hour claims, cost estimates, and benefit percentages were removed from the authoritative narrative.

### Civil aviation MOC

[[SBAS in Civil Aviation MOC]] was patched to reflect the upgraded editorial maturity of the integrity path and LPV page.

## Source and verification boundary

All upgraded pages remain `source-scaffold-linked`. They are now suitable as high-quality public learning pages, but they are not verified operational requirements tables.

Relevant source scaffolds remain:

- [[Source - RTCA DO-229]]
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-289]]
- [[Source - ICAO Doc 9854]]
- [[Source - ICAO Doc 9855]]
- [[SBAS Source Backlog]]

## Recommended next cycle

The next high-value cycle should create a source-backed standards matrix for the integrity path:

1. verify exact metadata and scope for [[Source - RTCA DO-229]];
2. verify exact metadata and scope for [[Source - RTCA DO-242]];
3. verify whether [[Source - ICAO Doc 9855]] or [[Source - ICAO Doc 9854]] is the correct anchor for each architecture, integrity, and testing claim;
4. add a comparison table showing which claims are airborne-equipment, system-level, procedure-design, regulator/ANSP, or service-provider claims;
5. only then reintroduce any numerical values into [[LPV-Approach-Procedure]].
