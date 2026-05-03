---
title: Institutional SBAS Knowledge Base Upgrade Roadmap
description: Roadmap for turning the SBAS Quartz site into an institutional-grade public reference
labels: [sbas, governance, roadmap, institutional-grade]
tags: [sbas, governance, roadmap, institutional-grade]
created: 2026-05-01
modified: 2026-05-01
status: active
verification_status: editorial-control
---

# Institutional SBAS Knowledge Base Upgrade Roadmap

## Mission

Upgrade this SBAS knowledge base from a useful research vault into a reference-grade public site that can shorten the learning curve for agencies, universities, ANSPs, researchers, and implementation teams.

The target audience includes readers who expect traceable, standards-aware, technically cautious material comparable in seriousness to institutional material from aerospace agencies, universities, regulators, and system operators.

## Current baseline

The current vault is structurally strong, but still uneven in maturity.

| Metric                                      | Current value |
| ------------------------------------------- | ------------: |
| Markdown notes audited                      |            97 |
| Institutional candidates                    |            36 |
| Reviewed candidates                         |            36 |
| Upgrade needed                              |            20 |
| Scaffolds                                   |             5 |
| Notes still marked draft                    |            62 |
| Notes missing explicit status               |            14 |
| Files with broken wikilinks detected        |            22 |
| Total broken wikilinks detected             |            73 |
| Local/private path issues after latest scan |             0 |

## Upgrade principle

Do not add large amounts of generic SBAS text first. First convert the knowledge base into a governed reference system:

1. clear learning paths
2. mature pillar pages
3. standards-linked source backbone
4. comparison matrices
5. implementation playbooks
6. diagrams and decision flows
7. explicit caveats for synthesis and research claims

## Phase 1 — Institutional audit and governance

Status: started.

Deliverables:

- [[Institutional Upgrade Audit 2026-05-01]]
- [[SBAS Knowledge Base Editorial and Source Policy]]
- link audit and maturity scoring
- upgrade queue for pillar pages and weak notes

Success criteria:

- every note has a known maturity state
- weak pages are visible as a backlog
- publication rules prevent private/local paths and unsupported claims

## Phase 2 — Core SBAS pillar pages

Create or upgrade the following as polished `living-standard` or `institutional` pages:

| Pillar                                 | Purpose                                                   | Initial target                                            |
| -------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| What is SBAS?                          | Beginner landing page                                     | Upgrade [[SBAS-Terminology]] or create a dedicated pillar |
| SBAS Architecture                      | System-level explanation                                  | Create new architecture pillar                            |
| SBAS Integrity                         | Explain integrity risk, monitors, and operational meaning | Upgrade [[SBAS Integrity]]                                |
| Protection Levels and Alert Limits     | Bridge equations, safety, and pilot/operation meaning     | Upgrade [[Protection Levels]] and [[Alert Limits]]        |
| SBAS Ionospheric Corrections           | Explain IGP, GIVE, delay, gradients, low-latitude risk    | Create or upgrade ionosphere pillar                       |
| SBAS Signal-in-Space and Message Types | Explain broadcast content and user processing             | Create new pillar                                         |
| SBAS Ground Segment                    | Reference stations, master stations, uplink, monitoring   | Create new pillar                                         |
| SBAS in Aviation Operations            | LPV/APV/RNP/PBN operational context                       | Upgrade aviation notes                                    |
| SBAS Standards and Certification       | ICAO/RTCA/EUROCAE/FAA/EASA/EUSPA map                      | Upgrade standards notes                                   |
| Global SBAS Systems Comparison         | WAAS/EGNOS/MSAS/GAGAN/KASS/BDSBAS/etc.                    | Upgrade systems branch                                    |

## Phase 3 — Standards and certification backbone

Priority source families:

- ICAO GNSS, PBN, Annex 10, APANPIRG, and regional implementation material
- RTCA/EUROCAE MOPS and interface/control documents
- FAA WAAS performance and certification material
- EGNOS service definition, performance, and EUSPA/ESA material
- MSAS, GAGAN, KASS, BDSBAS, SouthPAN, ASECNA, and other regional operator material
- Stanford GPS Lab and high-quality SBAS integrity literature

Each source note should support specific downstream claims, not just exist as a bibliography entry.

## Phase 4 — Learning paths

Create reader-specific paths:

- Beginner path: learn SBAS from zero
- Engineer path: evaluate or design SBAS service elements
- Regulator/ANSP path: certification, PBN, LPV, safety case, and rollout
- Researcher path: integrity, ionosphere, DFMC, ARAIM, and open problems
- ASEAN implementation path: readiness, governance, service model, testbed, and transition to operation

## Phase 5 — Implementation playbooks

Create procedural pages for real-world use:

- SBAS readiness assessment playbook
- LPV airport candidate assessment playbook
- Regional SBAS testbed design playbook
- SBAS performance monitoring playbook
- Ionospheric threat assessment playbook
- Regulatory and institutional roadmap playbook
- Testbed-to-operational-service transition playbook

## Phase 6 — Research-frontier branch

Build a research map for advanced users:

- DFMC SBAS
- ARAIM and SBAS relationship
- low-latitude ionospheric threat models
- plasma bubbles and post-sunset coverage gaps
- GNSS-RO for threat discovery
- RFI/spoofing resilience
- LEO-PNT interactions
- non-aviation SBAS applications

## Immediate execution queue

1. Repair broken wikilinks in homepage and core MOCs.
2. Add missing frontmatter status and verification fields to older core pages.
3. Upgrade [[SBAS-Terminology]] into a true beginner gateway or split it into a separate future `What is SBAS?` pillar.
4. Upgrade aviation operation notes with standards anchors.
5. Build the global SBAS systems comparison matrix.
6. Create the SBAS architecture pillar and diagram.
7. Upgrade [[SBAS Integrity]], [[Protection Levels]], and [[Alert Limits]] as a connected integrity learning path.
8. Create institutional source notes for the highest-value official standards and system documents.

## See also

- [[SBAS Knowledge Base Editorial and Source Policy]]
- [[Institutional Upgrade Audit 2026-05-01]]
- [[SBAS MOC]]
- [[SBAS-Systems-by-Region-MOC]]
- [[SBAS Source Backlog]]
