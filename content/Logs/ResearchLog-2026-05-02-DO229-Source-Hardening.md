---
title: Research Log - 2026-05-02 DO-229 Source Hardening
description: Work log documenting the RTCA DO-229 public-product and regulator-signal hardening cycle for the SBAS knowledge base
tags: [research-log, source-hardening, rtca, do-229, sbas, mops, qa]
created: 2026-05-02
modified: 2026-05-02
status: complete
verification_status: work-log
---

# Research Log - 2026-05-02 DO-229 Source Hardening

## Scope

This cycle strengthened the SBAS knowledge base's handling of [[Source - RTCA DO-229]] as the airborne GPS/SBAS equipment MOPS source-family anchor.

The objective was not to reproduce or paraphrase the proprietary RTCA standard. The objective was to use publicly visible institutional signals to tighten source routing, approval boundaries, and downstream documentation discipline.

## Public signals reviewed

| Source family              | Public signal used                                                                                               | Editorial implication                                                                         |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| RTCA product metadata      | DO-229F product page identifies GPS/SBAS airborne-equipment MOPS, issue date, SC-159, and single-frequency scope | DO-229 is the receiver/equipment MOPS source family; it is not a DFMC source by default       |
| RTCA product metadata      | DO-229E product page identifies revision lineage and public summary of selected changes                          | Revision baseline matters; public summaries are not detailed requirements                     |
| Standards catalog metadata | DO-229 public catalog page identifies active/current 2020 item and broad scope                                   | Supports source-family routing, not detailed requirement extraction                           |
| FAA TSO overview           | FAA explains TSOA as design/production approval and explicitly separates it from installation approval           | TSO/DO-229 evidence does not equal aircraft installation or operational approval              |
| EASA ETSO material         | Public ETSO-C145e/C146e material references DO-229E Section 2 and regulator-specific modifications               | DO-229 participates in approval frameworks, but jurisdiction-specific source notes are needed |
| ESA Navipedia              | Secondary orientation on SBAS standards split between ICAO SARPs and DO-229 receiver equipment                   | Useful for orientation only; not treated as primary authority                                 |

## Files changed

- [[Source - RTCA DO-229]] was rewritten as a stricter institutional source note.
- [[SBAS Standards Source Matrix]] was updated to distinguish DO-229 equipment routing from installation, operational, service, procedure, and DFMC claims.
- [[SBAS Source Backlog]] was updated so the next DO-229 task is official-text extraction plus FAA/EASA TSO/ETSO source-note creation.
- [[SBAS-Standards-Regulation]] was tightened around equipment standards versus approval context.
- [[SBAS Integrity]], [[Protection Levels]], and [[Alert Limits]] now describe DO-229 as a receiver/equipment source-family anchor, not a free-standing source for operational values.
- [[LPV-Approach-Procedure]] now separates DO-229 equipment support from LPV procedure availability, installation approval, operational approval, and service status.
- [[SBAS-vs-Other-Augmentation-Methods]], [[SBAS-vs-Other-Standards]], [[SBAS in Civil Aviation MOC]], [[SBAS MOC]], and [[SBAS-Research-MOC]] were updated to preserve the new source split.

## Documentation-quality decisions

1. No operational numerical values were added.
2. No LPV minima, alert limits, time-to-alert values, accuracy values, continuity values, or availability values were introduced.
3. DO-229 was kept in the receiver/equipment lane.
4. FAA/EASA material was used only to separate TSO/ETSO article approval from aircraft installation and operational approval.
5. DFMC was explicitly treated as outside the current DO-229 source support unless a dedicated source note is created.
6. The KB now distinguishes five layers that are often conflated:
   - DO-229 receiver/equipment MOPS;
   - FAA/EASA TSO/ETSO article approval frameworks;
   - aircraft installation approval;
   - procedure design and publication;
   - operational approval and real-time service availability.

## QA checklist

- Quartz build: pending in this cycle until final QA step.
- Formatting: pending in this cycle until final QA step.
- Wikilink audit: pending in this cycle until final QA step.
- Publication/privacy audit: pending in this cycle until final QA step.
- Deployment verification: pending in this cycle until final publish step.

## Recommended next cycle

Create dedicated source notes for FAA TSO-C145/C146 and EASA ETSO-C145/C146 so that DO-229 equipment claims can be separated cleanly from jurisdiction-specific article approval, installation approval, and aircraft/operator use.

Do not expand LPV operational values until the procedure-design and AIP/AIS source families are in place.
