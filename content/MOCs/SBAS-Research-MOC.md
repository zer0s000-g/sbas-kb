---
title: SBAS Research MOC
description: Top-level map of SBAS research knowledge base for civil aviation applications
tags: [MOC, research, sbas, navigation, aviation]
category: mocs
created: 2026-04-19
modified: 2026-05-01
version: 1.0
status: research
---

# 🗺️ SBAS Research Map of Consciousness

## Initialization review — 2026-04-23
- Parent navigation: [[SBAS MOC]]
- Current structure is useful for navigation, but much of the content is still draft synthesis rather than source-grounded research.
- Priority improvement area: create dedicated source notes before treating quantitative performance claims or standards mappings as settled.
- Use this MOC to navigate work-in-progress research, not as a standalone authority.

## 📊 **Research Portfolio Overview**

### **Knowledge Domains**
```
SBAS FUNDAMENTALS
    ├── GNSS Error Sources
    │   ├── Ionospheric Delay
    │   ├── Tropospheric Delay
    │   ├── Ephemeris Errors
    │   └── Receiver Noise
    ├── SBAS Architecture
    │   ├── Space Segment (GEO Satellites)
    │   ├── Ground Segment (Reference Stations)
    └── User Segment (Receivers)

CIVIL AVIATION APPLICATIONS
    ├── Approach Procedures
    │   ├── LPV (Localizer Performance with Vertical)
    │   ├── APV (Approach with Vertical Guidance)
    │   ├── LNAV/VNAV
    │   └── RNAV (GNSS) Approaches
    ├── Terminal Operations
    ├── En-Route Operations
    └── Oceanic/Remote Operations

REGIONAL SYSTEMS
    ├── WAAS (Wide Area Augmentation System)
    ├── EGNOS (European Geostationary Navigation Overlay Service)
    ├── MSAS (Multi-functional Satellite Augmentation System)
    ├── GAGAN (GPS Aided Geo Augmented Navigation)
    ├── BDSBAS (BeiDou Satellite-Based Augmentation System)
    ├── Other National Systems
    └── ASEAN implementation branch

COMPARATIVE ANALYSIS
    ├── SBAS vs GBAS
    ├── SBAS vs ABAS
    ├── SBAS vs RAIM
    └── ARAIM (Advanced RAIM)

STANDARDS & CERTIFICATION
    ├── ICAO SARPs (Doc 8083, 7084, 9854, 9855)
    ├── RTCA (DO-229, DO-242, DO-289)
    ├── EUROCAE (ED-52, ED-102, ED-142)
    └── National Regulations

INTEGRITY & SAFETY
    ├── Protection Levels
    ├── Alert Limits
    ├── Fault Detection
    └── Risk Assessment
```

## 🔬 **Research Methodology**

### **Evidence Hierarchy**
1. **Primary Sources**: ICAO docs, RTCA standards, EUROCAE specs
2. **Technical Literature**: IEEE papers, aviation journals
3. **Implementation Reports**: Operational system documentation
4. **Empirical Data**: Flight test results, performance monitoring

### **Knowledge Quality Levels**
- **Level 1**: Verified standards (direct quotes from docs)
- **Level 2**: Implementation evidence (test reports, operational data)
- **Level 3**: Expert synthesis (multi-source analysis)
- **Level 4**: Research frontiers (open questions, emerging tech)

## 📈 **Research Progress Tracking**

### **Current Maturity**
- **Conceptual Foundation**: 85% complete
- **Source Documentation**: 60% complete
- **Synthesis & Integration**: 40% complete
- **Aviation Applications**: 35% complete

### **Priority Research Areas**
1. **Immediate**: Core concept definitions (SBAS, GBAS, ABAS)
2. **Short-term**: Regional system comparisons
3. **Medium-term**: Civil aviation integration patterns
4. **Long-term**: Future trends & open research questions
5. **Current expansion**: ASEAN readiness, governance, and service-model research
6. **Empirical**: Ionospheric threat discovery for equatorial SBAS using GNSS-RO — [[IRI-2020 vs GNSS-RO Indonesia]], [[SBAS Ionospheric Threat — Empirical Evidence]], [[Indonesian SBAS ION Paper Iterations]]

## 📝 **Research Notes Management**

### **Active provenance work**
- Current backlog: [[SBAS Source Backlog]]
- Active source scaffolds: [[Source - RTCA DO-229]], [[Source - RTCA DO-242]], [[Source - RTCA DO-289]], [[Source - ICAO Doc 9854]], [[Source - ICAO Doc 9855]]
- Empirical source scaffolds: [[Source - GNSS Radio Occultation Technique]], [[Source - IRI-2020 Ionosphere Model]], [[Source - GNSS-RO Indonesia Empirical Study]]
- Immediate goal: turn high-frequency standards references into dedicated source notes before expanding quantitative claims.

### **Active regional expansion work**
- [[ASEAN SBAS Adoption Landscape]]
- [[ASEAN SBAS Readiness Heuristic]]
- [[ASEAN SBAS Operational Demand Drivers]]
- [[ASEAN SBAS Deployment Barriers]]
- [[ASEAN SBAS Governance and Institutional Actors]]
- [[ASEAN SBAS Service-Model Options]]
- country child notes for [[Indonesia]], [[Philippines]], [[Singapore]], [[Malaysia]], [[Thailand]], [[Viet Nam]], [[Lao PDR]], [[Cambodia]], [[Myanmar]], and [[Brunei Darussalam]]
- evidence-aware tightening now started for [[Singapore]], [[Indonesia]], [[Philippines]], [[Malaysia]], and [[Thailand]] through dedicated ASEAN source scaffolds
- current strongest early country evidence split: institutional-readiness signals for [[Singapore]], [[Malaysia]], and [[Thailand]]; distributed-network demand/context signals for [[Indonesia]] and [[Philippines]]
- empirical ionospheric evidence for [[Indonesia]]: [[IRI-2020 vs GNSS-RO Indonesia]], [[SBAS Ionospheric Threat — Empirical Evidence]]

### **Source Note Format**
```
--
title: [Source Title]
authors: [Author(s)]
source_type: [standard/paper/report/presentation]
date: [YYYY-MM-DD]
topic_tags: [tag1, tag2, ...]
--

## Summary
[Brief summary]

## Key Claims
- Claim 1: [with evidence]
- Claim 2: [with evidence]

## Technical Details
[Specifications, data, methods]

## Limitations & Uncertainties
[What's unknown or disputed]

## Relevance to SBAS
[How this applies to aviation SBAS]
```

### **Synthesis Note Format**
```
--
title: [Synthesis Topic]
type: [literature-review/comparative-analysis/integration]
sources: [[Source1], [Source2], ...]
--

## Consensus
[What multiple sources agree on]

## Divergent Views
[Where sources disagree]

## Evidence Quality
[Assessment of source reliability]

## Aviation Implications
[Operational meaning]
```

## 🎯 **Next Research Steps**

### Empirical Ionospheric Research (new)
- [ ] Deepen [[Source - GNSS-RO Indonesia Empirical Study]] with verified dataset metadata
- [ ] Add ground GNSS CORS/IGS validation for Indonesian TEC
- [ ] Targeted post-sunset GNSS-RO acquisition (18–21 LT gap)
- [ ] Convert threat-budget scaffold into candidate GIVE-like bins after validation
- [ ] Extend IGRF analysis to full-year or multi-year sampling

### **Week 1-2: Foundation**
- [ ] Create core concept notes (SBAS, GBAS, ABAS)
- [ ] Document GNSS error sources
- [ ] Establish SBAS architecture notes

### **Week 3-4: Applications**
- [ ] Create approach procedure notes (LPV, APV, etc.)
- [ ] Document operational use cases
- [ ] Analyze airport accessibility

### **Week 5-6: Regional Systems**
- [ ] Create individual regional system notes
- [ ] Build comparative analysis
- [ ] Document standards requirements

### **Week 7-8: Integration**
- [ ] Complete synthesis notes
- [ ] Build MOC navigation
- [ ] Establish open questions

*MOC Version: 1.0 | Status: Research Planning | Next Update: 2026-04-30*

## GIPTA 2.0 research expansion — 2026-05-01
- [[GIPTA 2.0 MOC]]
- [[GIPTA 2.0 and ASEAN SBAS Implementation Pathway]]
- [[ASEAN SBAS Testbed to Operational Service]]
- [[Source - ASEAN SBAS Testbed Development Proposal]]
- [[Source - ADB ASEAN SBAS Technical Assistance]]
