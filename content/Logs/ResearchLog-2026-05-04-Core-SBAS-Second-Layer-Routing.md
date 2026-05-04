---
title: Research Log - 2026-05-04 - Core SBAS Second-Layer Routing
description: Work log for the second ten-cycle core SBAS solidification pass focused on service performance, coverage, approach capability, standards-to-operations evidence, receiver modes, and ionospheric threat boundaries
tags: [research-log, sbas, core, source-routing, provenance, no-overlap]
created: 2026-05-04
modified: 2026-05-04
status: complete
verification_status: implementation-log
---

# Research Log - 2026-05-04 - Core SBAS Second-Layer Routing

## Scope

This cycle continued the core SBAS solidification work after [[SBAS Core Claim Routing]] was introduced.

The user priority was:

- institutional-grade core SBAS knowledge;
- no overlapping knowledge;
- no unsupported operational or numerical claims;
- skip long reference-website expansion;
- keep claims authenticated to the correct source family.

## Editorial decision

This pass did not perform a broad external-reference crawl. It used the existing source-routing backbone and created only core routing/concept pages needed to prevent overlap and source drift.

Existing FAA-related source notes remain in the vault where already present, but this pass did not deepen FAA-specific extraction.

## Files created

- [[SBAS Service Performance Concepts]]
- [[SBAS Service Volume and Coverage]]
- [[SBAS Approach Capability Taxonomy]]
- [[SBAS Standards to Operations Evidence Ladder]]
- [[SBAS Receiver Modes and Annunciation]]

## Files hardened

- [[SBAS Ionospheric Threat — Empirical Evidence]]
- [[LPV-Approach-Procedure]]
- [[SBAS MOC]]
- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]

## Non-overlap decisions

| Claim family                                                                 | Owner after this cycle                           | Boundary                                                                                    |
| ---------------------------------------------------------------------------- | ------------------------------------------------ | ------------------------------------------------------------------------------------------- |
| Accuracy, integrity, availability, continuity, coverage, service commitments | [[SBAS Service Performance Concepts]]            | Concept separation only; no numerical service claims                                        |
| Coverage and service-volume statements                                       | [[SBAS Service Volume and Coverage]]             | Coverage is not procedure publication, aircraft eligibility, or operational authorization   |
| LP/LPV/LNAV/VNAV labels                                                      | [[SBAS Approach Capability Taxonomy]]            | Capability labels are not proof of a published procedure or state approval                  |
| Standards-to-operations escalation                                           | [[SBAS Standards to Operations Evidence Ladder]] | Each evidence layer must be sourced before moving upward                                    |
| Receiver mode / annunciation                                                 | [[SBAS Receiver Modes and Annunciation]]         | No cockpit, timing, pilot-action, or receiver-algorithm detail without source extraction    |
| Ionospheric empirical evidence                                               | [[SBAS Ionospheric Threat — Empirical Evidence]] | Threat discovery only; not operational GIVE, service design, coverage, or approval evidence |

## Claims deliberately not added

This cycle did not add:

- SBAS message-number tables;
- bit fields or receiver algorithms;
- protection-level equations;
- alert-limit numerical values;
- service-availability percentages;
- coverage maps or service-volume coordinates;
- LPV minima, decision heights, runway examples, or procedure inventories;
- cockpit annunciation timing or pilot-action requirements;
- aircraft/operator eligibility claims.

## QA status

QA is part of Cycle 10. Required gates before commit/publish:

- Prettier
- `npm run check`
- Quartz build
- wikilink audit
- publication/privacy audit
- Markdown table audit
- suspicious separator audit
- `git diff --check`
- commit/push
- GitHub Actions and live Quartz verification

## See also

- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[SBAS Operational Validation Dashboard]]
