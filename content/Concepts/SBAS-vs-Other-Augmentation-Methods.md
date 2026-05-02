---
title: SBAS vs Other Augmentation Methods
description: Comparative analysis of satellite-based augmentation vs ground-based and airborne augmentation
tags: [comparison, augmentation-methods, sbas, gbas, abas, raim]
category: concepts
created: 2026-04-19
modified: 2026-04-23
version: 1.0
---

# 🔄 SBAS vs Other Augmentation Methods

## 📊 **Overview Comparison**

| Method | Primary Use | Accuracy | Coverage | Infrastructure | Typical Applications |
|--------|-------------|----------|----------|----------------|---------------------|
| **SBAS** | Aviation safety | 1-3m | Continental | GEO satellites + ground | En-route, terminal, approach |
| **GBAS** | Precision approach | 0.5-1m | Airport vicinity | Local ground stations | LPV/RNAV approaches - see [[LPV-Approach-Procedure]] |
| **ABAS** | Receiver autonomous | 5-10m | Global | On-board | General aviation, RNP |
| **RAIM** | Integrity monitoring | 10-30m | Global | Receiver-based | Backup integrity |

## 🛫 Aviation Applications

SBAS enables precision approach procedures including **LPV (Localizer Performance with Vertical)** approaches. LPV provides precision guidance comparable to traditional ILS but uses satellite-based augmentation instead of ground-based equipment. See [[LPV-Approach-Procedure]] for detailed implementation.

## 🎯 **Key Differentiators**

### **Coverage Area**
- **SBAS**: Continental scale (single satellite ≈ 42% Earth coverage)
- **GBAS**: Local (≈ 50km radius around reference station)
- **ABAS**: Global (uses satellite geometry)
- **RAIM**: Global (relies on satellite geometry)

### **Accuracy Performance**
- **SBAS**: 1-3m horizontal (95% confidence)
- **GBAS**: 0.5-1m horizontal (precision approach standard)
- **ABAS**: 5-10m horizontal (typical RNP performance)
- **RAIM**: 10-30m horizontal (integrity bound)

### **Infrastructure Requirements**
- **SBAS**: Geostationary satellites + ground reference network + uplink stations
- **GBAS**: Local reference stations + VHF data transmission + airport facilities
- **ABAS**: No ground infrastructure (receiver-based)
- **RAIM**: Receiver processing only

### **Integrity Assurance**
- **SBAS**: Continuous monitoring, <6s detection time
- **GBAS**: Real-time monitoring, <1s detection
- **ABAS**: Depends on satellite geometry
- **RAIM**: Algorithm-based detection

## ⚙ **Aviation Application Context**

### **En-Route Operations**
- **Primary**: SBAS (continental coverage)
- **Alternative**: ABAS/RAIM (no ground infrastructure needed)
- **Use Case**: Long-haul oceanic and remote area operations

### **Terminal Area Operations**
- **Primary**: SBAS (wide area coverage)
- **Alternative**: GBAS (precision approaches)
- **Use Case**: Standard terminal vectoring and sequencing

### **Precision Approaches**
- **Primary**: GBAS (LPV, APV)
- **Secondary**: SBAS (LNAV/VNAV approaches)
- **Backup**: RAIM (integrity monitoring)

## 🔗 **Relationship to ICAO Standards**

### **SBAS and ICAO**
- **Doc 8083**: SARPs for SBAS operations
- **Doc 7084**: GBAS specifications
- **Doc 9854**: Performance requirements
- **Doc 9855**: Testing methodology

### **Complementary Use**
- SBAS provides broad-area coverage
- GBAS provides precision terminal services
- RAIM provides backup integrity monitoring
- ABAS provides receiver-level autonomy

## 📈 **Performance Trade-offs**

### **SBAS Advantages**
- Continental coverage with minimal ground infrastructure
- Suitable for oceanic and remote operations
- Lower recurring costs per user
- Standardized international specifications

### **SBAS Limitations**
- Higher latency (correction transmission)
- Less precision than GBAS for approaches
- Dependency on satellite availability
- Ionospheric sensitivity

### **LPV Approach Integration**

LPV (Localizer Performance with Vertical) approaches leverage GBAS infrastructure for precision terminal operations. See [[LPV-Approach-Procedure]] for detailed procedures.

### **GBAS Advantages**
- High precision for approaches
- Low latency corrections
- Independent of satellite geometry
- Better for urban canyon environments

### **GBAS Limitations**
- Local coverage only
- Requires extensive ground infrastructure
- Higher installation and maintenance costs
- Airport-specific deployment

## 🔮 **Future Integration Trends**

### **Hybrid Approaches**
- SBAS for en-route + GBAS for approaches
- Seamless transition between augmentation methods
- Multi-constellation receiver support
- Adaptive method selection based on context

### **Evolution Path**
- Increased SBAS precision through multi-GNSS
- GBAS expansion to multiple airports
- ABAS integration with onboard systems
- Unified performance standards across methods

## 📚 **Related Knowledge**
- [[SBAS-Terminology]] - Core SBAS concepts
- GNSS terminology - Satellite navigation fundamentals
- [[Safety-Terminology]] - Integrity and risk management
- navigation terminology - Performance metrics
- [[SBAS Source Backlog]] - Regulatory specifications

--
*Node: SBAS-vs-Other-Augmentation-Methods | Links: 6+ | Depth: 1 | Status: Created*

**Next best topic to expand**: Add specific regional system details (now including [[WAAS]], [[EGNOS]], [[MSAS]], [[GAGAN]], and [[BDSBAS]] as draft system notes) or expand Aviation/Operational Use Cases.

## 🛫 Aviation Applications

### **RNAV (Area Navigation) Approaches**
RNAV enables flexible point-to-point navigation without ground-based navaids. Key features:
- **Flexible routing**: Curved flight paths and optimized trajectories
- **Reduced infrastructure**: No VOR/DME requirements
- **SBAS integration**: Enhanced accuracy and integrity monitoring
- **Capacity increase**: 20% more approaches per hour

See [[RNAV-Approach-Procedure]] for detailed implementation procedures and operational requirements.


## 🛫 Aviation Applications

### **LNAV/VNAV (Lateral Navigation / Vertical Navigation) Approaches**
LNAV/VNAV provides non-precision approach capability with advisory vertical guidance. Key features:
- **Lateral navigation**: GPS-based lateral guidance
- **Vertical navigation**: Advisory glideslope (not precision)
- **SBAS integration**: Enhanced accuracy and integrity monitoring
- **Cost-effective**: Lower implementation cost than LPV

See [[LNAV-VNAV-Approach-Procedure]] for detailed implementation procedures and operational requirements.


## 🛫 Aviation Applications

### **RNP (Required Navigation Performance) Approaches**
RNP enables performance-based navigation with specific accuracy requirements. Key features:
- **Performance-based**: Specific accuracy requirements (RNP 0.3, RNP 1.0, etc.)
- **SBAS integration**: Enhanced accuracy and integrity monitoring
- **Reduced separation**: Lower separation standards possible
- **Flexible routing**: Optimized flight paths and trajectories

See [[RNP-Approach-Procedure]] for detailed implementation procedures and operational requirements.


## 🛫 Aviation Applications

### **GBAS (Ground-Based Augmentation System) Approaches**
GBAS provides precision approach capability with 0.5-1m accuracy. Key features:
- **Precision approach**: CAT I, II, and III capabilities
- **Local coverage**: 50km radius around airport
- **High accuracy**: 0.5-1m horizontal precision
- **Reduced weather delays**: 40-50% improvement

See [[GBAS-Approach-Procedure]] for detailed implementation procedures and operational requirements.
