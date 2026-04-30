---
title: Protection Levels
description: Draft concept note on protection levels in SBAS and their role in aviation use decisions
tags: [concept, protection-levels, sbas, integrity, aviation, provisional]
created: 2026-04-23
modified: 2026-04-23
status: draft
verification_status: source-scaffold-linked
---

# Protection Levels

## Definition status
This note is a draft concept note.

Boundary:
- It synthesizes terminology already present in the vault.
- It is linked to provisional source scaffolds rather than completed source extraction.
- Numeric thresholds and operation-specific criteria elsewhere in the vault should be treated as provisional until anchored to verified source notes.

## Working definition
Within the current vault, protection levels are treated as bounds used in safety-relevant navigation decisions.

The existing vault language suggests that protection levels matter because they help determine whether the navigation solution remains acceptable for a specific operation, especially in approach contexts.

## Relationship to SBAS integrity
[[SBAS Integrity]] is the broader safety function; protection levels appear in the vault as one of the practical expressions of that function.

Current vault relationship pattern:
- integrity establishes the need for trustworthy use/no-use logic
- protection levels express the bound being compared against operational criteria
- alerting occurs when the operational criteria are not satisfied

This relationship still requires direct source confirmation.

## Current in-vault usage
Protection levels already appear in these places:
- [[Safety-Terminology]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[SBAS-Research-MOC]]

## Aviation implications
The current vault uses protection levels mainly in approach and operational-approval contexts.

Examples implied by existing notes:
- approach suitability depends on whether protection-level requirements are met
- different procedure types may imply different protection-level expectations
- protection-level language is closely tied to alert limits and integrity monitoring

These are synthesis statements and should not yet be treated as verified requirements.

## Current source anchors
These are source scaffolds, not completed source notes.
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9855]]
- [[Source - ICAO Doc 9854]]
- [[Source - RTCA DO-289]]

## Distinguish from related concepts
- [[SBAS Integrity]] is the broader safety concept.
- [[Alert Limits]] are the operational bounds against which use decisions may be framed.
- [[Safety-Terminology]] is currently the more general terminology stub.
- [[WAAS]] is a regional system context in which these concepts appear in current vault notes.

## Open provenance questions
- Which notes currently use "protection level" too loosely or without source support?
- Which protection-level claims in [[LPV-Approach-Procedure]] and [[LNAV-VNAV-Approach-Procedure]] are descriptive placeholders versus sourced requirements?
- Which source scaffold should become the primary anchor for a fully verified protection-level note?

## See also
- [[SBAS Integrity]]
- [[Alert Limits]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[SBAS Source Backlog]]
