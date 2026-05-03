---
title: Research Log - 2026-05-03 - SDCM and Operational Validation Source Hardening
description: Work log for five-cycle SBAS source-hardening pass covering SDCM, operational-validation routing, synthesis hardening, source backlog refresh, and publication QA
tags: [research-log, sbas, sdcm, validation, source-hardening, service-provider]
created: 2026-05-03
modified: 2026-05-03
status: complete
verification_status: implementation-log
---

# Research Log - 2026-05-03 - SDCM and Operational Validation Source Hardening

## Cycle scope

This five-cycle pass continued the institutional SBAS knowledge-base source-hardening program after the major service-provider child-source notes were created.

Primary goals:

1. represent SDCM without overstating current operational evidence;
2. prevent child service-provider notes from drifting into regulator/AIP/procedure claims;
3. harden cross-system synthesis pages against unsupported maturity/performance comparisons;
4. refresh backlog and source-routing matrix posture;
5. run publication QA, commit, push, and verify live Quartz deployment.

## Source evidence reviewed

| Topic                    | Public evidence used                                                                                                  | KB treatment                                                                                                      |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| SDCM / GLONASS IAC       | GLONASS IAC system-documents page and GLONASS OS PS Edition 2.2                                                       | Official GLONASS source posture; supports SDCM as GLONASS-based-system context, not aviation operational approval |
| SDCM / ICAO              | ICAO Assembly A37-WP/195 Russian Federation GLONASS working paper                                                     | Historical development-context signal; not current service declaration                                            |
| SDCM / public comparator | FAA SBAS Worldwide factsheet and UNOOSA-hosted Russian GNSS presentation search/extraction context                    | Bounded comparator/development status only                                                                        |
| Operational validation   | Existing source-family structure across standards, service-provider, procedure-design, TSO/ETSO, regulator/AIP layers | New dashboard routing layer, not original evidence                                                                |

## Files created

- [[Source - SDCM]]
- [[SDCM]]
- [[SBAS Operational Validation Dashboard]]

## Files strengthened

- [[Source - SBAS Service Providers]]
- [[SBAS Source Backlog]]
- [[SBAS Standards Source Matrix]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS MOC]]
- [[MSAS vs GAGAN]]
- [[Asia-Pacific SBAS Implementation Patterns]]

## Documentation-quality decisions

### SDCM evidence posture

SDCM was added as a source-routed system, but intentionally not upgraded to the same evidence posture as systems with current service-definition or provider material.

The KB can now say that SDCM has GLONASS/IAC and historical ICAO development-context support. It cannot say that SDCM currently provides aviation Safety-of-Life service, LPV/APV procedure availability, AIP-published procedures, service-volume commitments, or operational approval.

### Operational validation separation

A new dashboard was created because service-provider notes were becoming mature enough to create a new risk: readers might mistake service-definition or source-posture evidence for operational approval.

The dashboard owns only the validation ladder. It does not duplicate detailed system facts and does not act as original evidence for any operational claim.

### Synthesis hardening

[[MSAS vs GAGAN]] was rewritten from draft in-vault synthesis into a source-routed comparison that compares evidence posture rather than system maturity. [[Asia-Pacific SBAS Implementation Patterns]] now includes SDCM only as a bounded GLONASS augmentation research target, not as proof of regional operational equivalence.

## Open follow-up targets

1. Current official Russian SDCM service-definition/status evidence.
2. Russian regulator/AIP evidence before any SDCM aviation-use claim.
3. Regulator/AIP/procedure validation for WAAS, EGNOS, GAGAN, MSAS, KASS, BDSBAS, and SouthPAN operational claims.
4. Direct extraction of Annex 10, DO-229, and Doc 9849 sections before numerical operational values are published.
5. ASECNA / ANGA source note only after official public evidence is extracted.

## See also

- [[Source - SDCM]]
- [[SDCM]]
- [[SBAS Operational Validation Dashboard]]
- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - SBAS Service Providers]]
