---
title: SBAS in Civil Aviation MOC
description: Operational use cases, approach procedures, and safety implications for SBAS in civil aviation
tags: [MOC, civil-aviation, sbas, approach, operations]
category: mocs
created: 2026-04-19
modified: 2026-04-23
version: 1.0
status: research
---

# 🛡️ SBAS in Civil Aviation MOC

## Initialization review — 2026-04-23
- Parent navigation: [[SBAS MOC]]
- This note captures important operational themes, but several quantitative claims and standards references still need source-note support.
- Treat this note as a draft civil-aviation map pending dedicated source extraction and concept-note expansion.
- Highest-value follow-up: connect approach concepts to sourced notes on integrity, protection levels, alert limits, and operational approvals.
- Related concept scaffolds now available: [[SBAS Integrity]] and [[Protection Levels]].

## 📊 **Operational Use Cases**

### **Approach Categories Supported by SBAS**

```
EN-ROUTE (E/R)
    ├── LNAV (Lateral Navigation Only)
    ├── LPV (Localizer Performance with Vertical) - requires SBAS
    └── APV (Approach with Vertical Guidance)

TERMINAL (T)
    ├── RNAV (GNSS) Approaches
    ├── LPV approaches
    ├── Visual with GNSS guidance

LANDING (L)
    ├── Precision approaches (GBAS preferred)
    └── Non-precision with GNSS final approach
```

### **Airspace Access Implications**

**Airport Categories by SBAS Capability**
- **Category 1**: Basic GNSS (no augmentation) - limited operations
- **Category 2**: SBAS-enabled - expanded operations
- **Category 3**: GBAS/SBAS combination - full operations

**Operational Benefits**:
- Extended operating hours (reduced weather constraints)
- New route availability (oceanic, polar)
- Reduced holding patterns
- Fuel savings from direct routing

## 🔧 **Technical Mechanisms**

### **LPV Approach Requirements**
```
SBAS provides:
- Lateral guidance: ±10m accuracy (95%)
- Vertical guidance: ±15m accuracy (95%)
- Alerting: <6 seconds detection time
- Availability: 99.9% during approach

Decision Height: 
- LPV: typically 200 feet AGL
- LNAV: typically 400+ feet AGL
```

### **Integrity Requirements for Approach**
- **Protection Level**: Must meet approach category requirements — see [[Protection Levels]]
- **Alert Limit**: Must be tighter than approach minimums — see [[Alert Limits]]
- **False Alarm Rate**: <0.001% per approach hour
- **Detection Time**: <6 seconds for critical faults
- **Concept context**: [[SBAS Integrity]]

## 📊 **Safety & Risk Analysis**

### **Risk Reduction Factors**
- **Loss of Navigation**: Reduced by SBAS redundancy
- **Terrain Conflicts**: Improved obstacle clearance awareness
- **Weather**: Reduced impact through precision guidance
- **Controller Workload**: Reduced through automation

### **Failure Modes**
- **SBAS Unavailability**: Revert to non-SBAS procedures
- **Single Frequency Loss**: Use backup frequency or revert
- **Ionospheric Disturbance**: Enhanced monitoring required
- **Receiver Failure**: Standard avionics redundancy

## 🌍 **Regional Implementation Patterns**

### **High-Capacity Regions**
- **USA (WAAS)**: Full LPV approach coverage — see [[WAAS]]
- **Europe (EGNOS)**: Extensive terminal area coverage — see [[EGNOS]]
- **Japan (MSAS)**: Oceanic and terminal operations — see [[MSAS]]

### **Developing Regions**
- **Asia-Pacific**: Gradual SBAS rollout — see [[Asia-Pacific SBAS Implementation Patterns]]
- **ASEAN / Southeast Asia**: adoption depends on readiness, governance, and service-model choice more than on generic SBAS awareness — see [[ASEAN SBAS Adoption Landscape]]
- **Middle East**: Select airport coverage
- **Africa**: Limited infrastructure

### **ASEAN-focused retrieval path**
- Demand side: [[ASEAN SBAS Operational Demand Drivers]]
- Constraint side: [[ASEAN SBAS Deployment Barriers]]
- Governance side: [[ASEAN SBAS Governance and Institutional Actors]]
- Country grouping: [[ASEAN SBAS Readiness Heuristic]]
- Pathway comparison: [[ASEAN SBAS Service-Model Options]]

## 🔐 **Standards & Certification**

### **Required Approvals**
- **ICAO Doc 8083**: SBAS SARPs compliance
- **RTCA DO-229**: Equipment minimum performance — see [[Source - RTCA DO-229]] for the current provisional source scaffold
- **National Airworthiness**: Local certification requirements
- **Airport Authority**: Local operational approval

### **Avionics Requirements**
- **Receiver Type**: SBAS-capable multi-constellation
- **Display Capability**: Vertical deviation indication
- **Alert System**: Visual/audio warnings
- **Logging**: Flight data recorder compatibility

## 🎯 **Research Questions & Gaps**

### **Open Questions**
- How does SBAS availability vary by geographic region?
- What are the economic benefits for small airports?
- How do pilots adapt to SBAS-dependent procedures?
- What are the cybersecurity implications of SBAS dependence?

### **Data Needs**
- Global SBAS uptime statistics
- Approach success rates with vs without SBAS
- Pilot adaptation timelines
- Cost-benefit analysis by airport category

## 🔮 **Key References Needed**
- ICAO SBAS implementation guides
- Regional air navigation plans
- Airport categorization documents
- Flight test reports

*MOC Version: 1.0 | Status: Draft | Next Update: 2026-04-26*
