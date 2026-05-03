---
title: SBAS Operational Validation Dashboard
description: Institutional dashboard separating SBAS service-provider evidence from regulator, ANSP, AIP, procedure, aircraft, and operator evidence required for operational aviation claims
tags: [dashboard, validation, aviation, sbas, sources, operations, provenance]
category: standards
created: 2026-05-03
modified: 2026-05-03
status: active
verification_status: source-routing-dashboard-no-operational-approval
---

# SBAS Operational Validation Dashboard

## Purpose

This dashboard prevents service-provider source notes from being misused as operational aviation approval evidence.

A service-provider source can describe a system, a signal, a service definition, or a status snapshot. It does not automatically prove that an aircraft, operator, runway, procedure, state, or flight operation is authorized to use that service.

## Non-overlap rule

Do not duplicate detailed claims from child source notes here. This dashboard owns only the validation pathway: which evidence layer is still required before a claim becomes operationally safe to publish.

System-specific facts belong in the child source notes:

- [[Source - WAAS]]
- [[Source - EGNOS]]
- [[Source - GAGAN SBAS Operation]]
- [[Source - MSAS]]
- [[Source - BDSBAS]]
- [[Source - KASS]]
- [[Source - SouthPAN]]
- [[Source - SDCM]]

## Claim validation ladder

| Evidence layer                                 | What it can support                                                 | What it cannot support alone                                               |
| ---------------------------------------------- | ------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| Service-provider identity source               | System name, provider, high-level service or development status     | Procedure availability, aircraft/operator authorization, procedure minima  |
| Service-definition / performance report        | Service area, commitments, status, limitations, performance framing | Published airport/runway procedures unless linked to AIP/procedure sources |
| Standards / MOPS                               | Equipment function, integrity concepts, technical requirements      | Service availability, aircraft installation approval, operational approval |
| TSO / ETSO article approval                    | Approved equipment article context                                  | Installation approval, operator authorization, route/procedure eligibility |
| Procedure-design / PBN source                  | Design criteria and navigation-specification context                | Airport-specific published procedure availability                          |
| Regulator / ANSP / AIP / procedure publication | State or runway-specific operational procedure evidence             | General service-provider performance unless linked to service documents    |
| Aircraft / avionics / operator documentation   | Specific equipage and operational eligibility                       | System-wide status or public service commitments                           |

## Current system validation posture

| System       | Child source note                 | Current safe posture                                                         | Operational validation still needed                                                                                                      |
| ------------ | --------------------------------- | ---------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| [[WAAS]]     | [[Source - WAAS]]                 | FAA public WAAS material and procedure-count snapshots extracted             | FAA procedure/NFDC/AIP-style procedure records, current performance/status reports, aircraft/operator eligibility for specific use cases |
| [[EGNOS]]    | [[Source - EGNOS]]                | EGNOS SoL SDD source posture extracted                                       | National AIP/ANSP/regulator procedure evidence, EGNOS performance/status reports, aircraft/operator authorization evidence               |
| [[MSAS]]     | [[Source - MSAS]]                 | QZSS and ICAO APAC historical/current transmission-service context extracted | Current JCAB/MLIT/QZSS/AIP evidence for post-2023 LPV or APV operational status                                                          |
| [[GAGAN]]    | [[Source - GAGAN SBAS Operation]] | ICAO APAC ITF/7 and AAI FAQ source signals extracted                         | DGCA/AAI/AIP procedure-level confirmation, current procedure lists, aircraft/operator approval conditions                                |
| [[BDSBAS]]   | [[Source - BDSBAS]]               | BDSBAS-B1C ICD and bounded technical development context extracted           | CAAC/regulator aviation service declaration, procedure publication, service-performance status                                           |
| [[KASS]]     | [[Source - KASS]]                 | KARI, ICAO APAC, and bounded certification/status signals extracted          | Korean regulator/AIP/ANSP evidence for APV/LPV procedure availability and operational use                                                |
| [[SouthPAN]] | [[Source - SouthPAN]]             | Open Services / SIS Open Services evidence extracted                         | CASA/Airservices/LINZ/ANSP/AIP evidence for certified aviation SoL use and procedure availability                                        |
| [[SDCM]]     | [[Source - SDCM]]                 | GLONASS/IAC and historical ICAO development-context evidence extracted       | Current Russian SDCM service-definition, aviation regulator/AIP evidence, service-performance and procedure evidence                     |

## Publication rules

A page may say a system is represented by a source note only when the source note exists and states its permitted claims.

A page must not say a system supports operational LPV/APV use unless the relevant regulator/ANSP/AIP/procedure evidence is extracted and linked.

A page must not compare systems by availability, accuracy, continuity, service maturity, interoperability, or procedure inventory unless each compared system has equivalent official evidence of the same type and snapshot period.

## High-risk phrases requiring source escalation

Treat the following phrases as blocked unless the validation ladder is satisfied:

| Phrase type                        | Required source family before publication                                                           |
| ---------------------------------- | --------------------------------------------------------------------------------------------------- |
| "operationally approved"           | Regulator / ANSP / AIP / operator approval evidence                                                 |
| "LPV procedures available"         | AIP/procedure publication or official procedure inventory                                           |
| "service covers"                   | Current service-definition / performance / service-volume source                                    |
| "better than" / "more mature than" | Matched official performance or procedure evidence across systems                                   |
| "certified for aviation"           | Regulator or official service-provider certification evidence with scope and date                   |
| "supports CAT-I / APV-I"           | Standards/service-definition plus operational approval context; do not infer procedure availability |

## Recommended next extraction queues

1. WAAS: official FAA performance/status and procedure inventory source path.
2. EGNOS: official ESSP/EUSPA performance reports plus national AIP/ANSP procedure evidence.
3. GAGAN: DGCA/AAI/AIP procedure publication and current operational approval detail.
4. MSAS: post-2023 JCAB/MLIT/QZSS status and procedure evidence.
5. KASS: Korean regulator/AIP confirmation of APV/LPV operational procedure use.
6. BDSBAS: CAAC aviation service declaration and procedure evidence.
7. SouthPAN: aviation SoL approval and AIP/procedure evidence after Open Services.
8. SDCM: current official SDCM service-definition and aviation-use evidence.

## See also

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - SBAS Service Providers]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS in Civil Aviation MOC]]
- [[LPV-Approach-Procedure]]
