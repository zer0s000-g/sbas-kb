---
title: RNP Approach Procedure and SBAS Integration
description: Detailed procedure for Required Navigation Performance approaches using SBAS augmentation
tags: [aviation, approach, rnp, sbas, cdm, performance]
category: aviation-operations
created: 2026-04-19
modified: 2026-04-19
version: 1.0
---

# ✈️ RNP Approach Procedure and SBAS Integration

## 📋 **Procedure Overview**

**RNP (Required Navigation Performance)** is a navigation specification that enables:
- Performance-based navigation with specific accuracy requirements
- SBAS-provided integrity monitoring
- Reduced separation standards and increased capacity
- Flexible flight paths and optimized routing

## 📊 **Technical Specifications**

### **Performance Requirements**
```
NAVIGATION ACCURACY:
  Required: RNP 0.3 (0.3 NM) for terminal operations
  Alert Limit: 0.5 NM
  Containment: 95% probability

SBAS REQUIREMENTS:
  Correction Update: 1-6 seconds
  Position Accuracy: 0.8m horizontal (95%)
  Integrity: Fault detection <6 seconds
  Availability: 99.9% during approach

RNP SPECIFICATIONS:
  RNP 0.3: Terminal operations (0.3 NM accuracy)
  RNP 1.0: En-route operations (1.0 NM accuracy)
  RNP 2.0: Oceanic operations (2.0 NM accuracy)
```

### **SBAS Integration**
- **Correction Data**: Differential corrections from ground network
- **Integrity Monitoring**: Real-time fault detection
- **Position Updates**: Continuous SBAS-enhanced positioning
- **Alerting**: Visual and aural warnings for integrity issues

## 🔧 **Procedure Phases**

### **1. Initial Approach**
- **Entry Point**: RNP initial approach fix (IAF)
- **Configuration**: Aircraft in approach configuration
- **Speed Management**: Target approach speed + wind correction
- **SBAS Monitoring**: Verify correction lock and integrity

### **2. Intermediate Approach**
- **Altitude**: 2,000 feet AGL minimum
- **Track**: Follow RNP lateral path
- **Configuration**: Flaps 15-20°, speed reduction
- **Monitoring**: Lateral deviation ±150 feet

### **3. Final Approach**
- **Decision Height**: Minimum 200 feet AGL
- **Track**: Final course alignment
- **Configuration**: Full flaps, landing checklist
- **SBAS Alerting**: Monitor for integrity warnings

### **4. Missed Approach**
- **Trigger**: Loss of SBAS signal or altitude violation
- **Initial Climb**: 250-500 feet AGL
- **Turn**: Standard missed approach procedure
- **SBAS Re-acquisition**: Re-establish correction lock

## 🛡️ **Safety Considerations**

### **Integrity Monitoring**
- **Continuous Checks**: 1 Hz minimum
- **Alert Levels**: Visual and aural warnings
- **Fail-Safe**: Automatic missed approach trigger
- **Backup Systems**: Traditional navigation aids

### **Weather Constraints**
- **Minimums**: RNP requires 400 feet ceiling, 1 SM visibility
- **Wind Limits**: Crosswind 30 knots maximum
- **Precipitation**: Moderate rain acceptable
- **Low Visibility**: Operations down to 200 feet possible

### **Aircraft Requirements**
- **SBAS Receiver**: Certified multi-constellation
- **Display Capability**: Lateral deviation indicator
- **Autopilot**: Coupled to SBAS guidance
- **Backup Navigation**: Traditional radio navaids

## 📊 **Operational Benefits**

### **Advantages Over Traditional Approaches**
- **Reduced Weather Delays**: 25-30% improvement
- **Fuel Savings**: 10-15% reduction via direct routing
- **Capacity Increase**: 20% more approaches per hour
- **Accessibility**: Remote airport capability

### **Economic Impact**
- **Infrastructure Savings**: No VOR/DME installation
- **Operational Efficiency**: Reduced holding patterns
- **Environmental**: Lower emissions via optimized routing

## 🔧 **Implementation Requirements**

### **Ground Infrastructure**
- **SBAS Coverage**: Continental or regional augmentation
- **Reference Stations**: Within 500 km radius
- **Communication Links**: Reliable data transmission
- **Monitoring Systems**: 24/7 operational surveillance

### **Aircraft Certification**
- **Type Approval**: FAA/EASA SBAS RNP certification
- **Pilot Training**: 10-hour simulator plus 5 hours dual instruction
- **Equipment Check**: Pre-flight SBAS verification
- **Documentation**: Updated flight manual procedures

## ⚠️ **Limitations and Constraints**

### **Operational Restrictions**
- **Geographic**: Requires SBAS coverage area
- **Temporal**: Sun interference during equinox periods
- **Equipment**: Single-frequency receivers not approved
- **Procedural**: Specific approach chart requirements

### **Known Issues**
- **Ionospheric Disturbances**: Solar activity impact
- **Multipath Effects**: Urban canyon interference
- **Receiver Sensitivity**: Cold start acquisition time
- **Data Latency**: Correction transmission delays

## 🔄 **Integration with Other Systems**

### **SBAS Architecture**
- **Reference Network**: Local ground stations
- **Satellite Links**: GEO broadcast correction data
- **User Equipment**: Multi-constellation receivers
- **Monitoring**: Real-time integrity verification

### **Air Traffic Management**
- **Controller Procedures**: Standardized RNP approach vectors
- **Separation Standards**: Reduced spacing possible
- **Traffic Flow**: Optimized routing via SBAS
- **Emergency Protocols**: Immediate failure procedures

## 📊 **Performance Metrics**

### **Approach Success Rates**
- **RNP vs Traditional**: 88% vs 85% (weather-dependent)
- **Cancellation Rate**: 12% vs 15% (traditional)
- **On-Time Performance**: 85% improvement
- **Fuel Efficiency**: 12% savings average

### **Cost-Benefit Analysis**
- **Implementation Cost**: $300K - $1.5M per airport
- **Annual Savings**: $2-5M per major airport
- **ROI Period**: 3-5 years
- **Environmental Benefit**: 10,000 tons CO2 reduction annually

## 🔗 **Related Knowledge Links**
- [[SBAS-Terminology]](Concepts/SBAS-Terminology.md) - Core definitions and terminology
- [[Safety-Terminology]] - Safety and integrity requirements
- [[Communication-Terminology]] - Communication protocols and data formats
- [[SBAS in Civil Aviation MOC]](MOCs/SBAS-in-Civil-Aviation-MOC.md) - Operational procedures and use cases
- [[SBAS-Standards-Regulation]](Standards-Regulation/SBAS-Standards-Regulation.md) - Certification and regulatory requirements
- [[LPV-Approach-Procedure]](Aviation/LPV-Approach-Procedure.md) - LPV approach procedures and integration
- [[RNAV-Approach-Procedure]](Aviation/RNAV-Approach-Procedure.md) - RNAV approach procedures and integration
- [[LNAV-VNAV-Approach-Procedure]](Aviation/LNAV-VNAV-Approach-Procedure.md) - LNAV/VNAV approach procedures and integration

## 📝 **Research Notes**

### **Open Questions**
1. Urban canyon multipath mitigation effectiveness
2. Solar activity impact on tropical regions
3. Single-frequency receiver certification feasibility
4. Cost optimization for small airports

### **Future Considerations**
- **4D Trajectory**: Time-based procedures
- **A2C2 Integration**: Aircraft-to-controller communication
- **UAM Preparation**: Urban air mobility compatibility
- **Hybrid Approaches**: RNP + RNAV integration

*Document Status: Draft | Next Review: 2026-05-03 | Version: 1.0*
