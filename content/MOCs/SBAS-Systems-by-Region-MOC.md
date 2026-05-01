--
title: SBAS Systems by Region MOC
description: Regional SBAS implementations, performance, and interoperability
tags: [MOC, regional, sbas, comparison]
category: mocs
created: 2026-04-19
modified: 2026-05-01
version: 1.0
status: research
--

# 🗺️ SBAS Systems by Region MOC

## 📋 **Regional System Overview**

### **Primary SBAS Implementations**

#### **WAAS (Wide Area Augmentation System) - USA**
- See dedicated note: [[WAAS]]
- **Coverage**: Continental USA, Alaska, Hawaii, parts of Canada/Mexico
- **Satellites**: 3 GEO (G1, G2, G3)
- **Uplink**: 7150-7250 MHz
- **Accuracy**: 0.5-1.0 m (95%)
- **Status**: Operational since 2003
- **Key Features**: Full LPV approach support, oceanic coverage

#### **EGNOS (European Geostationary Navigation Overlay Service) - Europe**
- See dedicated note: [[EGNOS]]
- **Coverage**: European territory + surrounding regions
- **Satellites**: 3 GEO (E1, E2, E3)
- **Uplink**: 1575.42 MHz (L1)
- **Accuracy**: 0.7-1.5 m (95%)
- **Status**: Operational since 2011
- **Key Features**: Certified for LPV, interoperable with WAAS

#### **MSAS (Multi-functional Satellite Augmentation System) - Japan**
- See dedicated note: [[MSAS]]
- **Coverage**: Japan, selected Pacific regions
- **Satellites**: 4 GEO (M1-M4)
- **Uplink**: 1575.42 MHz
- **Accuracy**: 0.5-1.0 m (95%)
- **Status**: Operational since 2007
- **Key Features**: Strong focus on oceanic operations

#### **GAGAN (GPS Aided Geo Augmented Navigation) - India**
- See dedicated note: [[GAGAN]]
- **Coverage**: India, surrounding regions
- **Satellites**: 3 GEO (GAG-1, GAG-2, GAG-3 planned)
- **Uplink**: 1575.42 MHz
- **Accuracy**: 1.0-2.0 m (95%)
- **Status**: Operational since 2011
- **Key Features**: Cost-effective implementation, growing coverage

#### **BDSBAS (BeiDou Satellite-Based Augmentation System) - China**
- See dedicated note: [[BDSBAS]]
- **Coverage**: China, Asia-Pacific
- **Satellites**: 3 GEO (B1, B2, B3)
- **Uplink**: 1575.42 MHz
- **Accuracy**: 0.5-1.0 m (95%)
- **Status**: Operational since 2012 (enhanced 2020)
- **Key Features**: Integrated BeiDou constellation

### **Emerging Systems**
- **KASS (Korean Augmentation Satellite System)** - South Korea
- **SDCM (System for Differential Correction and Monitoring)** - Russia
- **ARAIM** - Advanced RAIM for global coverage

### **Regional Adoption Branches Without a Unified System Note**
- **ASEAN / Southeast Asia** - current gap area focused on implementation readiness, governance, and service-model choices rather than an already-deployed common system
- Start here: [[ASEAN SBAS Adoption Landscape]]
- Country grouping and prioritization: [[ASEAN SBAS Readiness Heuristic]]
- Pathway choices: [[ASEAN SBAS Service-Model Options]]

## 🔧 **Performance Comparison**

| System | Accuracy | Coverage | Uplink Freq | Status | Key Strength |
|--------|----------|----------|-------------|--------|-------------|
| WAAS | 0.5-1.0m | Continental | 7150-7250 MHz | Mature | LPV capability |
| EGNOS | 0.7-1.5m | European | 1575.42 MHz | Mature | Interoperability |
| MSAS | 0.5-1.0m | Regional | 1575.42 MHz | Mature | Oceanic focus |
| GAGAN | 1.0-2.0m | Regional | 1575.42 MHz | Growing | Cost-effective |
| BDSBAS | 0.5-1.0m | Regional | 1575.42 MHz | Growing | BeiDou integration |

## 🎯 **Interoperability Analysis**

### **Cross-System Compatibility**
- **WAAS-EGNOS**: Certified for joint use in transatlantic operations
- **EGNOS-MSAS**: Compatible for European-Asian routes
- **Multi-constellation receivers**: Support all systems simultaneously

### **Operational Benefits**
- **Redundancy**: Multiple systems provide backup coverage
- **Global coverage**: No oceanic gaps
- **Flexible routing**: Choose routes based on system availability
- **Competitive pricing**: Multiple suppliers drive innovation

## 📊 **Regional Performance Metrics**

### **Uptime Statistics**
- **WAAS**: >99.95% annual uptime
- **EGNOS**: >99.9% annual uptime  
- **MSAS**: >99.9% annual uptime
- **GAGAN**: >99.8% annual uptime (growing)

### **Infrastructure Requirements**
- **Reference Stations**: 12-24 per region (varies by size)
- **Uplink Stations**: 3-6 per region
- **Monitoring Centers**: 1-2 per region
- **Satellites**: 3-4 per system (GEO)

## 🔍 **Integration Challenges**

### **Technical Issues**
- **Frequency coordination**: Avoid interference between systems
- **Message format differences**: Ensure compatibility
- **Timing synchronization**: Nanosecond precision required
- **Receiver complexity**: Multi-system support increases cost

### **Regulatory Issues**
- **Spectrum allocation**: National regulations vary
- **Certification requirements**: Different approval processes
- **Data sharing agreements**: Privacy and security concerns

## 🔙 **Future Developments**

### **System Upgrades**
- **Second-generation satellites**: Higher power, better accuracy
- **L-band integration**: Single-frequency operations
- **AI-enhanced monitoring**: Predictive failure detection
- **Quantum timing**: Improved synchronization

### **Coverage Expansion**
- **Arctic coverage**: Address polar routing needs
- **Maritime extension**: Oceanic operations support
- **Urban enhancement**: Dense city coverage
- **Mountain terrain**: Challenging environment solutions

## 📚 **Knowledge Connections**

### **Linked Concepts**
- [[SBAS-Terminology]] - Core definitions
- [[SBAS Integrity]] - Integrity concept scaffold
- [[Protection Levels]] - Operational bound concept scaffold
- [[Alert Limits]] - Alerting-bound concept scaffold
- [[WAAS]] - regional system note (U.S. context)
- [[EGNOS]] - regional system note (European context)
- [[MSAS]] - regional system note (Japan/Pacific context)
- [[GAGAN]] - regional system note (India context)
- [[BDSBAS]] - regional system note (China/Asia-Pacific context)
- [[WAAS vs EGNOS]] - first regional comparison note
- [[MSAS vs GAGAN]] - Asia-focused regional comparison note
- [[Asia-Pacific SBAS Implementation Patterns]] - Asia-focused synthesis note
- [[ASEAN SBAS Adoption Landscape]] - Southeast Asia implementation branch
- [[ASEAN SBAS Readiness Heuristic]] - country grouping and prioritization heuristic
- [[ASEAN SBAS Service-Model Options]] - pathway comparison for Southeast Asia
- [[SBAS-vs-Other-Augmentation-Methods]] - Comparative analysis

### **Research Priorities**
1. Real-time performance monitoring across regions
2. Cost-effectiveness analysis by region
3. Pilot acceptance and training requirements
4. Future-proofing for next-generation systems
5. Compare Asia-Pacific patterns via [[Asia-Pacific SBAS Implementation Patterns]]
6. Build ASEAN-specific regional implementation knowledge via [[ASEAN SBAS Adoption Landscape]]

*MOC Version: 1.0 | Status: Draft | Next Update: 2026-04-26*

## 📜 **Standards & Certification Links**
- [[SBAS-Standards-Regulation.md]] - Primary standards documentation
- [[SBAS-vs-Other-Standards.md]] - Comparative standards analysis
- [[ICAO-SBAS-Standards-Library.md]] - Complete regulatory library
- [[Source - RTCA DO-229]] - provisional source scaffold for equipment-standard references

## 🚀 **Regulatory Resources**
- Certification requirements by jurisdiction
- Type approval processes
- Continuing airworthiness requirements
- Maintenance program standards

## GIPTA 2.0 ASEAN planning layer
- [[GIPTA 2.0 MOC]] adds source-linked material for ASEAN implementation planning, testbed development, and service-model comparison.
- [[Japan MSAS GBAS Lessons for ASEAN SBAS]] connects Japan comparator evidence to ASEAN service-model options without treating MSAS expansion as already selected.
