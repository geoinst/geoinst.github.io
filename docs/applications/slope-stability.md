---
lang: en
lang_alt: vi/applications/slope-stability/
---
# Slope Stability Monitoring

## Objective

Detect the onset of slope movement before failure, identify the shear surface, and quantify the rate of movement to inform early-warning and remediation.

---

## Comprehensive Chapter References from Reference Manuals

### From Dunnicliff — Geotechnical Instrumentation for Monitoring Field Performance
| Chapter | Title | Application to Slope Stability |
|---------|-------|--------------------------------|
| **Ch 1** | Geotechnical Instrumentation: An Overview | Importance of slope monitoring, failure consequences |
| **Ch 2** | Behavior of Soil and Rock | Shear strength, failure mechanisms, soil/rock behavior |
| **Ch 3** | Benefits of Using Geotechnical Instrumentation | Early warning, design verification, legal protection |
| **Ch 4** | Systematic Approach to Planning Monitoring Programs | 20-step planning process specific to slopes |
| **Ch 9** | Measurement of Groundwater Pressure | Piezometers for pore pressure triggering failure |
| **Ch 12** | Measurement of Deformation | Inclinometers, extensometers, tiltmeters, settlement systems |
| **Ch 17** | Installation of Instruments | Drilling, grouting, casing installation in slopes |
| **Ch 18** | Collection, Processing, Presentation, Interpretation | Data collection frequency, automated systems, interpretation |
| **Ch 19** | Braced Excavations | Strut loads, wall deflection, ground movement, groundwater |
| **Ch 22** | **Excavated and Natural Slopes** | **Primary chapter for slopes** — inclinometers, piezometers, tiltmeters, surface survey |

### From Foundation Engineering: A Public-Domain Reference (USACE / FHWA)
| Chapter | Title | Application |
|---------|-------|-------------|
| **Ch 13** | Slope Stability | Infinite/finite slopes, method of slices, factor of safety |
| **Ch 10** | Lateral Earth Pressure | Rankine/Coulomb, active/passive pressures on slopes |
| **Ch 11** | Retaining Walls & MSE Walls | Stabilizing structures at slope toes |
| **Ch 12** | Sheet Pile Walls & Braced Excavations | Excavation support on slopes |

### From Soil Mechanics & Geotechnical Engineering: A Public-Domain Reference (USACE / FHWA)
| Chapter | Title | Application |
|---------|-------|-------------|
| **Ch 6** | Seepage & Flow Nets | Seepage forces, slope drainage |
| **Ch 7** | Effective Stress & Pore Pressure | Pore pressure effects on effective stress |
| **Ch 10** | Shear Strength | Mohr-Coulomb, triaxial tests, CU/CD, pore pressure parameters |
| **Ch 13** | Problem Soils | Expansive and collapsible soils on slopes |

---

## Typical Instrument Array for Slope Stability

| Instrument | Purpose | Dunnicliff Chapter | Representative Instrument |
|------------|---------|-------------------|------------------------|
| **In-place inclinometer (IPI) array** | Continuous profile of lateral movement | Ch 12, 22 | MEMS IPI, wireless IPI |
| **Vibrating-wire piezometers** | Pore water pressure triggering failure | Ch 9, 22 | VW piezometers, wireless piezometer nodes |
| **Surface tiltmeters** | Catch the upper edge of a moving mass | Ch 12, 22 | MEMS tiltmeters, wireless tilt arrays |
| **Surface survey points / GPS** | Surface displacement monitoring | Ch 12, 22 | Locator One GNSS, wireless mesh radio |
| **Crackmeters / jointmeters** | Discrete crack/joint opening | Ch 12 | Crackmeters, jointmeters |
| **wireless mesh radio** | Brings sensor data back to alert gateway | Ch 8, 18 | wireless mesh radio |

---

## Installation Guidelines (from Dunnicliff Ch 9, 12, 17, 22)

### Inclinometer Installation
- Casing: ABS or aluminum, grooved (4-groove standard)
- Grouting: Cement-bentonite grout, tremie method
- Initial readings: Establish baseline within 24 hrs
- Reading frequency: Daily (construction), weekly (monitoring), monthly (long-term)

### Piezometer Installation
- Filter tip: Saturated, compatible with formation
- Seal: Bentonite above/below filter zone
- Saturation: VW piezometers per Ch 9 procedure
- Cable routing: Protected, strain-relieved

### Tiltmeter Installation
- Mount: Stable concrete pad or bedrock
- Orientation: Perpendicular to anticipated movement
- Temperature compensation: Required for MEMS

---

## Data Interpretation Guidelines (from Dunnicliff Ch 18, 22)

| Parameter | Threshold/Action Level | Reference |
|-----------|------------------------|-----------|
| Inclinometer displacement rate | > 5 mm/day = alert; > 20 mm/day = evacuation | Ch 22 |
| Pore pressure increase | > 80% of design value = alert | Ch 22 |
| Tilt rate | > 0.1°/day = alert | Ch 22 |
| Crackmeter opening rate | > 1 mm/day = alert | Ch 22 |

---

## Related Pages
- [Dunnicliff Chapter 22](../reference-manuals/dunnicliff/chapter-14-applications.md)
- [GTI Doctor — Ask about slope monitoring](../gti-doctor.md)

---

*Source: Compiled from Dunnicliff (616 chunks), Foundation Engineering (USACE/FHWA, public domain), Soil Mechanics (USACE/FHWA, public domain), NCHRP Synthesis 89, and field reference manuals.*
