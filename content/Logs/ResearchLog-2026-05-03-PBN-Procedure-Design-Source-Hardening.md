---
title: Research Log - 2026-05-03 PBN Procedure-Design Source Hardening
description: Work log for the PBN procedure-design source-hardening cycle that created ICAO/FAA/EASA procedure-design source notes and hardened Aviation/ procedure pages
tags: [log, research, pbn, procedure-design, source-hardening, icao, faa, easa]
created: 2026-05-03
modified: 2026-05-03
status: active
---

# Research Log - 2026-05-03 PBN Procedure-Design Source Hardening

## Purpose

This log documents the PBN procedure-design source-hardening cycle executed on 2026-05-03. The cycle created institutional-grade source notes for ICAO PANS-OPS/PBN and FAA/EASA procedure-design material, then hardened all five Aviation/ procedure pages (LPV, LNAV/VNAV, RNAV, RNP, GBAS) to remove unsourced numerical claims and add proper source routing.

## Problem statement

The Aviation/ procedure pages (LNAV/VNAV, RNAV, RNP, GBAS) contained:

- Unsourced numerical claims: accuracy values, alert limits, detection times, decision heights, weather minima, wind limits, fuel savings percentages, cost figures, and pilot-training hours
- Emoji in titles (not institutional grade)
- Broken or corrupted wikilinks (especially GBAS)
- Mixed wikilink syntax (using `[[Note]](path)` instead of `[[Note]]`)
- No boundary statements distinguishing equipment capability from procedure design
- No links to procedure-design source notes (which did not yet exist)
- Missing frontmatter fields (verification_status, status)

The LPV page had been partially hardened in a previous cycle but still lacked procedure-design source routing.

## Research conducted

### ICAO sources

1. **ICAO Doc 8168 Volume II** (PANS-OPS)
   - ICAO Store page: https://store.icao.int/en/procedures-for-air-navigation-services-pans-aircraft-operations-volume-ii-construction-of-visual-instrument-flight-procedures-doc-8168
   - Edition: 7th Edition, 2020
   - Full title: Procedures for Air Navigation Services (PANS) - Aircraft Operations - Volume II Construction of Visual & Instrument Flight Procedures
   - Purpose: "Intended for the guidance of procedures specialists and describes the essential areas and obstacle clearance requirements for the achievement of safe, regular instrument flight operations"
   - Scope: "Provides basic guidelines to States, and those operators and organizations producing instrument flight charts, that will result in uniform practices at all aerodromes where instrument flight procedures are carried out"

2. **ICAO Doc 9613** (PBN Manual)
   - ICAO Store page: https://store.icao.int/en/performance-based-navigation-pbn-manual-doc-9613
   - Edition: 5th Edition, 2023
   - Full title: Performance Based Navigation (PBN) Manual
   - Purpose: "Identifies the relationship between RNAV and RNP applications and the advantages and limitations of choosing one or the other as the navigation requirement for an airspace concept"
   - Additional: "Provides practical guidance to States, ANSPs and airspace users on how to implement RNAV and RNP applications"

### FAA sources

3. **FAA Order 8260.3G** (TERPS)
   - FAA page: https://www.faa.gov/regulations_policies/orders_notices/index.cfm/go/document.information/documentID/1042947
   - Date issued: 2024-07-01
   - Status: Active
   - Full title: United States Standard for Terminal Instrument Procedures (TERPS)
   - Purpose: "Prescribes standardized methods for design and evaluation of IFPs prescribed under Title 14, Code of Federal Regulations (14 CFR) part 97 as well as other IFPs and ATC procedures not specified under part 97"
   - Applicability: Pertinent to 14 CFR parts 1, 71, 77, 91, 95, 97, 121, 125, 129, 135 and 171

4. **FAA Order 8260.58D** (PBN Instrument Procedure Design)
   - FAA page: https://www.faa.gov/regulations_policies/orders_notices/index.cfm/go/document.information/documentID/1043458
   - Date issued: 2025-01-15
   - Status: Active
   - Full title: United States Standard for Performance Based Navigation (PBN) Instrument Procedure Design
   - Purpose: "Provides guidance for the design and evaluation of Performance Based Navigation (PBN) Instrument Flight Procedures (IFPs)"
   - Scope: PBN IFPs are those based on RNAV or RNP, including transitions to ILS or GBAS/GLS final segment

### EASA sources

5. **EASA Easy Access Rules for ATM/ANS Equipment**
   - EASA page: https://www.easa.europa.eu/en/document-library/easy-access-rules/easy-access-rules-air-traffic-managementair-navigation-0
   - Publication date: 25 November 2024
   - Legal basis: Commission Implementing Regulation (EU) 2023/1769 and Commission Delegated Regulation (EU) 2023/1768
   - Scope: Certification and declaration of ATM/ANS systems and constituents; AMC and GM

6. **EASA PBN Operations Transition**
   - EASA page: https://www.easa.europa.eu/en/domains/air-traffic-management/transition-pbn-operations
   - Scope: Identifies navigation specifications and functionalities for en-route ATS routes, SIDs, STARs, and instrument approach procedures

## Files created

1. `Sources/Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual.md` -- NEW institutional source note with ICAO Store metadata, scope statements, boundary statements, downstream routing, and extraction template
2. `Sources/Source - FAA and EASA Procedure-Design and PBN Material.md` -- NEW institutional source note with FAA/EASA public catalog metadata, boundary statements, downstream routing, and extraction template

## Files modified

3. `Aviation/LNAV-VNAV-Approach-Procedure.md` -- REWRITTEN: removed all unsourced numerical claims, added scope/boundary statements, added source anchors, fixed wikilinks, institutional grade
4. `Aviation/RNAV-Approach-Procedure.md` -- REWRITTEN: same treatment as LNAV/VNAV
5. `Aviation/RNP-Approach-Procedure.md` -- REWRITTEN: same treatment, with emphasis on onboard monitoring/alerting distinction
6. `Aviation/GBAS-Approach-Procedure.md` -- REWRITTEN: same treatment, fixed corrupted wikilinks, added SBAS/GBAS architectural distinction
7. `Aviation/LPV-Approach-Procedure.md` -- UPDATED: added procedure-design source anchors to source section, updated See also links
8. `Standards-Regulation/SBAS Standards Source Matrix.md` -- UPDATED: added procedure-design source notes to claim-routing matrix and claim-type matrix; updated recommended sequence; updated modified date
9. `Sources/SBAS Source Backlog.md` -- UPDATED: updated procedure-design section; marked item 4 as completed in suggested execution order; updated modified date
10. `MOCs/SBAS-in-Civil-Aviation-MOC.md` -- UPDATED: changed editorial status of LNAV/VNAV, RNAV, RNP, GBAS from "draft educational scaffold" to "reviewed; source-scaffold-linked"; added source-routing table; updated modified date

## QA results

### Pre-commit checks to run

- [ ] Prettier formatting pass on all modified files
- [ ] Quartz build (expect 113+ Markdown files, no errors)
- [ ] Wikilink audit (expect 0 broken wikilinks)
- [ ] Publication/privacy audit (expect no local paths, secrets, or backup paths)

## Boundary decisions

1. **Two source notes instead of four**: Combined ICAO Doc 8168 Vol II and Doc 9613 into one ICAO source note, and FAA TERPS/8260.58D/EASA material into one FAA/EASA source note, following the pattern of the FAA/EASA TSO/ETSO pair from the previous cycle.

2. **Verification status**: Both new source notes use `public-catalog-reviewed-not-source-extracted` to signal that public catalog metadata supports document identity and purpose, but direct text extraction has not been performed.

3. **Procedure pages**: All five Aviation/ procedure pages now use the same institutional structure as the previously hardened LPV page, with explicit scope/boundary statements, no numerical claims, proper wikilink syntax, and source routing.

4. **No EASA direct text extraction**: EASA AMC/GM material is referenced in the FAA/EASA source note but not directly extracted. Future cycles should identify exact AMC/GM document numbers and editions for PBN operational approval.

## Recommended next cycles

1. **Direct extraction of ICAO Doc 8168 Vol II**: Extract procedure-design criteria for instrument approach procedures, obstacle clearance surfaces, and SBAS/APV/LPV-specific material.
2. **Direct extraction of ICAO Doc 9613**: Extract RNP navigation specifications, RNAV/RNP comparison material, and implementation guidance.
3. **Direct extraction of FAA Order 8260.3G and 8260.58D**: Extract U.S. TERPS criteria and PBN procedure-design criteria.
4. **Service-provider source notes**: Create source notes for WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, SouthPAN service definitions before publishing comparative performance tables.
5. **Annex 10 extraction**: Continue extracting ICAO Annex 10 Volume I GNSS/SBAS technical provisions.

## Related notes

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - ICAO PANS-OPS Doc 8168 and Doc 9613 PBN Manual]]
- [[Source - FAA and EASA Procedure-Design and PBN Material]]
- [[LPV-Approach-Procedure]]
- [[LNAV-VNAV-Approach-Procedure]]
- [[RNAV-Approach-Procedure]]
- [[RNP-Approach-Procedure]]
- [[GBAS-Approach-Procedure]]
- [[SBAS in Civil Aviation MOC]]
