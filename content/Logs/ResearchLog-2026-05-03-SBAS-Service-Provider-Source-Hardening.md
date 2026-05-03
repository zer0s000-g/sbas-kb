---
title: Research Log - 2026-05-03 SBAS Service-Provider Source Hardening
description: Work log for the SBAS service-provider source-hardening cycle that created an institutional service-provider source note and updated system pages
tags: [log, research, sbas, service-provider, waas, egnos, msas, gagan, bdbsas, kass, southpan]
created: 2026-05-03
modified: 2026-05-03
status: active
---

# Research Log - 2026-05-03 SBAS Service-Provider Source Hardening

## Purpose

This log documents the SBAS service-provider source-hardening cycle executed on 2026-05-03. The cycle created an institutional-grade source note for SBAS service providers (WAAS, EGNOS, MSAS, GAGAN, BDSBAS, KASS, SouthPAN) and updated downstream system pages with proper source routing.

## Problem statement

The SBAS service-provider source family was not yet represented by a dedicated source note. System pages (WAAS, EGNOS, MSAS, GAGAN, BDSBAS) were in draft/provisional state with `in-vault-synthesis-only` verification status. Comparative pages (WAAS vs EGNOS, MSAS vs GAGAN) lacked source routing to service-provider material. The Standards Source Matrix listed service-provider definition documents as "Not yet represented consistently."

## Research conducted

### WAAS (United States)

- FAA official page: https://www.faa.gov/about/office_org/headquarters_offices/ato/service_units/techops/navservices/gnss/waas
- Scope: "WAAS provides service for all classes of aircraft in all phases of flight"
- Real-time status: https://www.nstb.tc.faa.gov/rt_waassatellitestatus.htm

### EGNOS (Europe)

- EUSPA/ESA official page: https://egnos.gsc-europa.eu/egnos-system/about-egnos
- Scope: "EGNOS is Europe's regional satellite-based augmentation system (SBAS)"
- Safety of Life service declared available for aviation: 2 March 2011

### MSAS (Japan)

- ESA Navipedia: https://gssc.esa.int/navipedia/index.php/MSAS_General_Introduction
- Operating agency: JCAB, Ministry of Land, Infrastructure, Transport and Tourism
- System evolution linked to Michibiki (QZSS) constellation

### GAGAN (India)

- AAI official page: https://www.aai.aero/en/content/what-gagan
- Operating agency: Airports Authority of India (AAI) and Indian Space Research Organisation (ISRO)
- Scope: GPS Aided GEO Augmented Navigation

### BDSBAS (China)

- BeiDou official site: http://en.beidou.gov.cn/SYSTEMS/System/
- Operating agency: China Satellite Navigation Office
- Formerly known as Satellite Navigation Augmentation System (SNAS)

### KASS (South Korea)

- KARI official page: https://www.kari.re.kr/eng/contents/200
- Scope: "KASS utilizes SBAS technology to reduce GPS positioning errors to within three meters"
- Certified by Korean national authorities and declared operational

### SouthPAN (Australia/New Zealand)

- Geoscience Australia official page: https://www.ga.gov.au/scientific-topics/positioning-navigation/positioning-australia/about-the-program/southpan
- Operating agency: Geoscience Australia and Toitu Te Whenua Land Information New Zealand
- Services: L1 SBAS, DFMC SBAS, Precise Point Positioning Via SouthPAN (PVS)

## Files created

1. `Sources/Source - SBAS Service Providers.md` -- NEW institutional source note with official source signals for all 7 SBAS systems, boundary statements, downstream routing, and extraction template

## Files modified

2. `Systems/WAAS.md` -- UPDATED: added source anchors section linking to service-provider source note
3. `Systems/EGNOS.md` -- UPDATED: added source anchors section
4. `Systems/MSAS.md` -- UPDATED: added source anchors section
5. `Systems/GAGAN.md` -- UPDATED: added source anchors section
6. `Systems/BDSBAS.md` -- UPDATED: added source anchors section
7. `Syntheses/WAAS vs EGNOS.md` -- UPDATED: added source anchors and updated next-source-support targets
8. `Syntheses/MSAS vs GAGAN.md` -- UPDATED: modified date
9. `MOCs/SBAS-Systems-by-Region-MOC.md` -- UPDATED: modified date
10. `MOCs/SBAS-Research-MOC.md` -- UPDATED: modified date
11. `Standards-Regulation/SBAS Standards Source Matrix.md` -- UPDATED: added service-provider source note to claim-routing matrix and claim-type matrix
12. `Sources/SBAS Source Backlog.md` -- UPDATED: marked service-provider item as completed; updated suggested execution order

## Boundary decisions

1. **Single consolidated source note**: All 7 SBAS systems covered in one source note (Source - SBAS Service Providers) following the pattern of the FAA/EASA TSO/ETSO and procedure-design source notes.

2. **Verification status**: The new source note uses `public-catalog-reviewed-not-source-extracted` to signal that public catalog metadata supports system identity and operating agency, but direct service-provider document extraction has not been performed.

3. **System pages**: WAAS, EGNOS, MSAS, GAGAN, BDSBAS pages remain in draft/provisional state with `in-vault-synthesis-only` verification status. Source routing has been added but claims are not yet verified.

4. **No KASS or SouthPAN system pages**: These systems are referenced in the service-provider source note but do not have dedicated system pages in the vault. Future cycles could create them if needed for ASEAN/regional analysis.

## Recommended next cycles

1. **Direct extraction of WAAS service definition**: Extract FAA WAAS service scope, coverage, and availability claims.
2. **Direct extraction of EGNOS service definition**: Extract EUSPA/ESA EGNOS service scope, coverage, and availability claims.
3. **Direct extraction of other service-provider documents**: MSAS (JCAB), GAGAN (AAI/ISRO), BDSBAS (BeiDou), KASS (KARI), SouthPAN (GA/LINZ).
4. **Annex 10 direct extraction**: Continue extracting ICAO Annex 10 Volume I GNSS/SBAS technical provisions.
5. **Country/regional source hardening**: Continue ASEAN branch source hardening with verified service-provider data.

## Related notes

- [[SBAS Standards Source Matrix]]
- [[SBAS Source Backlog]]
- [[Source - SBAS Service Providers]]
- [[WAAS]]
- [[EGNOS]]
- [[MSAS]]
- [[GAGAN]]
- [[BDSBAS]]
- [[KASS]]
- [[SouthPAN]]
- [[WAAS vs EGNOS]]
- [[MSAS vs GAGAN]]
- [[SBAS-Systems-by-Region-MOC]]
