---
title: Satellite-Based Augmentation System (SBAS) Terminology
description: Controlled terminology page for core SBAS concepts used throughout the knowledge base
tags: [terminology, sbas, gnss, corrections, integrity]
category: core-terminology
created: 2026-04-19
modified: 2026-05-03
version: 3.1
status: reviewed
verification_status: source-routed-core-terminology
---

# Satellite-Based Augmentation System (SBAS) Terminology

## Purpose

This note defines recurring SBAS terms used across the knowledge base. It is now a controlled terminology page, not the main beginner explanation. New readers should start with [[What is SBAS]] and then continue to [[SBAS Architecture]].

Definitions here are concise and intentionally conservative. Exact operational thresholds, message definitions, approval criteria, and service-performance commitments must be traced to the relevant source notes and official documents before being used as authoritative requirements.

## Core terms

| Term                         | Working definition                                                                                                      | Related notes                                                       |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| SBAS                         | Wide-area GNSS augmentation service that broadcasts correction and integrity information to users                       | [[What is SBAS]], [[SBAS Architecture]]                             |
| GNSS                         | Satellite navigation constellations and signals used as the base positioning source                                     | [[SBAS Architecture]]                                               |
| Reference station            | Surveyed ground receiver used to monitor GNSS signal behavior for augmentation processing                               | [[SBAS Architecture]]                                               |
| Master or processing station | Facility/function that estimates corrections, integrity parameters, and broadcast messages                              | [[SBAS Architecture]]                                               |
| Uplink station               | Ground element that sends SBAS messages to the broadcast satellite or payload                                           | [[SBAS Architecture Flow]]                                          |
| SBAS broadcast               | Signal carrying augmentation messages to user receivers                                                                 | [[SBAS Architecture Flow]]                                          |
| SBAS-capable receiver        | User equipment able to receive, decode, and apply SBAS information according to its approval basis                      | [[SBAS Ground Segment and Airborne Receiver Responsibilities]]      |
| SBAS message flow            | Functional path from monitored observations through augmentation messages to receiver processing                        | [[SBAS Signal and Message Flow]]                                    |
| Correction                   | Information used to reduce modeled navigation errors where applicable                                                   | [[SBAS Corrections and Integrity Separation]]                       |
| Integrity                    | Ability to support timely warning when navigation information should not be relied upon for the intended operation      | [[SBAS Integrity]]                                                  |
| Protection level             | Receiver-computed or service-supported bound used to judge whether navigation error remains acceptable for an operation | [[Protection Levels]]                                               |
| Alert limit                  | Operation-specific bound that protection levels must satisfy for the operation to continue                              | [[Alert Limits]]                                                    |
| Availability                 | Probability or proportion of time that service requirements are met in the relevant context                             | [[SBAS-Systems-by-Region-MOC]]                                      |
| Continuity                   | Probability that service remains available for the duration of a defined operation                                      | [[SBAS in Civil Aviation MOC]]                                      |
| LPV                          | Localizer Performance with Vertical guidance; an SBAS-enabled approach concept where approved                           | [[LPV-Approach-Procedure]]                                          |
| APV                          | Approach with vertical guidance; operational family relevant to GNSS/SBAS implementation                                | [[SBAS in Civil Aviation MOC]]                                      |
| GBAS                         | Ground-Based Augmentation System; local-area augmentation, usually airport-centered                                     | [[GBAS-Approach-Procedure]], [[SBAS-vs-Other-Augmentation-Methods]] |
| ABAS                         | Aircraft-Based Augmentation System; receiver/aircraft-side monitoring rather than a regional broadcast service          | [[SBAS-vs-Other-Augmentation-Methods]], [[ASEAN ABAS Concept]]      |

## Terms requiring careful source handling

The following terms are frequently misused or over-generalized:

- **Accuracy**: must be tied to a metric, confidence level, service mode, and source.
- **Integrity**: should not be reduced to “high accuracy”; it is about bounding and alerting.
- **Availability**: may refer to signal availability, service availability, procedure availability, or operational availability; these are not interchangeable.
- **Operational**: can mean a live technical service, a certified aviation service, a published procedure, or an approved aircraft operation. State which meaning is intended.
- **Coverage**: a coverage footprint does not automatically imply approved procedures or service-level compliance at every airport.
- **Readiness**: in regional implementation analysis, readiness includes institutional, regulatory, AIS/AIM, procedure-design, aircraft-equipage, and safety-oversight dimensions.

## Source posture

Terminology in this page is aligned with the site’s current synthesis and source scaffolds. High-priority source anchors include:

- [[SBAS Standards Source Matrix]]
- [[SBAS Core Claim Routing]]
- [[Source - RTCA DO-229]]
- [[Source - ICAO Annex 10 Volume I GNSS SBAS]]
- [[Source - ICAO Doc 9849]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[SBAS Operational Validation Dashboard]]

## See also

- [[What is SBAS]]
- [[SBAS Architecture]]
- [[SBAS Architecture Flow]]
- [[SBAS Signal and Message Flow]]
- [[SBAS Corrections and Integrity Separation]]
- [[SBAS Ground Segment and Airborne Receiver Responsibilities]]
- [[SBAS Core Claim Routing]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[Safety-Terminology]]
- [[Communication-Terminology]]
- [[SBAS-vs-Other-Augmentation-Methods]]
- [[SBAS-Standards-Regulation]]
