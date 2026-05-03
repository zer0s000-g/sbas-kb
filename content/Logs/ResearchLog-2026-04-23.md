# Research Log - 2026-04-23

## Cycle

- Time: 2026-04-23 08:30 WIB
- Classification: review, retrieval, MOC maintenance
- Focus: initialize top-level SBAS navigation and identify provenance gaps

## What changed

- Created [[SBAS MOC]] as the new top-level navigation note for SBAS work.
- Updated [[SBAS Research MOC]] with an initialization review and explicit provenance warning.
- Updated [[SBAS in Civil Aviation MOC]] with an initialization review and next-step guidance.

## Files touched

- MOCs/SBAS MOC.md
- MOCs/SBAS-Research-MOC.md
- MOCs/SBAS-in-Civil-Aviation-MOC.md

## Sourced vs synthesized vs uncertain

- Sourced this cycle: none added; this was a structure-and-provenance review cycle.
- Synthesized this cycle: assessment that the vault has promising structure but weak source-note coverage.
- Flagged as uncertain/provisional: unsourced quantitative performance figures, standards scope statements, and cross-region interoperability claims in existing draft notes.

## Links added

- [[SBAS MOC]] -> [[SBAS Research MOC]]
- [[SBAS MOC]] -> [[SBAS in Civil Aviation MOC]]
- [[SBAS MOC]] -> [[SBAS-Systems-by-Region-MOC]]
- [[SBAS Research MOC]] -> [[SBAS MOC]]
- [[SBAS in Civil Aviation MOC]] -> [[SBAS MOC]]

## Next best research question

Which foundational source note should be built first to stabilize the vault: an ICAO SBAS standards note, an RTCA airborne SBAS note, or an atomic concept note on [[SBAS Integrity]] and [[Protection Levels]]?

## Follow-on cycle — 2026-04-23 08:33 WIB

- Classification: provenance management, retrieval, source backlog creation
- Improvement: created [[SBAS Source Backlog]] to convert recurring standards references into an explicit verification queue.
- Why this was chosen: the vault repeatedly cites ICAO/RTCA/EUROCAE documents without dedicated source notes, making many technical and regulatory claims hard to audit.
- New recommendation: build [[Source - RTCA DO-229]] first, then use it to clean up airborne-equipment and operational-approval claims across the vault.

## Follow-on cycle — 2026-04-23 09:18 WIB

- Classification: Asia-Pacific comparison expansion, regional broadening, retrieval strengthening
- Improvement 1: created [[MSAS vs GAGAN]] as the first Asia-focused regional comparison note using in-vault references only.
- Improvement 2: created [[BDSBAS]] to extend Asia coverage beyond Japan and India into a China/BeiDou-centered regional context.
- Improvement 3: updated [[SBAS-Systems-by-Region-MOC]], [[SBAS MOC]], and [[SBAS-vs-Other-Augmentation-Methods]] to surface the stronger Asia comparison layer.
- Result: the vault now has an Asia-focused regional comparison path spanning [[MSAS]], [[GAGAN]], and [[BDSBAS]], plus a dedicated [[MSAS vs GAGAN]] comparison note.

## Follow-on cycle — 2026-04-23 14:30 WIB

- Classification: regional expansion, non-overlapping branch creation, retrieval strengthening
- Focus: expand the vault into the missing ASEAN SBAS implementation layer without repeating generic SBAS basics already covered elsewhere.
- New notes created:
  - [[ASEAN SBAS Adoption Landscape]]
  - [[ASEAN SBAS Readiness Heuristic]]
  - [[ASEAN SBAS Operational Demand Drivers]]
  - [[ASEAN SBAS Deployment Barriers]]
  - [[ASEAN SBAS Governance and Institutional Actors]]
  - [[ASEAN SBAS Service-Model Options]]
- Navigation updated in:
  - [[SBAS MOC]]
  - [[SBAS-Research-MOC]]
  - [[SBAS-Systems-by-Region-MOC]]
  - [[SBAS in Civil Aviation MOC]]
  - [[Asia-Pacific SBAS Implementation Patterns]]
- Sourced this cycle: limited external scouting signals for ICAO APAC SBAS/GBAS implementation forums, ASEAN member-state scope, and country-context proxies used only for readiness heuristics.
- Synthesized this cycle: the ASEAN branch is best treated as an adoption/governance/readiness problem rather than as an already-deployed regional system note.
- Flagged as uncertain/provisional: country-by-country implementation status, formal ASEAN-level SBAS program ownership, and any claim that a specific service-model path has already been chosen.
- Result: the vault now has a dedicated Southeast Asia expansion layer that is structurally separated from generic standards, system overviews, and broad Asia-Pacific synthesis.

## Next best research question

Which ASEAN-facing source stack should be built first: ICAO APAC regional meeting/source notes, country-level PBN readiness notes, or an equatorial-ionosphere evidence note for Southeast Asian SBAS feasibility?

## Follow-on cycle — 2026-04-23 14:48 WIB

- Classification: regional continuation, country-layer expansion, retrieval strengthening
- Focus: extend the ASEAN branch downward from heuristic grouping into dedicated country child notes without duplicating ASEAN-wide demand, barrier, governance, or service-model notes.
- New notes created under `ASEAN/Countries/`:
  - [[Indonesia]]
  - [[Philippines]]
  - [[Singapore]]
  - [[Malaysia]]
  - [[Thailand]]
  - [[Viet Nam]]
  - [[Lao PDR]]
  - [[Cambodia]]
  - [[Myanmar]]
  - [[Brunei Darussalam]]
- Navigation updated in:
  - [[ASEAN SBAS Readiness Heuristic]]
  - [[ASEAN SBAS Adoption Landscape]]
  - [[SBAS MOC]]
  - [[SBAS-Research-MOC]]
- Sourced this cycle: none newly extracted into dedicated source notes; this was a structural expansion cycle built on the prior ASEAN heuristic layer.
- Synthesized this cycle: each country now has a distinct child role in the ASEAN storyline, separated into archipelagic demand anchors, hub/connector states, lower-readiness mainland beneficiaries, and a compact fast-follower case.
- Flagged as uncertain/provisional: country-level implementation posture, PBN maturity details, and any implicit ranking beyond the heuristic roles already stated.
- Result: the ASEAN branch now has a full country-note layer, making it possible to continue next into source-backed national evidence without rewriting the regional notes.

## Follow-on cycle — 2026-04-23 14:56 WIB

- Classification: provenance continuation, ASEAN source-layer creation, governance verification support
- Focus: add an ASEAN-specific source backbone so the new regional and country notes can later be tightened against identifiable source stacks.
- New notes created:
  - [[ASEAN SBAS Source Backlog]]
  - [[Source - ICAO APAC GBAS-SBAS Implementation Forums]]
- Notes updated to surface the source layer:
  - [[ASEAN SBAS Adoption Landscape]]
  - [[ASEAN SBAS Governance and Institutional Actors]]
  - [[SBAS Source Backlog]]
- Sourced this cycle: no direct quote extraction yet; created provenance scaffolds based on the previously identified ICAO APAC meeting/forum trail.
- Synthesized this cycle: the most valuable first ASEAN-facing source stack is the ICAO APAC forum layer because it bears directly on the current governance hypothesis.
- Flagged as uncertain/provisional: exact meeting metadata, the degree of ASEAN-specific participation, and whether APANPIRG/CNS material supports implementation planning versus only broad coordination.
- Result: the ASEAN branch now has both a thematic layer and an explicit provenance queue, which is the right base for future source-backed country or governance upgrades.

## Follow-on cycle — 2026-04-23 15:04 WIB

- Classification: provenance continuation, source-stack expansion, barrier/governance support
- Focus: expand the ASEAN provenance layer beyond the first ICAO APAC forum scaffold into adjacent regional planning and technical-feasibility source stacks.
- New notes created:
  - [[Source - APANPIRG and CNS SG SBAS References]]
  - [[Source - Equatorial Ionosphere and SBAS Feasibility]]
- Notes updated to surface the new source layer:
  - [[ASEAN SBAS Deployment Barriers]]
  - [[ASEAN SBAS Governance and Institutional Actors]]
  - [[ASEAN SBAS Source Backlog]]
- Sourced this cycle: no direct extraction yet; created two additional provenance scaffolds to distinguish governance-source support from technical-feasibility support.
- Synthesized this cycle: the ASEAN branch now separates three evidence lanes clearly — ICAO APAC implementation forums, APANPIRG/CNS regional planning references, and equatorial-ionosphere feasibility evidence.
- Flagged as uncertain/provisional: exact documentary support for APANPIRG/CNS SBAS planning language, and any technical conclusion about what equatorial conditions do or do not allow in Southeast Asian SBAS service design.
- Result: the provenance layer is now deep enough to support a future source-backed tightening pass without collapsing back into generic ASEAN synthesis.

## Follow-on cycle — 2026-04-23 15:12 WIB

- Classification: provenance continuation, country-readiness support, archipelagic-demand support
- Focus: extend the ASEAN source layer into the first two scaffolds needed to upgrade country notes from heuristic placeholders toward evidence-backed differentiation.
- New notes created:
  - [[Source - ASEAN Country PBN Readiness Signals]]
  - [[Source - Archipelagic Airport Network Context in ASEAN]]
- Notes updated to surface the new source layer:
  - [[ASEAN SBAS Readiness Heuristic]]
  - [[Indonesia]]
  - [[Philippines]]
  - [[ASEAN SBAS Source Backlog]]
- Sourced this cycle: no direct extraction yet; created source scaffolds that separate country-readiness evidence from archipelagic-demand evidence.
- Synthesized this cycle: the country branch can now be tightened along two distinct axes rather than one blended heuristic — readiness signals and airport-network/access context.
- Flagged as uncertain/provisional: any claim that archipelagic demand implies early implementation, and any ranking of ASEAN states by readiness before country-specific documents are extracted.
- Result: the ASEAN branch now has enough provenance structure to support the next real evidence pass on [[Indonesia]], [[Philippines]], [[Singapore]], and [[ASEAN SBAS Readiness Heuristic]].

## Follow-on cycle — 2026-04-23 15:26 WIB

- Classification: evidence-tightening, country-readiness refinement, cautious claim narrowing
- Focus: use live institutional findings to tighten the highest-value ASEAN country notes without overstating unsupported conclusions.
- Live evidence incorporated this cycle:
  - CAAS website signals for [[Singapore]], including visible AIM-system support and current regulator planning/publication documents.
  - World Bank country-page support for [[Indonesia]] as an archipelagic case, including wording that the country is made up of over 17,000 islands.
  - a negative finding for [[Philippines]]: the source path was reached, but no equally clean institutional archipelagic sentence was extracted during this cycle.
- Notes updated:
  - [[Source - ASEAN Country PBN Readiness Signals]]
  - [[Source - Archipelagic Airport Network Context in ASEAN]]
  - [[Singapore]]
  - [[Indonesia]]
  - [[Philippines]]
  - [[ASEAN SBAS Readiness Heuristic]]
- Sourced this cycle: limited but real live evidence, used only where the source support was clear enough.
- Synthesized this cycle: the first country-tightening pass now differentiates between claims supported by direct institutional signals and claims that remain heuristic placeholders.
- Flagged as uncertain/provisional: direct PBN depth for Singapore, airport-network metrics for Indonesia, and an institutional archipelagic citation strong enough to tighten the Philippines note beyond its current wording.
- Result: the ASEAN branch now contains its first evidence-aware country refinements rather than only source scaffolds and heuristics.

## Five-cycle continuation block — 2026-04-23 15:40 WIB

- Classification: multi-cycle continuation, evidence tightening, country-readiness refinement, provenance synchronization
- Scope: continue autonomously for five successive ASEAN-focused cycles without stopping.

### Cycle 1

- Attempted deeper extraction from Singapore CAAS-linked PDFs and recorded a precise limit: direct PDF text extraction remains incomplete in the current environment.
- Preserved the stronger live evidence already available from the CAAS site itself rather than over-claiming from unread PDFs.

### Cycle 2

- Added live Malaysia readiness evidence through official CAAM pages.
- Usable support captured for:
  - national/state safety-planning structures
  - AIS/AIP/AIRAC publication capability
  - visible official PBN circular links

### Cycle 3

- Added live Thailand readiness evidence through ICAO APAC PBN progress-report paths and a visible CAAT PBN guidance-material path.
- Tightened Thailand only to the level of documented PBN-modernization activity, not SBAS adoption.

### Cycle 4

- Improved the Philippines evidence base through CAAP references to "CAAP-operated airports" and "all CAAP-operated airports," strengthening the distributed-airport context.
- Updated the Philippines note to reflect improved network-context support while keeping the archipelagic-demand claim cautious.

### Cycle 5

- Synchronized the branch by updating:
  - [[Source - ASEAN Country PBN Readiness Signals]]
  - [[Source - Archipelagic Airport Network Context in ASEAN]]
  - [[Singapore]]
  - [[Indonesia]]
  - [[Philippines]]
  - [[Malaysia]]
  - [[Thailand]]
  - [[ASEAN SBAS Readiness Heuristic]]
  - [[ASEAN SBAS Adoption Landscape]]
  - [[ASEAN SBAS Source Backlog]]
  - [[SBAS-Research-MOC]]
- Result: the ASEAN branch now has a broader first-generation evidence-backed country layer spanning five states.

- Sourced in this five-cycle block:
  - CAAS website institutional signals for Singapore
  - World Bank Indonesia country-page archipelagic wording
  - CAAP distributed-airport context wording for the Philippines
  - CAAM pages and PBN-related document paths for Malaysia
  - ICAO APAC / CAAT source paths for Thailand PBN progress and guidance material
- Synthesized in this five-cycle block:
  - readiness and demand are now being separated more cleanly by evidence type rather than by intuition alone
  - some countries are better supported on institutional readiness, others on distributed-network demand
- Flagged as uncertain/provisional:
  - direct SBAS adoption claims for all five countries
  - exact PBN implementation depth or procedure counts where underlying PDFs were not directly extracted
  - a stronger official archipelagic citation for the Philippines beyond the current CAAP-operated-airports context
- Result: the vault has now moved from ASEAN branch creation into sustained evidence-aware refinement.

## Three-cycle continuation block — 2026-04-23 15:55 WIB

- Classification: multi-cycle continuation, targeted evidence tightening, branch synchronization
- Scope: continue autonomously for three successive ASEAN-focused cycles without stopping.

### Cycle 1

- Strengthened the Philippines evidence base beyond generic CAAP-operated-airports wording.
- Added a stronger live CAAP signal supporting 44 commercially operating airports under CAAP and 48 commercially operated airports nationwide.
- Tightened the Philippines note toward a nationwide commercial-airport-network framing while keeping the broader archipelagic-demand claim cautious.

### Cycle 2

- Consolidated Malaysia and Thailand as evidence-aware readiness cases.
- Malaysia remains supported by CAAM governance, AIS/AIP/AIRAC, and PBN circular signals.
- Thailand remains supported by ICAO APAC PBN implementation-reporting paths and visible CAAT PBN guidance material.
- Chose not to over-claim beyond those live source paths.

### Cycle 3

- Synchronized the branch by updating:
  - [[Source - Archipelagic Airport Network Context in ASEAN]]
  - [[Philippines]]
  - [[ASEAN SBAS Readiness Heuristic]]
  - [[ASEAN SBAS Adoption Landscape]]
  - [[ASEAN SBAS Source Backlog]]
  - [[SBAS-Research-MOC]]
- Result: the branch now distinguishes more clearly between evidence-backed readiness states and evidence-backed distributed-network demand states.

- Sourced in this three-cycle block:
  - CAAP commercial-airport-network wording for the Philippines
  - previously captured CAAM and ICAO APAC / CAAT evidence retained and synchronized rather than re-expanded
- Synthesized in this three-cycle block:
  - the Philippines is now better supported as a distributed commercial-airport-network case
  - the branch's strongest current early split is now explicit: institutional-readiness signals for [[Singapore]], [[Malaysia]], and [[Thailand]] versus distributed-network demand/context signals for [[Indonesia]] and [[Philippines]]
- Flagged as uncertain/provisional:
  - direct SBAS adoption claims for all five countries remain unsupported
  - Philippines still needs a cleaner official archipelagic citation beyond the current airport-network evidence
  - Malaysia and Thailand still need deeper primary-text extraction before stronger PBN-detail claims are made
- Result: the ASEAN knowledge base is now materially more evidence-shaped and less heuristic than before this three-cycle block.
