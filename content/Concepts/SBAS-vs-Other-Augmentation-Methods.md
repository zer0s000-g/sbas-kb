---
title: SBAS vs Other Augmentation Methods
description: Source-disciplined comparison of SBAS with GBAS, ABAS, RAIM, and related augmentation concepts
tags: [comparison, augmentation-methods, sbas, gbas, abas, raim, integrity]
category: concepts
created: 2026-04-19
modified: 2026-05-02
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# SBAS vs Other Augmentation Methods

## Scope

This page compares augmentation concepts at an educational level. It intentionally avoids unsupported numerical accuracy, coverage, latency, alerting, and benefit claims. Exact performance and operational eligibility must be checked against authoritative standards, service-provider documentation, regulator material, AIP/procedure publications, aircraft/avionics approvals, and operator procedures.

## Short comparison

| Method | Core idea                                                                                                                             | Typical source family needed                                                   | Main caution                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ----------------------------------------------------------------------------- |
| SBAS   | Wide-area GNSS augmentation using a monitored reference network, correction/integrity processing, and broadcast to equipped receivers | ICAO GNSS/SBAS material, service-provider definitions, airborne-equipment MOPS | Do not infer operational approval from signal availability alone              |
| GBAS   | Local-area GNSS augmentation serving a specific airport or local service volume                                                       | GBAS standards, airport/service approvals, AIP/procedure material              | Local precision service is not interchangeable with continental SBAS          |
| ABAS   | Aircraft/receiver-based augmentation and integrity support using onboard processing and available signals                             | Receiver standards, aircraft equipment approval, PBN/regulator guidance        | Receiver autonomy is not the same as external SBAS service monitoring         |
| RAIM   | Receiver autonomous integrity monitoring using satellite geometry and consistency checks                                              | Receiver standards, PBN/regulator guidance, aircraft/equipment approvals       | RAIM availability and suitability depend on operation, receiver, and geometry |

## Architecture distinction

SBAS and GBAS both augment GNSS, but they solve different deployment problems:

- SBAS is designed for wide-area service provision and can support many users across a large service region when service, procedure, equipment, and regulatory conditions are met.
- GBAS is designed around local-area augmentation, usually tied to an airport or local service environment.
- ABAS and RAIM are onboard/receiver-side concepts rather than external wide-area augmentation services.

## Aviation-use distinction

[[LPV-Approach-Procedure]] is an SBAS-supported approach concept, not a GBAS procedure. Earlier draft wording in this vault blurred that distinction. The corrected interpretation is:

- LPV is associated with SBAS-capable airborne equipment and an approved SBAS-supported procedure environment.
- GBAS supports its own local-area precision-approach concepts and should be documented through GBAS-specific standards and airport/service sources.
- LNAV/VNAV, RNAV, RNP, ABAS, and RAIM concepts need their own source-disciplined procedure and equipment notes.

## Integrity distinction

Integrity is not simply higher accuracy.

- [[SBAS Integrity]] explains SBAS integrity as the safety-relevant use-or-non-use function.
- [[Protection Levels]] explain bounded-error concepts.
- [[Alert Limits]] explain operation-specific usability thresholds.
- ABAS/RAIM integrity concepts should not be presented as equivalent to SBAS service-level integrity without source-specific language.

## Current source anchors

- [[SBAS Standards Source Matrix]] — current claim-routing matrix.
- [[Source - RTCA DO-229]] — current GPS/SBAS airborne-equipment source-family anchor.
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]] — current ICAO SARPs/technical-provisions source-family routing anchor for GNSS/SBAS.
- [[Source - ICAO Doc 9849]] — current ICAO GNSS implementation-guidance source-family anchor.
- [[Source - RTCA DO-242]], [[Source - RTCA DO-289]], [[Source - ICAO Doc 9854]], and [[Source - ICAO Doc 9855]] — red-flag notes documenting earlier mis-scoped references.

## Open source-hardening needs

1. Directly extract [[Source - ICAO Annex 10 Volume I GNSS SBAS]] before expanding GNSS/SBAS technical-baseline claims.
2. Create procedure-design source notes before expanding RNAV, RNP, LNAV/VNAV, LPV, or GBAS procedure comparisons.
3. Create service-provider source notes before publishing regional performance comparisons.
4. Replace generic numerical tables only with source-anchored, context-specific values.

## See also

- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS Integrity]]
- [[LPV-Approach-Procedure]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[SBAS MOC]]
