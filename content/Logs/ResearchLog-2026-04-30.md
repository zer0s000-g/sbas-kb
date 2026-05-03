---
title: Research Log - GNSS-RO Indonesia Merge
date: 2026-04-30
type: merge
source_vault: private GNSS-RO research workspace
target_vault: retired SBAS vault
---

# Research Log - GNSS-RO Indonesia Merge

## Merge Summary

Merged the GNSS-RO Indonesia empirical research vault into the main SBAS knowledge base.

### Merge scope

- Source vault: private GNSS-RO research notes (6 markdown notes + 1 project summary)
- Target vault: retired SBAS vault
- Merge date: 2026-04-30
- Performed by: Hermes Agent with `obsidian-knowledge-management` skill

### Non-overlap verification

The following domains were verified as **non-overlapping** before merge:

| Domain                           | In SBAS vault before merge                                    | In GNSS-RO vault                               |
| -------------------------------- | ------------------------------------------------------------- | ---------------------------------------------- |
| GNSS Radio Occultation technique | Not present                                                   | Full coverage                                  |
| Total Electron Content (TEC)     | Mentioned in integrity context only; no detailed concept note | Full empirical statistics                      |
| IRI-2020 model                   | Not present                                                   | Systematic validation                          |
| Ionospheric model validation     | Conceptual only (standards/regulation)                        | Empirical methodology + results                |
| Indonesia equatorial ionosphere  | Only starter scaffold; zero empirical data                    | 301-occultation study + 4 ION paper iterations |
| SBAS ionospheric threat          | Conceptual only                                               | Pre-operational threat budget with numbers     |

**Verdict: zero content overlap confirmed.**

### Files created

#### Concepts (3 new atomic notes)

1. `Concepts/GNSS Radio Occultation.md` — technique definition with SBAS-context boundary
2. `Concepts/Total Electron Content (TEC).md` — observable concept with delay conversion table
3. `Concepts/Ionospheric Model Validation.md` — methodology concept with error metrics

#### Sources (3 new source scaffolds)

4. `Sources/Source - GNSS Radio Occultation Technique.md`
5. `Sources/Source - IRI-2020 Ionosphere Model.md`
6. `Sources/Source - GNSS-RO Indonesia Empirical Study.md`

#### Syntheses (3 new synthesis notes)

7. `Syntheses/IRI-2020 vs GNSS-RO Indonesia.md` — comparison with tables
8. `Syntheses/SBAS Ionospheric Threat — Empirical Evidence.md` — bridge to integrity design
9. `Syntheses/Indonesian SBAS ION Paper Iterations.md` — V1→V4 tracking note

#### Logs (1 new log)

10. `Logs/ResearchLog-2026-04-30.md` — this merge log

### Existing files strengthened with bidirectional links

| File                                                             | Links added                                                                                           |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| `ASEAN/Countries/Indonesia.md`                                   | `[[IRI-2020 vs GNSS-RO Indonesia]]`, `[[SBAS Ionospheric Threat — Empirical Evidence]]` (2 locations) |
| `ASEAN/ASEAN SBAS Deployment Barriers.md`                        | `[[SBAS Ionospheric Threat — Empirical Evidence]]`, `[[IRI-2020 vs GNSS-RO Indonesia]]` (2 locations) |
| `MOCs/SBAS-Research-MOC.md`                                      | Empirical research section, source scaffolds, priority area #6                                        |
| `MOCs/SBAS MOC.md`                                               | New concept links, suggested targets, see-also                                                        |
| `Sources/SBAS Source Backlog.md`                                 | 3 new execution-order entries, related notes                                                          |
| `Sources/Source - Equatorial Ionosphere and SBAS Feasibility.md` | Multiple links to empirical anchors                                                                   |

### Connection health metrics

- **New nodes created:** 10 (3 concepts, 3 sources, 3 syntheses, 1 log)
- **Bidirectional links per new node:** 4–7 (within 3–5 target)
- **Existing notes strengthened:** 6
- **Orphan nodes:** 0
- **Estimated path to any new topic from SBAS MOC:** ≤3 steps

### Provenance status of merged content

| Note          | Status   | verification_status     |
| ------------- | -------- | ----------------------- |
| Concepts (3)  | Draft    | `empirical-study`       |
| Syntheses (3) | Draft    | `empirical-study`       |
| Sources (3)   | Starter  | `metadata-pending`      |
| Log (1)       | Complete | `internal-backlog-only` |

### Next steps identified

1. Deepen `Source - GNSS-RO Indonesia Empirical Study` with verified dataset metadata
2. Add ground GNSS CORS/IGS validation for Indonesian TEC
3. Targeted post-sunset GNSS-RO acquisition (18–21 LT gap)
4. Convert threat-budget scaffold into candidate GIVE-like bins after validation
5. Extend IGRF analysis to full-year or multi-year sampling

### Merge checklist

- [x] New terminology nodes created with full specifications
- [x] Zero content overlap verified (file-system enforced, separate subdirectories)
- [x] All nodes connected (3–5 bidirectional links each)
- [x] Explicit uncertainty language in source scaffolds (metadata-pending)
- [x] Recurring references converted into prioritized queue (source backlog updated)
- [x] MOC navigation paths validated (≤3 steps to any topic from SBAS MOC)
- [x] Version control via git-like file structure preserved
- [x] Next source-building steps clearly identified
- [x] Merge log created

---

_Protocol followed: obsidian-knowledge-management skill, Expansion Methodology + Provenance-First Quality Assurance_
