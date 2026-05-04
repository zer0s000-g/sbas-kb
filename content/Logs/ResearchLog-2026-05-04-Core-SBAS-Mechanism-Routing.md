---
title: Research Log - 2026-05-04 - Core SBAS Mechanism Routing
description: Work log for the third ten-cycle core SBAS solidification pass focused on ranging, correction mechanisms, integrity bounds, and service-status routing
tags: [research-log, sbas, core, source-routing, corrections, integrity, quartz]
created: 2026-05-04
modified: 2026-05-04
status: complete
verification_status: qa-passed
---

# Research Log - 2026-05-04 - Core SBAS Mechanism Routing

## Scope

This ten-cycle pass solidified the next layer of core SBAS knowledge after the earlier claim-routing and service-performance passes. The user requested institutional-grade quality, no overlapping knowledge, authenticated/source-routed truth, priority on core SBAS knowledge, and no long reference-website expansion.

## Source discipline

No new long reference-website expansion was performed. The pass used existing KB source anchors and created routing/concept notes only. New pages explicitly avoid publishing detailed standards text, equations, message tables, numerical values, current NOTAM/outage details, procedure minima, aircraft/operator eligibility, or operational approvals.

## Files created

- [[SBAS Ranging Sources and Time Reference]]
- [[SBAS Satellite Orbit and Clock Corrections]]
- [[SBAS Ionospheric Grid Correction Concept]]
- [[SBAS Correction Timescale Taxonomy]]
- [[SBAS Integrity Data and User Bounds]]
- [[SBAS Service Status and Operational Notices]]

## Files patched

- [[SBAS Core Claim Routing]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[SBAS MOC]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Signal and Message Flow]]

## Non-overlap decisions

| New note                                        | Owns                                                                                            | Does not own                                                             |
| ----------------------------------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| [[SBAS Ranging Sources and Time Reference]]     | ranging/time-reference claim routing                                                            | message tables, receiver approval, operational use                       |
| [[SBAS Satellite Orbit and Clock Corrections]]  | satellite-related correction context                                                            | equations, validity, update rates, service commitments                   |
| [[SBAS Ionospheric Grid Correction Concept]]    | ionospheric correction-routing boundary                                                         | GIVE values, grid definitions, operational model certification           |
| [[SBAS Correction Timescale Taxonomy]]          | fast/long-term/ionospheric category separation                                                  | message numbers, update intervals, timeout rules                         |
| [[SBAS Integrity Data and User Bounds]]         | bridge between corrections, protection levels, alert limits, and receiver/useability boundaries | equations, numerical bounds, alert timing, approval                      |
| [[SBAS Service Status and Operational Notices]] | status/notice routing rules                                                                     | current outages, NOTAMs, AIRAC-cycle data, provider bulletin duplication |

## Validation posture

The pass strengthens conceptual truth by narrowing each claim to its correct source family and owner note. It does not claim to have extracted new official Annex 10 or DO-229 requirements. Direct source extraction remains future work before any detailed numerical/mechanistic requirement is published.

## QA status

Cycle 10 will run full QA, commit, push, and verify live Quartz pages.
