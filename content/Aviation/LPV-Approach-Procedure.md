--
title: LPV Approach Procedure and SBAS Integration
description: Detailed procedure for Localizer Performance with Vertical guidance using SBAS
tags: [aviation, approach, lpv, sbas, cdm, performance]
category: aviation-operations
created: 2026-04-19
modified: 2026-04-19
version: 1.0
--

# ✈️ LPV Approach Procedure and SBAS Integration

## 📋 **Procedure Overview**

**LPV (Localizer Performance with Vertical)** is a Category A approach that combines:
- Lateral guidance equivalent to Localizer
- Vertical guidance with Glideslope equivalent
- SBAS-provided integrity monitoring
- Precision approach capability without traditional ILS

## 📊 **Technical Specifications**

### **Performance Requirements**
```
LATERAL GUIDANCE:
  Accuracy: ±10m (95%)
  Alert Limit: ±20m
  Detection Time: <2 seconds

VERTICAL GUIDANCE:
  Accuracy: ±15m (95%)
  Alert Limit: ±30m  
  Glideslope: 3° nominal

INTEGRITY:
  Protection Level: CAT I equivalent
  False Alarm Rate: <0.001% per approach
  Detection Time: <6 seconds
  Availability: 99.9% during approach
```

### **SBAS Requirements for LPV**
- **Correction Update Rate**: 1-6 seconds
- **Position Accuracy**: 0.8m horizontal (95%)
- **Integrity Monitoring**: Continuous fault detection
- **Signal Processing**: Dual-frequency (L1+L5) recommended

## 🔧 **Procedure Phases**

### **1. Initial Approach**
- **Entry Point**: SBAS-defined initial approach fix
- **Speed Management**: Target Vref + wind correction
- **Configuration**: Landing gear down, flaps 15-20°
- **SBAS Monitoring**: Verify correction lock

### **2. Intermediate Approach**
- **Altitude**: 1,500 feet AGL minimum
- **Track**: Follow SBAS lateral path
- **Configuration**: Flaps 30-40°, speed reduction
- **Monitoring**: Vertical deviation ±100 feet

### **3. Final Approach**
- **Decision Height**: Minimum 200 feet AGL (LPV minimum)
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
- **Backup Systems**: RAIM or alternative navigation

### **Weather Constraints**
- **Minimums**: LPV requires 400 feet ceiling, 1 SM visibility
- **Wind Limits**: Crosswind 30 knots maximum
- **Precipitation**: Moderate rain acceptable with proper configuration
- **Low Visibility**: Operations down to 200 feet possible with LPV

### **Aircraft Requirements**
- **SBAS Receiver**: Certified multi-constellation
- **Display Capability**: Vertical deviation indicator
- **Autopilot**: Coupled to SBAS guidance
- **Backup Navigation**: Traditional radio navaids

## 📊 **Operational Benefits**

### **Advantages Over Traditional Approaches**
- **Reduced Weather Delays**: 30-40% improvement in low visibility
- **Fuel Savings**: 15-20% reduction via direct routing
- **Capacity Increase**: 25% more approaches per hour
- **Accessibility**: Remote airport capability

### **Economic Impact**
- **Infrastructure Savings**: No ILS installation ($2-5M per installation)
- **Operational Efficiency**: Reduced holding patterns
- **Environmental**: Lower emissions via optimized routing

## 🔧 **Implementation Requirements**

### **Ground Infrastructure**
- **SBAS Coverage**: Continental or regional augmentation
- **Reference Stations**: Within 500 km radius
- **Communication Links**: Reliable data transmission
- **Monitoring Systems**: 24/7 operational surveillance

### **Aircraft Certification**
- **Type Approval**: FAA/EASA SBAS LPV certification
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
- **Controller Procedures**: Standardized LPV approach vectors
- **Separation Standards**: Reduced spacing possible
- **Traffic Flow**: Optimized routing via SBAS
- **Emergency Protocols**: Immediate failure procedures

## 📊 **Performance Metrics**

### **Approach Success Rates**
- **LPV vs ILS**: 92% vs 95% (weather-dependent)
- **Cancellation Rate**: 8% vs 12% (traditional)
- **On-Time Performance**: 88% improvement
- **Fuel Efficiency**: 18% savings average

### **Cost-Benefit Analysis**
- **Implementation Cost**: $500K - $2M per airport (vs $2-5M ILS)
- **Annual Savings**: $3-8M per major airport
- **ROI Period**: 2-4 years
- **Environmental Benefit**: 15,000 tons CO2 reduction annually

## 🔗 **Related Knowledge Links**
- [[SBAS-Terminology]](Concepts/SBAS-Terminology.md) - Core definitions and terminology
- [[Safety-Terminology]](Concepts/Safety-Terminology.md) - Safety and integrity requirements
- [[Communication-Terminology]](Concepts/Communication-Terminology.md) - Communication protocols and data formats
- [[MOCs/SBAS-in-Civil-Aviation-MOC.md]](MOCs/SBAS-in-Civil-Aviation-MOC.md) - Operational procedures and use cases
- [[Standards-Regulation/SBAS-Standards-Regulation.md]](Standards-Regulation/SBAS-Standards-Regulation.md) - Certification and regulatory requirements

## 📝 **Research Notes**

### **Open Questions**
1. Urban canyon multipath mitigation effectiveness
2. Solar activity impact on tropical regions
3. Single-frequency receiver certification feasibility
4. Cost optimization for small airports

### **Future Considerations**
- **GBAS Integration**: Hybrid approaches
- **4D Trajectory**: Time-based procedures
- **A2C2 Integration**: Aircraft-to-controller communication
- **UAM Preparation**: Urban air mobility compatibility

*Document Status: Draft | Next Review: 2026-05-03 | Version: 1.0*
