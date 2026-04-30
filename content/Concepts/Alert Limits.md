---
title: Alert Limits
description: Draft concept note on alert limits in SBAS and their role in operational acceptability decisions
tags: [concept, alert-limits, sbas, integrity, aviation, provisional]
created: 2026-04-23
modified: 2026-04-23
status: draft
verification_status: source-scaffold-linked
---

# Alert Limits

## Definition status
This note is a draft concept note.

Boundary:
- It synthesizes existing vault language rather than verified primary-source extraction.
- It is linked to provisional source scaffolds, not yet to completed source notes.
- Numeric values already present in procedure notes should be treated as provisional until tied to verified source material.

## Working definition
Within the current vault, alert limits are treated as operational boundaries used to determine whether a navigation solution remains acceptable for the intended phase of flight.

The vault's existing language implies that alert limits matter because exceeding them should trigger a warning or a loss-of-use decision.

## Relationship to integrity and protection levels
[[SBAS Integrity]] is the broader safety function.
[[Protection Levels]] are currently treated in the vault as the bound being compared against operational criteria.
[[Alert Limits]] are the operational criteria that frame whether continued use is acceptable.

This relationship still requires direct source confirmation.

## Current in-vault usage
Alert-limit language already appears in these places:
- [[Safety-Terminology]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]

## Aviation implications
The current vault uses alert limits mainly in approach and operational-safety contexts.

Examples implied by existing notes:
- alert limits help determine whether an approach can continue
- alerting logic is tied to missed-approach or non-use decisions
- alert limits are closely related to procedure type and integrity monitoring

These are synthesis statements and should not yet be treated as verified requirements.

## Current source anchors
These are source scaffolds, not completed source notes.
- [[Source - RTCA DO-242]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9855]]
- [[Source - ICAO Doc 9854]]
- [[Source - RTCA DO-289]]

## Distinguish from related concepts
- [[SBAS Integrity]] is the broader safety function.
- [[Protection Levels]] are the inferred bounds being assessed against use criteria.
- [[Safety-Terminology]] is the current general terminology stub.

## Open provenance questions
- Which alert-limit statements in procedure notes are placeholders versus source-grounded requirements?
- Which source scaffold should become the primary anchor for a fully verified alert-limits note?
- How should alert-limit language be distinguished from generic warning thresholds in non-SBAS procedure notes?

## See also
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[SBAS Source Backlog]]
