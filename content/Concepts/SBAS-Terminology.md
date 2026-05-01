---
title: Satellite-Based Augmentation System (SBAS) Terminology
description: Core SBAS concepts, definitions, and technical specifications
tags: [terminology, sbas, gnss, corrections, integrity]
category: core-terminology
created: 2026-04-19
modified: 2026-04-19
version: 2.0
---

# 📖 Satellite-Based Augmentation System (SBAS) Terminology

## 📋 **SBAS Definition**
A ground-based augmentation system enhancing GNSS accuracy, integrity, and availability through differential correction transmitted via geostationary satellites.

## 🌐 **Core Technical Specifications**

### **System Architecture**
- **Reference Stations**: Ground-based GNSS receivers
- **Processing Center**: Central differential computation facility  
- **Uplink Stations**: Ground transmitters to GEO satellites
- **Satellite Network**: Geostationary broadcast satellites
- **User Receivers**: SBAS-capable positioning equipment

### **Performance Standards**
- **Update Rate**: 0.5 - 6 seconds per correction
- **Position Accuracy**: 1-3 meters (95% confidence)
- **Integrity Monitoring**: Continuous fault detection
- **Availability**: 99.9% operational time
- **Coverage**: Continental scale per satellite

## 🛠 **Technical Components**

### **Correction Types**
1. **Fast Corrections**: Pseudorange and carrier phase adjustments
2. **Long-term Corrections**: Ionospheric model updates
3. **Differential Code Biases**: Satellite-specific corrections
4. **URA (User Range Accuracy)**: Confidence interval indicators

### **Signal Processing**
- **Multi-constellation Support**: GPS, GLONASS, Galileo, BeiDou, QZSS
- **Ionospheric Correction**: Dual-frequency measurements
- **Message Generation**: Real-time correction computation
- **Broadcast Transmission**: Encoded satellite uplink

## 🔗 **Cross-Reference Links**
- [[SBAS-vs-Other-Augmentation-Methods]] - Comparative analysis
- [[SBAS-Signal-Processing]] - Signal processing algorithms
- [[GNSS-Terminology]] - Satellite navigation fundamentals
- [[Safety-Terminology]] - Safety requirements and integrity
- [[ICAO-SBAS-Standards-Library.md]] - Regulatory specifications
- [[MOCs/SBAS-Research-MOC.md]] - Research overview
- [[MOCs/SBAS-in-Civil-Aviation-MOC.md]] - Operational applications
- [[MOCs/SBAS-Systems-by-Region-MOC.md]] - Regional implementations
- [[Standards-Regulation/SBAS-Standards-Regulation.md]] - Standards
- [[Standards-Regulation/SBAS-vs-Other-Standards.md]] - Standards comparison

--
*Node: SBAS-Terminology | Links: 10+ | Depth: 1 | Status: Active*

### **LPV (Localizer Performance with Vertical)**
Category A precision approach utilizing SBAS for lateral and vertical guidance. Provides 0.8m horizontal and 15m vertical accuracy without traditional ILS infrastructure.
