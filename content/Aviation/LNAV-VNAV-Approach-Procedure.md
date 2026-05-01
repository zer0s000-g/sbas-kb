---
title: LNAV/VNAV Approach Procedure and SBAS Integration
description: Detailed procedure for Lateral Navigation / Vertical Navigation approaches using SBAS augmentation
tags: [aviation, approach, lnav-vnav, sbas, cdm, performance]
category: aviation-operations
created: 2026-04-19
modified: 2026-04-19
version: 1.0
---

# ✈️ LNAV/VNAV Approach Procedure and SBAS Integration

## 📋 **Procedure Overview**

**LNAV/VNAV (Lateral Navigation / Vertical Navigation)** is a non-precision approach that combines:
- Lateral guidance via GPS/SBAS
- Vertical guidance with advisory glideslope
- SBAS-provided integrity monitoring
- Simplified approach procedure compared to LPV

## 📊 **Technical Specifications**

### **Performance Requirements**
```
LATERAL GUIDANCE:
  Accuracy: ±25m (95%)
  Alert Limit: ±50m
  Detection Time: <2 seconds

VERTICAL GUIDANCE:
  Accuracy: ±50m (95%)
  Alert Limit: ±100m  
  Glideslope: 3° nominal (advisory)

INTEGRITY:
  Protection Level: LNAV/VNAV equivalent
  False Alarm Rate: <0.01% per approach
  Detection Time: <6 seconds
  Availability: 99.8% during approach
```

### **SBAS Requirements for LNAV/VNAV**
- **Correction Update Rate**: 1-6 seconds
- **Position Accuracy**: 0.8m horizontal (95%)
- **Integrity Monitoring**: Continuous fault detection
- **Signal Processing**: Multi-constellation support

## 🔧 **Procedure Phases**

### **1. Initial Approach**
- **Entry Point**: LNAV/VNAV initial approach fix
- **Configuration**: Aircraft in approach configuration
- **Speed Management**: Target approach speed + wind correction
- **SBAS Monitoring**: Verify correction lock and integrity

### **2. Intermediate Approach**
- **Altitude**: 2,500 feet AGL minimum
- **Track**: Follow LNAV lateral path
- **Configuration**: Flaps 15-20°, speed reduction
- **Monitoring**: Lateral deviation ±150 feet

### **3. Final Approach**
- **Decision Height**: Minimum 300 feet AGL (LNAV/VNAV minimum)
- **Track**: Final course alignment
- **Configuration**: Full flaps, landing checklist
- **SBAS Alerting**: Monitor for integrity warnings

### **4. Missed Approach**
- **Trigger**: Loss of SBAS signal or altitude violation
- **Initial Climb**: 300-600 feet AGL
- **Turn**: Standard missed approach procedure
- **SBAS Re-acquisition**: Re-establish correction lock

## 🛡️ **Safety Considerations**

### **Integrity Monitoring**
- **Continuous Checks**: 1 Hz minimum
- **Alert Levels**: Visual and aural warnings
- **Fail-Safe**: Automatic missed approach trigger
- **Backup Systems**: Traditional navigation aids

### **Weather Constraints**
- **Minimums**: LNAV/VNAV requires 400 feet ceiling, 1 SM visibility
- **Wind Limits**: Crosswind 25 knots maximum
- **Precipitation**: Light to moderate rain acceptable
- **Low Visibility**: Operations down to 300 feet possible

### **Aircraft Requirements**
- **SBAS Receiver**: Certified multi-constellation
- **Display Capability**: Lateral deviation indicator
- **Vertical Guidance**: Advisory glideslope display
- **Backup Navigation**: Traditional radio navaids

## 📊 **Operational Benefits**

### **Advantages Over Traditional Approaches**
- **Reduced Weather Delays**: 20-25% improvement
- **Fuel Savings**: 8-12% reduction via direct routing
- **Capacity Increase**: 15% more approaches per hour
- **Accessibility**: Remote airport capability

### **Economic Impact**
- **Infrastructure Savings**: No ILS/VOR installation
- **Operational Efficiency**: Reduced holding patterns
- **Environmental**: Lower emissions via optimized routing

## 🔧 **Implementation Requirements**

### **Ground Infrastructure**
- **SBAS Coverage**: Continental or regional augmentation
- **Reference Stations**: Within 500 km radius
- **Communication Links**: Reliable data transmission
- **Monitoring Systems**: 24/7 operational surveillance

### **Aircraft Certification**
- **Type Approval**: FAA/EASA SBAS LNAV/VNAV certification
- **Pilot Training**: 8-hour simulator plus 3 hours dual instruction
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
- **Controller Procedures**: Standardized LNAV/VNAV approach vectors
- **Separation Standards**: Reduced spacing possible
- **Traffic Flow**: Optimized routing via SBAS
- **Emergency Protocols**: Immediate failure procedures

## 📊 **Performance Metrics**

### **Approach Success Rates**
- **LNAV/VNAV vs Traditional**: 85% vs 80% (weather-dependent)
- **Cancellation Rate**: 15% vs 20% (traditional)
- **On-Time Performance**: 80% improvement
- **Fuel Efficiency**: 10% savings average

### **Cost-Benefit Analysis**
- **Implementation Cost**: $200K - $1M per airport
- **Annual Savings**: $1-3M per major airport
- **ROI Period**: 4-6 years
- **Environmental Benefit**: 8,000 tons CO2 reduction annually

## 🔗 **Related Knowledge Links**
- [[SBAS-Terminology]](Concepts/SBAS-Terminology.md) - Core definitions and terminology
- [[Safety-Terminology]](Concepts/Safety-Terminology.md) - Safety and integrity requirements
- [[Communication-Terminology]](Concepts/Communication-Terminology.md) - Communication protocols and data formats
- [[MOCs/SBAS-in-Civil-Aviation-MOC.md]](MOCs/SBAS-in-Civil-Aviation-MOC.md) - Operational procedures and use cases
- [[Standards-Regulation/SBAS-Standards-Regulation.md]](Standards-Regulation/SBAS-Standards-Regulation.md) - Certification and regulatory requirements
- [[Aviation/LPV-Approach-Procedure.md]](Aviation/LPV-Approach-Procedure.md) - LPV approach procedures and integration
- [[Aviation/RNAV-Approach-Procedure.md]](Aviation/RNAV-Approach-Procedure.md) - RNAV approach procedures and integration

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
- **Hybrid Approaches**: LNAV/VNAV + RNAV integration

*Document Status: Draft | Next Review: 2026-05-03 | Version: 1.0*
