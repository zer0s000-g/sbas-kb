---
title: SBAS in Civil Aviation MOC
description: Institutional map of how SBAS connects to civil aviation operations, approach procedures, integrity, and regulatory approval
tags: [MOC, civil-aviation, sbas, approach, operations, integrity]
category: mocs
created: 2026-04-19
modified: 2026-05-02
version: 2.0
status: reviewed
verification_status: source-scaffold-linked
---

# SBAS in Civil Aviation MOC

## Scope

This note maps the aviation-operations branch of the knowledge base. It explains how SBAS relates to approach procedures, integrity concepts, operational approval, and implementation planning.

It is not an operational manual. Do not use this page to determine procedure minima, aircraft eligibility, crew authorization, or service availability. Those decisions require the applicable AIP, procedure chart, avionics approval, operator approval, regulator material, and service-provider documentation.

## Core aviation logic

SBAS contributes to civil aviation by combining wide-area GNSS augmentation with integrity information that can support approved operations. The operational chain has several layers:

1. a certified or otherwise approved SBAS service is available for the intended area and operation;
2. the aircraft has suitable SBAS-capable equipment and installation approval;
3. the procedure is designed, published, and maintained by the appropriate authority;
4. the crew and operator are authorized for the operation;
5. the receiver indicates that the required performance and integrity conditions are satisfied during the operation.

A weak link in any layer can prevent operational use even when the technical SBAS signal is present.

## Approach and navigation concepts

| Concept                          | Role in the knowledge base                                         | Editorial status                 |
| -------------------------------- | ------------------------------------------------------------------ | -------------------------------- |
| [[LPV-Approach-Procedure]]       | SBAS-enabled vertical guidance learning note                       | reviewed; source-scaffold-linked |
| [[LNAV-VNAV-Approach-Procedure]] | vertical navigation context and comparison path                    | draft educational scaffold       |
| [[RNAV-Approach-Procedure]]      | area-navigation context                                            | draft educational scaffold       |
| [[RNP-Approach-Procedure]]       | performance-based navigation context                               | draft educational scaffold       |
| [[GBAS-Approach-Procedure]]      | local-area augmentation comparison                                 | draft educational scaffold       |
| [[SBAS Integrity]]               | safety-relevant function connecting system monitoring to operation | reviewed; source-scaffold-linked |
| [[Protection Levels]]            | bounded-error concept used in operational usability checks         | reviewed; source-scaffold-linked |
| [[Alert Limits]]                 | operation-specific bounds and alerting interpretation              | reviewed; source-scaffold-linked |

## Integrity, protection levels, and alert limits

In aviation, SBAS must be understood through integrity rather than accuracy alone.

- [[SBAS Integrity]] explains why timely warning and bounded error are central.
- [[Protection Levels]] explain the receiver/service-side bound concept.
- [[Alert Limits]] explain the operation-specific threshold concept.

A simplified operational relationship is:

```text
If the relevant protection level is within the applicable alert limit,
and all other service/equipment/procedure/approval conditions are satisfied,
then the operation may continue under the approved procedure basis.
```

This relationship is conceptual. Exact definitions and thresholds must come from authoritative standards and approved operational material.

## Operational benefits to evaluate

SBAS may support:

- wider access to vertically guided approach procedures where ground navaids are limited;
- improved operational resilience for remote, island, mountainous, or distributed airport networks;
- more consistent regional navigation capability for equipped aircraft;
- reduced dependence on some legacy ground infrastructure, depending on local safety and regulatory decisions;
- improved basis for PBN implementation where procedures, oversight, and equipage are aligned.

These benefits are context-dependent. They should be evaluated against real airport networks, procedure inventories, traffic needs, terrain/weather constraints, equipage, and regulator/ANSP readiness.

## Regional implementation context

Regional branches relevant to civil aviation include:

- [[SBAS-Systems-by-Region-MOC]] — global system comparison and regional implementation map.
- [[Asia-Pacific SBAS Implementation Patterns]] — Asia-Pacific synthesis.
- [[ASEAN SBAS Adoption Landscape]] — Southeast Asian adoption framing.
- [[ASEAN SBAS Operational Demand Drivers]] — why SBAS may matter operationally in ASEAN.
- [[ASEAN SBAS Deployment Barriers]] — why implementation is difficult.
- [[ASEAN SBAS Governance and Institutional Actors]] — institutional pathway analysis.
- [[ASEAN SBAS Service-Model Options]] — possible regional service models.

## Standards and source anchors

Current source scaffolds relevant to aviation operations include:

- [[SBAS Standards Source Matrix]]
- [[Source - RTCA DO-229]] — current GPS/SBAS airborne-equipment anchor; approval and installation context still requires FAA/EASA/regulator source separation.
- [[Source - ICAO Doc 9849]] — current ICAO GNSS implementation-guidance anchor.
- [[Source - RTCA DO-242]], [[Source - RTCA DO-289]], [[Source - ICAO Doc 9854]], and [[Source - ICAO Doc 9855]] — retained as red-flag provenance notes because earlier drafts likely mis-scoped them for SBAS.
- [[SBAS Source Backlog]]

Several earlier notes contain numerical values or operational examples that should be treated as provisional until tied to the correct official source family.

## Open source-hardening tasks

1. Verify exact standards and guidance references for SBAS-supported aviation procedures.
2. Separate LPV, APV, LNAV/VNAV, RNAV, and RNP terminology carefully.
3. Replace generic benefit percentages with sourced case studies or remove them.
4. Tie any minima, alerting, or performance figures to specific standards, service definitions, or regulator material.
5. Add country- or airport-level evidence only when the relevant AIP/AIS/procedure source is visible.

## See also

- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS MOC]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[ASEAN SBAS Source Backlog]]
