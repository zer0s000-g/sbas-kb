---
title: Source - EASA ETSO-C145e and ETSO-C146e
description: Source note for EASA ETSO-C145e/C146e as the European article-approval layer for GPS/SBAS airborne navigation sensors and stand-alone navigation equipment, with extracted public PDF signals and approval-boundary rules
tags: [source, easa, etso, etso-c145e, etso-c146e, sbas, gps, airborne-equipment, approval]
source_type: regulator-standard
created: 2026-05-02
modified: 2026-05-02
status: active
verification_status: public-pdf-extracted-with-official-text-boundaries
---

# Source - EASA ETSO-C145e and ETSO-C146e

## Scope of this note

This note is the knowledge base's current EASA source-family anchor for **ETSO-C145e** and **ETSO-C146e A1**, the European Technical Standard Order layer associated with GPS/SBAS airborne navigation equipment.

Public EASA PDFs were retrieved and text-extracted in this cycle. This note records source-family identity, applicability boundaries, and downstream editorial rules. It is not a substitute for the official EASA CS-ETSO text, a Declaration of Design and Performance, aircraft certification basis, installation approval, operational approval, or avionics manual.

## Public identity and document signals reviewed

| Field                       | ETSO-C145e public signal                                | ETSO-C146e A1 public signal                                                                                               |
| --------------------------- | ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Issuing authority           | EASA                                                    | EASA                                                                                                                      |
| Decision / amendment signal | ED Decision 2018/002/R; CS-ETSO Amendment 13            | ED Decision 2020/011/R; CS-ETSO Amendment 16                                                                              |
| Applicability date signal   | 21 February 2018                                        | Applicable from 25 July 2020                                                                                              |
| Public subject signal       | Airborne navigation sensors using GPS augmented by SBAS | Stand-alone airborne navigation equipment using GPS augmented by SBAS                                                     |
| DO-229 relationship         | RTCA DO-229E Section 2 as modified by ETSO appendices   | RTCA DO-229E Section 2 as amended by ETSO appendices                                                                      |
| Equipment class signal      | Functional equipment Class Beta                         | Functional equipment Class Gamma or Delta; A1 adds an option involving an ETSO-2C205a Class Delta CCA functional sensor   |
| Integration boundary        | Does not address integration issues with other avionics | Except for ADS with Class Gamma, integration with other avionics is not addressed; aircraft-level requirements may differ |

## ETSO-C145e extracted scope signal

The public ETSO-C145e text applies to airborne navigation sensors using GPS augmented by SBAS that provide position, velocity, and time information to navigation-management units or non-navigation applications. It points to DO-229E Section 2 for Class Beta equipment, as modified by ETSO appendices.

For this knowledge base, ETSO-C145e should be routed as:

```text
European article-approval source family for GPS/SBAS navigation sensors,
not a complete aircraft installation or operational-use approval.
```

## ETSO-C146e A1 extracted scope signal

The public ETSO-C146e A1 text applies to stand-alone airborne navigation equipment using GPS augmented by SBAS. It identifies DO-229E Section 2 as the MPS basis for functional equipment Class Gamma or Delta, as amended by ETSO appendices. The A1 material introduces an option for using an ETSO-2C205a Class Delta circuit-card-assembly functional sensor, while stating there is no technical MOPS change compared with ETSO-C146e.

For this knowledge base, ETSO-C146e should be routed as:

```text
European article-approval source family for stand-alone GPS/SBAS navigation equipment,
not a blanket approval for an aircraft, operator, procedure, runway, or region.
```

## Approval and integration boundaries

The extracted EASA material contains several boundary signals that should be preserved in downstream writing:

- ETSO-C145e and ETSO-C146e depend on RTCA DO-229E, but with EASA appendices/modifications.
- Equipment can have antenna-related limitations that must appear in the installation manual when applicable.
- GEO satellite bias data must be available for EASA review under the extracted provisions.
- Failure-condition classifications are minimum equipment-level classifications; aircraft-level certification specifications may require different classifications.
- Integration with other avionics is explicitly outside or limited in the extracted scope.
- A Class Delta CCA option in ETSO-C146e A1 does not make the end-use manufacturer responsibility disappear.

## Relationship to DO-229 and FAA TSOs

[[Source - RTCA DO-229]] is the equipment MOPS source-family anchor. This EASA ETSO note is the European article-approval layer that references DO-229E and adds EASA-specific modifications and approval context.

[[Source - FAA TSO-C145e and TSO-C146e]] is the U.S. regulator/article-approval counterpart. The FAA and EASA paths should be compared cautiously. Similar titles and common DO-229 references do not by themselves prove identical approval conditions, identical appendices, identical deviations, or mutual operational approval.

## What this source can currently anchor

This note can support these statements:

- EASA ETSO-C145e is an approval-layer source for GPS/SBAS airborne navigation sensors.
- EASA ETSO-C146e A1 is an approval-layer source for stand-alone GPS/SBAS airborne navigation equipment.
- Both source families visibly rely on RTCA DO-229E Section 2, modified or amended by EASA ETSO appendices.
- ETSO-C145e is associated with Class Beta equipment in the extracted public text.
- ETSO-C146e A1 is associated with Class Gamma or Delta equipment in the extracted public text.
- EASA material preserves installation/manual, antenna, GEO-bias, failure-classification, and aircraft-integration boundaries that prevent overclaiming.

## What this source must not be used for alone

Do not use this note alone to publish or validate:

- a claim that a specific aircraft installation is approved;
- a claim that a specific operator, crew, procedure, route, runway, or region is operationally approved;
- LPV minima, LPV availability, or charting status;
- complete equipment-class definitions or all DO-229 requirements;
- test tolerances, algorithms, receiver annunciation behavior, or protection-level formulas;
- FAA equivalence, bilateral validation, or export/import approval conclusions;
- DFMC or multi-constellation requirements not explicitly supported by the applicable official source.

## Downstream documentation rules

When editing downstream pages:

1. Use ETSO-C145e for European GPS/SBAS navigation-sensor article-approval routing.
2. Use ETSO-C146e for European stand-alone GPS/SBAS navigation-equipment article-approval routing.
3. Pair either ETSO with [[Source - RTCA DO-229]] for MOPS context.
4. Pair ETSO material with aircraft-level certification, installation, avionics, operator, and AIP/procedure sources before any operational claim.
5. Preserve the difference between equipment-level failure classification and aircraft-level safety assessment.
6. Preserve the difference between article approval and installation/integration approval.

## Extraction template for a future EASA cycle

### Sections to map with official section references

- applicability and subject;
- minimum performance standard paragraph;
- functional and operational equipment-class language;
- appendices modifying DO-229E;
- cybersecurity/spoofing and data-validity language;
- antenna limitation and installation-manual provisions;
- GEO satellite-bias data requirement;
- failure-condition classification;
- marking and DDP requirements;
- ETSO-2C205a Class Delta CCA integration option under ETSO-C146e A1;
- availability of referenced documents.

### Downstream pages to revisit after extraction

- [[Source - RTCA DO-229]]
- [[SBAS Standards Source Matrix]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Integrity]]
- [[Protection Levels]]
- [[Alert Limits]]
- [[LPV-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]

## Public sources reviewed

- EASA ETSO-C145e public PDF: `https://www.easa.europa.eu/download/etso/ETSO-C145e_CS-ETSO_13.pdf`
- EASA ETSO-C146e A1 public PDF: `https://www.easa.europa.eu/download/etso/ETSO-C146e_A1.pdf`
- EASA list of current and historic ETSOs: `https://www.easa.europa.eu/en/domains/aircraft-products/etso/list-of-all-etso`
- EASA NPA 2017-08 public PDF, used as harmonisation/context signal only: `https://www.easa.europa.eu/sites/default/files/dfu/NPA%202017-08.pdf`

## See also

- [[Source - RTCA DO-229]]
- [[Source - FAA TSO-C145e and TSO-C146e]]
- [[SBAS Standards Source Matrix]]
- [[SBAS-Standards-Regulation]]
- [[SBAS Source Backlog]]
- [[LPV-Approach-Procedure]]
- [[SBAS Integrity]]
