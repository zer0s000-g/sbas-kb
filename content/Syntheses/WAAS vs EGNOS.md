---
title: WAAS vs EGNOS
description: Source-routed comparison note between the U.S. WAAS and European EGNOS SBAS implementations, focused on source posture rather than unsupported performance ranking
tags: [comparison, waas, egnos, sbas, regional-systems]
created: 2026-04-23
modified: 2026-05-03
status: reviewed
verification_status: source-routed-comparison-no-performance-ranking
---

# WAAS vs EGNOS

## Scope status

This is a source-routed comparison note between [[WAAS]] and [[EGNOS]]. It compares what the knowledge base can safely say from current official/public source notes; it does not compare operational performance.

Boundary:

- It does not rank WAAS and EGNOS by accuracy, continuity, availability, coverage, maturity, or interoperability.
- It does not verify airport/runway procedure availability or approach minima.
- It does not treat FAA and EGNOS/EUSPA service documents as equivalent in detail, legal status, or service-boundary structure without direct matched extraction.

## Why compare them

WAAS and EGNOS are useful comparison anchors because they represent mature U.S. and European SBAS service-provider contexts. They are also useful for showing how the KB must separate service-provider material from equipment standards, article approval, procedure design, and operational approval.

## Current authenticated comparison posture

| Dimension                            | WAAS source-routed posture                                                                                                                                    | EGNOS source-routed posture                                                                                                                                           | Safe comparison rule                                                                            |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| Dedicated source note                | [[Source - WAAS]]                                                                                                                                             | [[Source - EGNOS]]                                                                                                                                                    | Compare source posture before comparing system performance                                      |
| Current official source basis        | FAA WAAS public page and FAA August 2025 quick-facts PDF                                                                                                      | EGNOS Safety of Life Service Definition Document page and Issue 3.6 PDF                                                                                               | Both have official public provider material, but not identical document types                   |
| Broad aviation-service claim         | FAA material describes WAAS as serving all classes of aircraft in all phases of flight and supporting vertically guided approaches at qualified NAS locations | EGNOS material describes the SoL service as tailored to safety-critical aviation applications and compliant with APV-I/CAT-I requirements as defined by ICAO Annex 10 | Both can be described as aviation SBAS service-provider contexts within their source boundaries |
| Procedure-count / operational detail | FAA quick facts include LPV/LP public count snapshots for August 2025                                                                                         | Current extracted EGNOS note does not provide an equivalent procedure-count snapshot                                                                                  | Do not compare procedure inventory until matched official procedure/AIP evidence exists         |
| Authorization boundary               | Aircraft/operator/runway-specific claims require FAA procedure, operational, and status sources                                                               | Official EGNOS material states operational use may require relevant-authority authorization                                                                           | Keep authorization separate from service-definition statements                                  |

## What can be said safely now

- WAAS is routed through official FAA public WAAS material in [[Source - WAAS]].
- EGNOS is routed through official EGNOS Safety of Life service-definition material in [[Source - EGNOS]].
- Both belong to the service-provider source family routed by [[Source - SBAS Service Providers]].
- Neither source note alone authorizes aircraft/operator use, runway-specific procedures, or comparative performance conclusions.

## What remains uncertain

- Whether any interoperability statements between WAAS and EGNOS are supported by official bilateral/multilateral provider material.
- Whether procedure inventories can be compared using equivalent source types and snapshot dates.
- Whether service-area or performance comparisons can be made without mixing different definitions and legal/service commitments.

## Source anchors

- [[Source - WAAS]] -- official FAA public WAAS material.
- [[Source - EGNOS]] -- official EGNOS Safety of Life service-definition material.
- [[Source - SBAS Service Providers]] -- service-provider family router.
- [[SBAS Standards Source Matrix]] -- claim-routing matrix for source-family boundaries.

## Best next source-support targets

- FAA WAAS service/performance standard or performance reports.
- Official EGNOS/ESSP performance reports and current service-status material.
- FAA and European AIP/procedure sources if procedure inventories are compared.
- Official interoperability or transition-zone material before publishing cross-system interoperability conclusions.

## See also

- [[WAAS]]
- [[EGNOS]]
- [[Source - WAAS]]
- [[Source - EGNOS]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS in Civil Aviation MOC]]
- [[SBAS-vs-Other-Augmentation-Methods]]
- [[SBAS Source Backlog]]
