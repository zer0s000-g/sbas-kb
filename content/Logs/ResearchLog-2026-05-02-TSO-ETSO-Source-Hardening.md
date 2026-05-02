---
title: Research Log - 2026-05-02 TSO ETSO Source Hardening
description: Work log documenting FAA TSO-C145e/C146e and EASA ETSO-C145e/C146e source-note creation and standards-branch routing updates
tags: [research-log, standards, sources, faa, easa, tso, etso, sbas]
created: 2026-05-02
modified: 2026-05-02
status: active
verification_status: work-log
---

# Research Log - 2026-05-02 TSO ETSO Source Hardening

## Objective

Create the regulator/article-approval source layer that the DO-229 cycle identified as the next institutional gap: FAA TSO-C145e/C146e and EASA ETSO-C145e/C146e.

## Source posture before this cycle

- [[Source - RTCA DO-229]] correctly identified FAA/EASA TSO/ETSO material as approval-context evidence.
- The KB did not yet have dedicated source notes for FAA TSO-C145e/C146e or EASA ETSO-C145e/C146e.
- Several downstream pages still had to describe approval boundaries generically rather than linking to explicit regulator-source anchors.

## Public sources reviewed

| Source family                   | Public evidence used                                                                                              | Editorial use                                                                                                           |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| FAA TSO overview                | FAA public TSO page defining TSO as a minimum performance standard and separating TSOA from installation approval | Strong approval-boundary rule                                                                                           |
| FAA DRS TSO-C145e/C146e records | Public DRS/search signals locating the TSO records and DO-229E relationship snippets                              | Source identity and future extraction routing; not full TSO extraction                                                  |
| FAA AC 20-138B                  | Public airworthiness guidance for installed positioning/navigation equipment                                      | Context for installation/airworthiness separation, used cautiously                                                      |
| EASA ETSO-C145e PDF             | Public EASA PDF text-extracted in this cycle                                                                      | Dedicated source note with extracted scope, DO-229E, Class Beta, and integration-boundary signals                       |
| EASA ETSO-C146e A1 PDF          | Public EASA PDF text-extracted in this cycle                                                                      | Dedicated source note with extracted scope, DO-229E, Class Gamma/Delta, CCA option, and aircraft-level-boundary signals |
| EASA ETSO list / NPA context    | Public EASA list and rulemaking context                                                                           | Secondary context only; not used to create operational claims                                                           |

## Files created

- [[Source - FAA TSO-C145e and TSO-C146e]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]

## Files patched

- [[Source - RTCA DO-229]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[SBAS-Standards-Regulation]]
- [[SBAS-vs-Other-Standards]]
- [[SBAS-Research-MOC]]
- [[SBAS in Civil Aviation MOC]]

## Documentation-quality decisions

1. FAA and EASA material were treated as regulator/article-approval source layers, not as operational approval layers.
2. The FAA note is deliberately conservative because the specific TSO PDFs were located through public DRS signals but not fully extractable in this cycle.
3. The EASA note is stronger because the public PDFs were retrieved and text-extracted, but it still avoids replacing official source review, aircraft-level certification, installation manuals, and operational approvals.
4. No LPV minima, alert limits, protection-level equations, receiver algorithms, or aircraft eligibility claims were introduced.
5. The standards matrix now separates MOPS, FAA TSO, EASA ETSO, installation approval, operational approval, and procedure/service availability.

## Recommended next cycle

Proceed to procedure-design/PBN source notes for LPV, LP, LNAV/VNAV, RNAV, and RNP claim boundaries. The equipment and approval-source backbone is now stronger, but operational procedure claims still require the procedure-design/AIP/operator/regulator layer before numerical or eligibility statements can be expanded.
