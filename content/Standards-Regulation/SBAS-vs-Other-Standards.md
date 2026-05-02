---
title: SBAS Standards Comparison
description: Source-disciplined comparison of standards source families for SBAS, GBAS, ABAS, RAIM, and related aviation-navigation concepts
tags: [standards, comparison, sbas, gbas, abas, raim, source-discipline]
category: standards
created: 2026-04-19
modified: 2026-05-02
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# SBAS Standards Comparison

## Scope

This page compares standards source families, not operational approvals. It does not certify that a document supports a specific numerical requirement or procedure. Use [[SBAS Standards Source Matrix]] for the current source-routing table.

## Provenance status

Several earlier draft mappings were corrected in the 2026-05-02 source-matrix cycle:

- [[Source - RTCA DO-242]] is now red-flagged as ADS-B/surveillance related rather than an SBAS augmentation-system source.
- [[Source - RTCA DO-289]] is now red-flagged as aircraft-surveillance related rather than an SBAS performance-testing source.
- [[Source - ICAO Doc 9854]] is now red-flagged as the Global ATM Operational Concept rather than an SBAS performance-testing document.
- [[Source - ICAO Doc 9855]] is now red-flagged as public-internet guidance for aeronautical applications rather than an SBAS technical-specification document.
- [[Source - ICAO Doc 9849]] has been added as the current ICAO GNSS implementation-guidance anchor.

## Source-family comparison

| Domain                    | Likely source family                                                     | Current KB source posture                                             | Main caution                                                                                                                          |
| ------------------------- | ------------------------------------------------------------------------ | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| SBAS airborne equipment   | RTCA/EUROCAE airborne-equipment MOPS                                     | [[Source - RTCA DO-229]] is public-product/regulatory-signal reviewed | Detailed requirements, classes, installation approval, and operational approval require official RTCA and regulator-source extraction |
| SBAS state implementation | ICAO GNSS guidance and Annex 10                                          | [[Source - ICAO Doc 9849]] added; Annex 10 note still needed          | Guidance is not the same as an approval decision                                                                                      |
| SBAS service availability | Service-provider definitions, NOTAM/status, AIP/regulator material       | Future service-provider notes needed                                  | Do not infer availability from architecture                                                                                           |
| LPV procedures            | Equipment MOPS + procedure design + AIP/regulator/operator sources       | LPV page is source-scaffold-linked                                    | Do not publish minima without procedure/source context                                                                                |
| GBAS                      | GBAS standards, local service approvals, airport-specific publications   | Current GBAS notes remain educational scaffolds                       | Do not compare precision using unsourced generic numbers                                                                              |
| ABAS/RAIM                 | Receiver standards, PBN/regulator guidance, aircraft equipment approvals | Current notes are conceptual                                          | Do not treat RAIM as interchangeable with SBAS integrity                                                                              |

## Comparison rules

When comparing SBAS with GBAS, ABAS, RAIM, or other augmentation methods:

1. Compare architecture and source family first.
2. Compare numerical performance only after matching source types are available.
3. Avoid mixing airborne-equipment standards, service-provider commitments, procedure-design criteria, and regulator approvals in one unsupported table.
4. Treat operational phrases such as available, approved, capable, certified, or precision as source-sensitive terms.

## Current safe summary

- SBAS is a wide-area GNSS augmentation concept with ground monitoring, correction/integrity processing, broadcast, and receiver processing.
- GBAS is local-area augmentation and should be sourced through GBAS-specific standards and airport/service approvals.
- ABAS/RAIM are receiver/onboard integrity concepts and should not be presented as equivalent to SBAS service-level integrity without careful sourcing.
- LPV depends on an approved chain of SBAS service, airborne equipment, published procedure, operator/crew authorization, and real-time integrity conditions.

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS-Standards-Regulation]]
- [[SBAS-vs-Other-Augmentation-Methods]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Doc 9849]]
- [[SBAS Source Backlog]]
- [[SBAS MOC]]
