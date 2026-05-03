---
title: SBAS Knowledge Base Editorial and Source Policy
description: Editorial rules for converting the SBAS Quartz knowledge base into an institutional-grade public reference
labels: [sbas, governance, editorial-policy, source-policy, quartz]
tags: [sbas, governance, editorial-policy, source-policy, quartz]
created: 2026-05-01
modified: 2026-05-01
status: active
verification_status: editorial-control
---

# SBAS Knowledge Base Editorial and Source Policy

## Purpose

This policy governs how the SBAS knowledge base is expanded into an institutional-grade public reference for engineers, researchers, regulators, ANSPs, universities, and implementation teams.

The knowledge base should shorten the learning curve for SBAS without presenting draft synthesis as certified operational guidance.

## Non-negotiable publication rules

- Do not publish local filesystem paths, machine names, private folder names, credentials, tokens, or private source locations.
- Use neutral provenance labels such as "GIPTA source document collection" or "private research archive" when a source is not publicly linkable.
- Prefer official public URLs, document titles, issuing institutions, revision identifiers, and publication dates over private-file references.
- Do not claim operational certification, safety approval, service availability, or standards compliance unless an authoritative source explicitly supports it.
- Separate verified facts, synthesis, implementation interpretation, and open questions.
- Keep all frontmatter valid YAML wrapped by `---` delimiters.

## Maturity labels

| Status            | Meaning                                                 | Publication handling                         |
| ----------------- | ------------------------------------------------------- | -------------------------------------------- |
| `seed`            | Placeholder or early stub                               | Keep out of core navigation unless necessary |
| `draft`           | Useful but not fully verified                           | Allow, but show caveats and source gaps      |
| `reviewed`        | Checked against specific source anchors                 | Suitable for normal public navigation        |
| `institutional`   | Polished reference-grade page with clear source support | Promote in learning paths and MOCs           |
| `living-standard` | Core maintained page requiring periodic review          | Use for primary pillar pages                 |

## Verification labels

| Label                        | Use when                                                                                    |
| ---------------------------- | ------------------------------------------------------------------------------------------- |
| `source-scaffold-linked`     | The note is tied to one or more source notes but still needs deeper verification            |
| `official-source-verified`   | The central claims are checked against official institutional material                      |
| `standards-linked`           | The note is anchored in ICAO, RTCA, EUROCAE, FAA, EASA, EUSPA, ANSP, or regulator documents |
| `research-literature-linked` | The note is anchored in peer-reviewed or recognized technical research                      |
| `synthesis-with-caveats`     | The note interprets multiple sources and must preserve uncertainty                          |
| `implementation-playbook`    | The note is procedural guidance, not certification material                                 |
| `editorial-control`          | The note defines site governance or editorial process                                       |

## Institutional page template

Use this structure for pillar pages and implementation playbooks:

1. Scope and reader profile
2. Executive summary
3. Core concept or operational problem
4. Architecture, process, or technical mechanism
5. Standards and source anchors
6. Operational implications
7. Common misunderstandings
8. Implementation or research relevance
9. Boundaries and caveats
10. See also

## Source-note minimum fields

Every serious source note should include:

- document title
- issuing institution
- source type
- version or date where known
- public URL where available
- scope of the source
- supported claims
- unsupported or ambiguous claims
- downstream notes that rely on it
- related standards, systems, or regions

## Claim discipline

| Claim type             | Required support                                                                                          |
| ---------------------- | --------------------------------------------------------------------------------------------------------- |
| Definition             | Authoritative standard, system documentation, or clearly marked synthesis                                 |
| Performance number     | Official performance report, standard, paper, or reproducible analysis                                    |
| Certification/approval | Regulator, ANSP, service provider, or official safety documentation                                       |
| Regional readiness     | Visible evidence such as AIP/AIS/PBN, CNS plans, institutional statements, or documented testbed activity |
| Research frontier      | Research literature or explicitly marked open question                                                    |

## Quartz quality gates

Before pushing publication changes:

- run a local Quartz build
- scan Markdown content for private/local path patterns
- scan generated public output for private/local path patterns
- check frontmatter delimiters
- check new wikilinks
- check that new institutional pages link to at least three relevant existing notes

## See also

- [[Institutional SBAS Knowledge Base Upgrade Roadmap]]
- [[Institutional Upgrade Audit 2026-05-01]]
- [[SBAS MOC]]
- [[SBAS Source Backlog]]
