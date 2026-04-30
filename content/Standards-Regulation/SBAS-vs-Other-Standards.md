--
title: SBAS Standards Comparison
description: Comparative analysis of SBAS, GBAS, ABAS, and RAIM standards and requirements
tags: [standards, comparison, sbas, gbas, abas, raim]
category: standards
created: 2026-04-19
modified: 2026-04-23
version: 1.0
status: draft
--

# 📜 SBAS Standards Comparison

## Provenance status — 2026-04-23
- This note is still a draft comparison layer, not a verified source note.
- Several document-to-topic mappings below remain provisional until checked against dedicated source notes.
- Current source scaffolds: [[Source - RTCA DO-229]], [[Source - RTCA DO-242]], [[Source - ICAO Doc 9855]].
- Treat broad statements about certification focus or document scope as synthesis pending direct source verification.

## 📊 **Standards Framework Comparison**

| Standard Type | Primary Authority | Key Documents | Certification Focus |
|---------------|-------------------|---------------|---------------------|
| **SBAS** | ICAO, RTCA, EUROCAE | Doc 8083, DO-242, ED-52 | System-level certification |
| **GBAS** | ICAO, RTCA, EUROCAE | Doc 7084, DO-229, ED-102 | Equipment & approach certification |
| **ABAS** | RTCA | DO-296, DO-229 | Receiver autonomous integrity |
| **RAIM** | RTCA, ICAO | DO-229, DO-242 | Built-in receiver integrity |

## 🔧 **ICAO Standardization**

### **Core ICAO Documents for SBAS**
- **Doc 8083**: Procedures for Air Navigation Services
  - Contains SBAS-specific SARPs
  - Defines operational requirements
  - Establishes safety management framework
  
- **Doc 9855**: Technical Specifications for SBAS
  - Detailed technical requirements
  - Performance specifications
  - Interface definitions

### **ICAO SARPs Structure**
```
SARPs (Standards and Recommended Practices)
    ├─ Volume I: Personnel Licensing
    ├─ Volume II: Airworthiness
    ├─ Volume III: Meteorology
    ├─ Volume IV: Aeronautical Telecommunications
    └─ Volume V: Air Navigation Services ← SBAS SARPs here
```

## 🔍 **Regulatory Compliance Matrix**

### **SBAS Certification Requirements**
| Requirement | SBAS | GBAS | ABAS | RAIM |
|-------------|------|------|------|------|
| **Type Certification** | Required | Required | Optional | Not applicable |
| **Performance Testing** | Extensive | Extensive | Moderate | Limited |
| **Field Evaluation** | Required | Required | Optional | Not applicable |
| **Safety Assessment** | Mandatory | Mandatory | Recommended | Not applicable |
| **Ongoing Monitoring** | Required | Required | Optional | Not applicable |

### **Key Regulatory Differences**
- **SBAS**: System-level certification, broader coverage
- **GBAS**: Focus on approach procedures, site-specific
- **ABAS**: Receiver-level certification, less stringent
- **RAIM**: Algorithm-based, receiver-integrated

## 🚀 **Implementation Standards**

### **SBAS Technical Standards**
- **Message Format**: Standardized correction messages
- **Timing Requirements**: Nanosecond precision
- **Accuracy Specifications**: Defined by application
- **Integrity Monitoring**: Continuous fault detection

### **Cross-System Standards**
- **Message Compatibility**: Ensure interoperability
- **Timing Synchronization**: Coordinated clocks
- **Frequency Management**: Spectrum coordination
- **Data Exchange**: Standardized formats

## 🎯 **Research & Development Standards**

### **Emerging Technology Standards**
- **Dual-Frequency Operations**: L1+L5 integration
- **Modernized SBAS**: Next-generation capabilities
- **Cybersecurity Requirements**: Enhanced protection
- **Data Privacy**: Protection frameworks

### **Harmonization Efforts**
- **Global Standards**: ICAO-led initiatives
- **Regional Cooperation**: Mutual recognition
- **Simplified Certification**: Streamlined processes
- **Cost Reduction**: Efficiency improvements

## 🔮 **Key Standards References**

### **Primary Standards**
1. ICAO Doc 8083 - Procedures for Air Navigation Services
2. [[Source - RTCA DO-229]] - current provisional airborne-equipment source scaffold
3. EUROCAE ED-52 - EGNOS Technical Specifications
4. [[Source - RTCA DO-242]] - current provisional augmentation-system source scaffold

### **Supporting Standards**
1. [[Source - ICAO Doc 9855]] - current provisional ICAO technical-specification source scaffold
2. RTCA DO-289 - SBAS Performance Testing
3. EUROCAE ED-102 - Interface Specifications
4. RTCA DO-296 - RNP Performance Requirements

## 🚀 **Future Regulatory Trends**

### **Upcoming Standards**
- **Advanced SBAS**: Next-generation capabilities
- **L5 Integration**: Dual-frequency operations
- **Enhanced Safety**: Stricter requirements
- **Global Harmonization**: Unified standards

### **Regulatory Challenges**
- Technology evolution pace
- Regional variation management
- Cost-effective compliance
- Training and education

*Document Status: Draft | Next Review: 2026-07-19 | Version: 1.0*
