--
title: GBAS Approach Procedure and SBAS Integration
description: Detailed procedure for Ground-Based Augmentation System approaches using local ground stations
tags: [aviation, approach, gbas, sbas, cdm, performance]
category: aviation-operations
created: 2026-04-19
modified: 2026-04-19
version: 1.0
--

# ✈️ GBAS Approach Procedure and SBAS Integration

## 📋 **Procedure Overview**

**GBAS (Ground-Based Augmentation System)** is a precision approach system that enables:
- Local precision approach with 0.5-1m accuracy
- SBAS-provided integrity monitoring
- Airport-specific coverage with 50km radius
- CAT I, II, and III approach capabilities

## 📊 **Technical Specifications**

### **Performance Requirements**
```
POSITION ACCURACY:
  Lateral: ±0.5m (95%)
  Vertical: ±1.0m (95%)
  Integrity: Continuous monitoring

SBAS REQUIREMENTS:
  Correction Update: 1-6 seconds
  Position Accuracy: 0.8m horizontal (95%)
  Integrity: Fault detection <6 seconds
  Availability: 99.9% during approach

GBAS SPECIFICATIONS:
  Coverage: 50km radius around airport
  Accuracy: 0.5-1m horizontal (CAT I)
  Availability: 99.9% operational time
  Integrity: CAT I, II, III capabilities
```

### **SBAS Integration**
- **Correction Data**: Differential corrections from ground network
- **Integrity Monitoring**: Real-time fault detection
- **Position Updates**: Continuous GBAS-enhanced positioning
- **Alerting**: Visual and aural warnings for integrity issues

## 🔧 **Procedure Phases**

### **1. Initial Approach**
- **Entry Point**: GBAS initial approach fix
- **Configuration**: Aircraft in approach configuration
- **Speed Management**: Target approach speed + wind correction
- **GBAS Monitoring**: Verify correction lock and integrity

### **2. Intermediate Approach**
- **Altitude**: 1,500 feet AGL minimum
- **Track**: Follow GBAS lateral path
- **Configuration**: Flaps 15-20°, speed reduction
- **Monitoring**: Lateral deviation ±50 feet

### **3. Final Approach**
- **Decision Height**: Minimum 200 feet AGL (CAT I)
- **Track**: Final course alignment
- **Configuration**: Full flaps, landing checklist
- **GBAS Alerting**: Monitor for integrity warnings

### **4. Missed Approach**
- **Trigger**: Loss of GBAS signal or altitude violation
- **Initial Climb**: 300-600 feet AGL
- **Turn**: Standard missed approach procedure
- **GBAS Re-acquisition**: Re-establish correction lock

## 🛡️ **Safety Considerations**

### **Integrity Monitoring**
- **Continuous Checks**: 1 Hz minimum
- **Alert Levels**: Visual and aural warnings
- **Fail-Safe**: Automatic missed approach trigger
- **Backup Systems**: Traditional navigation aids

### **Weather Constraints**
- **Minimums**: GBAS requires 200 feet ceiling, 1/2 SM visibility
- **Wind Limits**: Crosswind 30 knots maximum
- **Precipitation**: Moderate rain acceptable
- **Low Visibility**: Operations down to 50 feet possible

### **Aircraft Requirements**
- **GBAS Receiver**: Certified multi-constellation
- **Display Capability**: Lateral deviation indicator
- **Vertical Guidance**: Precision glideslope display
- **Backup Navigation**: Traditional radio navaids

## 📊 **Operational Benefits**

### **Advantages Over Traditional Approaches**
- **Reduced Weather Delays**: 40-50% improvement
- **Fuel Savings**: 15-20% reduction via direct routing
- **Capacity Increase**: 25% more approaches per hour
- **Accessibility**: Remote airport capability

### **Economic Impact**
- **Infrastructure Savings**: No ILS installation
- **Operational Efficiency**: Reduced holding patterns
- **Environmental**: Lower emissions via optimized routing

## 🔧 **Implementation Requirements**

### **Ground Infrastructure**
- **Reference Stations**: Local ground-based receivers
- **Processing Center**: Central differential computation
- **Uplink Stations**: Ground transmitters to aircraft
- **Monitoring Systems**: 24/7 operational surveillance

### **Aircraft Certification**
- **Type Approval**: FAA/EASA GBAS certification
- **Pilot Training**: 10-hour simulator plus 5 hours dual instruction
- **Equipment Check**: Pre-flight GBAS verification
- **Documentation**: Updated flight manual procedures

## ⚠️ **Limitations and Constraints**

### **Operational Restrictions**
- **Geographic**: Airport vicinity only (50km radius)
- **Temporal**: Sun interference during equinox periods
- **Equipment**: Single-frequency receivers not approved
- **Procedural**: Specific approach chart requirements

### **Known Issues**
- **Multipath Effects**: Urban canyon interference
- **Receiver Sensitivity**: Cold start acquisition time
- **Data Latency**: Correction transmission delays
- **Maintenance**: Regular calibration required

## 🔄 **Integration with Other Systems**

### **GBAS Architecture**
- **Reference Network**: Local ground stations
- **Processing Center**: Central differential computation
- **Uplink Stations**: Ground transmitters to aircraft
- **Monitoring**: Real-time integrity verification

### **Air Traffic Management**
- **Controller Procedures**: Standardized GBAS approach vectors
- **Separation Standards**: Reduced spacing possible
- **Traffic Flow**: Optimized routing via GBAS
- **Emergency Protocols**: Immediate failure procedures

## 📊 **Performance Metrics**

### **Approach Success Rates**
- **GBAS vs ILS**: 98% vs 95% (weather-dependent)
- **Cancellation Rate**: 2% vs 5% (traditional)
- **On-Time Performance**: 95% improvement
- **Fuel Efficiency**: 18% savings average

### **Cost-Benefit Analysis**
- **Implementation Cost**: $2-5M per airport
- **Annual Savings**: $3-8M per major airport
- **ROI Period**: 2-4 years
- **Environmental Benefit**: 15,000 tons CO2 reduction annually

## 🔗 **Related Knowledge Links**
- [[]()] -  - Core concepts
- [[]()] -  - Integrity requirements
- [[]()] -  - Data transmission
- [[]()] -  - Operational procedures
- [[]()] -  - Certification requirements
- [[]()] -  - LPV approach procedures
- [[]()] -  - RNAV approach procedures
- [[]()] -  - LNAV/VNAV approach procedures
- [[]()] -  - RNP approach procedures

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
- **Hybrid Approaches**: GBAS + SBAS integration

*Document Status: Draft | Next Review: 2026-05-03 | Version: 1.0*
