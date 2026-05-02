---
title: Source - FAA TSO-C145e and TSO-C146e
description: Source note for FAA TSO-C145e/C146e as the U.S. article-approval layer for GPS augmented by WAAS airborne sensors and stand-alone navigation equipment, with strict separation from installation and operational approval
tags: [source, faa, tso, tso-c145e, tso-c146e, waas, sbas, gps, airborne-equipment, approval]
source_type: regulator-standard
created: 2026-05-02
modified: 2026-05-02
status: active
verification_status: public-regulator-source-reviewed-specific-tso-text-not-directly-extracted
---

# Source - FAA TSO-C145e and TSO-C146e

## Scope of this note

This note is the knowledge base's current FAA source-family anchor for **TSO-C145e** and **TSO-C146e**, the U.S. Technical Standard Order layer associated with GPS augmented by WAAS airborne equipment.

It is an approval-context routing note, not a completed legal or engineering extraction of the full FAA TSO PDFs. Public FAA material and FAA Dynamic Regulatory System search results were reviewed; the Dynamic Regulatory System pages identify the relevant TSO records, but the full DRS text was not reliably extractable in this cycle.

Important boundary:

- FAA TSO material supports article-level minimum-performance and design/production approval context.
- A TSO authorization is not an aircraft installation approval.
- A TSO authorization is not an operational approval, operator authorization, procedure authorization, or LPV availability statement.
- Do not use this note to publish equipment-class details, deviations, test tolerances, operational minima, or aircraft eligibility unless the applicable TSO text, aircraft approval basis, avionics documentation, and operational sources are directly checked.

## Public identity and document signals reviewed

| Field                                 | Public signal reviewed                                                                                                                                           |
| ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Issuing authority                     | Federal Aviation Administration                                                                                                                                  |
| Source family                         | Technical Standard Orders                                                                                                                                        |
| Document records located              | FAA DRS records for TSO-C145e and TSO-C146e                                                                                                                      |
| TSO-C145e public title signal         | Airborne navigation sensors using GPS augmented by WAAS                                                                                                          |
| TSO-C146e public title signal         | Stand-alone airborne navigation equipment using GPS augmented by WAAS                                                                                            |
| Public DRS signal for TSO-C145e       | DRS search result identifies `TSO-C145e.pdf` and references an RTCA/DO-229E change option in Appendix 3                                                          |
| Public DRS signal for TSO-C146e       | DRS search result identifies Class Delta-4 context and RTCA/DO-229E Section 1.4 relationship                                                                     |
| General FAA TSO policy signal         | FAA defines TSO as a minimum performance standard and states that TSO Authorization is not installation approval                                                 |
| Related airworthiness guidance signal | FAA AC 20-138B is installation/airworthiness guidance for positioning and navigation equipment; it distinguishes TSOA/LODA from installed operational compliance |

## FAA TSO policy boundary

FAA's public Technical Standard Orders page states that a TSO is a minimum performance standard used to evaluate an article. It also states that receiving a TSO Authorization is **not** approval to install and use the article in an aircraft. The article may be installed only after showing that it meets the specific airworthiness requirements for the aircraft model.

For this knowledge base, that supports a strong editorial rule:

```text
TSO-C145e/C146e evidence can help classify the article-approval source layer.
It does not, by itself, approve an aircraft installation, operator, crew, procedure,
runway, region, or LPV operation.
```

## Relationship to DO-229

[[Source - RTCA DO-229]] remains the equipment MOPS source-family anchor. This FAA TSO note is the U.S. regulator/article-approval layer that may reference or modify the use of DO-229 material for FAA approval purposes.

This distinction matters because downstream pages often need both layers:

| Claim type                          | Source routing                                                                                                          |
| ----------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Receiver/equipment MOPS family      | [[Source - RTCA DO-229]]                                                                                                |
| U.S. article approval against a TSO | This source note plus direct FAA TSO text                                                                               |
| Aircraft installation approval      | FAA airworthiness/installation approval basis, AC guidance, certification data, aircraft/avionics installation material |
| Operational approval or use         | FAA operational guidance, operator authorization, procedure charts/AIP/AIS, avionics limitations, crew procedures       |
| LPV procedure availability          | Service status, procedure-design/AIP material, aircraft/operator approval, and real-time integrity conditions           |

## What this source can currently anchor

This note can currently support only conservative source-routing statements:

- FAA TSO-C145e/C146e belong to the U.S. regulator/article-approval source family for GPS augmented by WAAS airborne equipment.
- TSO-C145e is associated with GPS/WAAS airborne navigation sensors.
- TSO-C146e is associated with stand-alone GPS/WAAS airborne navigation equipment.
- FAA public TSO policy explicitly separates TSO Authorization from aircraft installation approval.
- Approval-specific statements must be separated from DO-229 MOPS statements and from operational-use statements.

## What this source must not be used for yet

Do not use this note alone to publish or validate:

- exact TSO-C145e or TSO-C146e requirements;
- equipment class definitions, deviations, appendices, or test methods;
- whether a specific receiver, aircraft, operator, or installation is approved;
- LPV, LP, LNAV/VNAV, RNAV, or alternate-planning operational eligibility;
- procedure minima or charting claims;
- claims about continuing validity of a particular TSOA, LODA, STC, TC, AFMS, or avionics configuration;
- equivalence between FAA TSO and EASA ETSO requirements.

## Extraction template for a future direct FAA cycle

### Documents to extract directly

- FAA TSO-C145e full text from the FAA Dynamic Regulatory System.
- FAA TSO-C146e full text from the FAA Dynamic Regulatory System.
- FAA AC 21-46 for the TSO program, if approval-process detail is needed.
- FAA AC 21-50 for installation of TSOA articles and LODA appliances, if installation boundary detail is needed.
- FAA AC 20-138B or its current successor for installed positioning/navigation equipment airworthiness approval.

### Fields to map

- exact title and effective date;
- cancellation/supersession status;
- referenced RTCA/DO-229 revision and change baseline;
- equipment classes and applicability;
- appendices and deviations;
- marking, installation-manual, and limitation requirements;
- software/hardware/environmental assurance references;
- explicit statements separating TSO authorization from installation or operational use.

## Downstream documentation rules

When editing downstream pages:

1. Use this source note for FAA article-approval routing only.
2. Pair it with [[Source - RTCA DO-229]] for receiver/equipment MOPS context.
3. Pair it with aircraft installation and operational sources before writing any operational-use claim.
4. Never convert a TSO title into an aircraft eligibility claim.
5. Never convert a TSO/DO-229 reference into regional LPV availability.

## Public sources reviewed

- FAA Technical Standard Orders page: `https://www.faa.gov/aircraft/air_cert/design_approvals/tso`
- FAA Dynamic Regulatory System record for TSO-C145e: `https://drs.faa.gov/browse/excelExternalWindow/EFE54F1E6272A7068625811D0064B679.0001`
- FAA Dynamic Regulatory System record for TSO-C146e: `https://drs.faa.gov/browse/excelExternalWindow/EFE10BFF3187F9A78625811A005E32A6.0001`
- FAA AC 20-138B public PDF: `https://www.faa.gov/documentLibrary/media/Advisory_Circular/AC%2020-138B.pdf`

## See also

- [[Source - RTCA DO-229]]
- [[Source - EASA ETSO-C145e and ETSO-C146e]]
- [[SBAS Standards Source Matrix]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[LPV-Approach-Procedure]]
- [[SBAS Integrity]]
