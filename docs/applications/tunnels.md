---
lang: en
lang_alt: vi/applications/tunnels/
---
# Tunnel Instrumentation

## Objective

Monitor ground movement around tunnel excavation, convergence of linings, and pore-pressure changes during construction — protecting both the tunnel cross-section and adjacent structures above.

---

## Comprehensive Chapter References from Reference Manuals

### From Dunnicliff — Geotechnical Instrumentation for Monitoring Field Performance
| Chapter | Title | Application to Tunnel Instrumentation |
|---------|-------|----------------------------------------|
| **Ch 1** | Geotechnical Instrumentation: An Overview | Importance of tunnel monitoring, collapse consequences |
| **Ch 2** | Behavior of Soil and Rock | Rock mass behavior, squeezing ground, rockburst |
| **Ch 3** | Benefits of Using Geotechnical Instrumentation | Design verification, construction safety, contractual |
| **Ch 4** | Systematic Approach to Planning Monitoring Programs | 20-step planning for tunnel projects |
| **Ch 8** | Instrumentation Transducers & Data Acquisition | Convergence sensors, automated systems |
| **Ch 9** | Measurement of Groundwater Pressure | Dewatering pressures, piezometers at tunnel face |
| **Ch 12** | **Measurement of Deformation** | **Primary** — Convergence, extensometers, inclinometers |
| **Ch 13** | Measurement of Load and Strain | Rock bolt loads, lining stress, telltales |
| **Ch 17** | Installation of Instruments | Tunnel-specific: drilling from tunnel, limited space |
| **Ch 18** | Collection, Processing, Presentation, Interpretation | Real-time convergence monitoring, alarm systems |
| **Ch 23** | **Underground Excavations** | **Primary chapter for tunnels** — convergence, rock bolts, groundwater, face pressure |

### From Foundation Engineering: A Public-Domain Reference (USACE / FHWA)
| Chapter | Application |
|---------|-------------|
| **Ch 10** | Lateral Earth Pressure — tunnel lining design |
| **Ch 12** | Sheet Pile Walls & Braced Excavations — portal and cut-and-cover support |
| **Ch 13** | Slope Stability — portal slopes, surface settlement |

### From Soil Mechanics & Geotechnical Engineering: A Public-Domain Reference (USACE / FHWA)
| Chapter | Application |
|---------|-------------|
| **Ch 6** | Seepage & Flow Nets — groundwater inflow, face pressure |
| **Ch 7** | Effective Stress & Pore Pressure — ground response around openings |
| **Ch 10** | Shear Strength — rock mass and soil strength parameters |

---

## Typical Instrument Array for Tunnel Instrumentation

| Instrument | Purpose | Dunnicliff Chapter | Representative Instrument |
|------------|---------|-------------------|------------------------|
| **Convergence arrays / tape extensometers** | Monitor tunnel cross-section closure | Ch 12, 23 | Tape extensometers, convergence arrays |
| **Multi-point borehole extensometers (MPBX)** | Rock mass displacement above crown | Ch 12, 23 | MPBX extensometers, wireless |
| **Inclinometers (surface/portal)** | Detect surface settlement trough | Ch 12, 23 | MEMS inclinometers, IPI arrays |
| **Piezometers** | Dewatering pressures near tunnel face | Ch 9, 23 | VW piezometers, wireless |
| **Rock bolt load cells** | Anchor/bolt load monitoring | Ch 13, 23 | VW load cells, strain gages |
| **Convergence meters** | Real-time lining convergence | Ch 12, 23 | Convergence meters, wireless |
| **Rock bolt strain gages** | Bolt load monitoring | Ch 13 | VW strain gages, wireless |
| **Pressure cells (NATM)** | Ground pressure on lining | Ch 10, 23 | VW pressure cells |
| **Crackmeters / jointmeters** | Segment joint opening | Ch 12, 23 | Crackmeters, jointmeters |
| **Inclinometer (TBM shield)** | TBM articulation/alignment | Ch 12 | MEMS tilt sensors |
| **wireless mesh radio** | Data from tunnel to surface gateway | Ch 8, 18 | wireless mesh + surface gateway |

---

## Installation Guidelines (from Dunnicliff Ch 12, 17, 23)

### Convergence Monitoring
- **Array types**: Tape extensometer, convergence meter, MPBX
- **Locations**: Crown, springlines, invert
- **Frequency**: Daily (excavation), weekly (construction), monthly (operation)

### Extensometer Installation (MPBX)
- **Anchor depths**: Multiple anchors at varying rock cover depths
- **Installation**: From tunnel crown/drilling from surface
- **Reference head**: Stable location outside tunnel influence zone

### Piezometer Installation
- **Locations**: Ahead of face, at face, behind lining
- **Types**: VW piezometers for remote reading
- **Dewatering monitoring**: Upstream/downstream of tunnel

### Rock Bolt Monitoring
- **Load cells**: Installed at bolt head
- **Strain gages**: Bonded to bolt shank
- **Tell-tales**: For long bolt elongation

---

## Data Interpretation Guidelines (from Dunnicliff Ch 18, 23)

| Parameter | Normal Range | Alert Level | Critical Level | Reference |
|-----------|--------------|-------------|----------------|-----------|
| Convergence rate | < 2 mm/day | > 5 mm/day | > 10 mm/day | Ch 23 |
| Crown settlement rate | < 2 mm/day | > 5 mm/day | > 10 mm/day | Ch 23 |
| Rock bolt load loss | < 10% | > 20% | > 30% | Ch 13 |
| Pore pressure change | Baseline | 2× baseline | > design value | Ch 9, 23 |
| Rock bolt load loss rate | < 5%/mo | > 10%/mo | > 20%/mo | Ch 13 |

---

## Automated Monitoring for Tunnels (Dunnicliff Ch 18, Ch 23)

| System | Function | Implementation |
|--------|----------|-------------------|
| **Real-time convergence** | Continuous crown/springline monitoring | wireless convergence sensors |
| **Face pressure monitoring** | TBM shield pressure, dewatering | wireless piezometers |
| **Rock bolt monitoring** | Bolt load + strain | VW load cells + strain gages |
| **Automated alarms** | Threshold exceedance | cloud platform |
| **TBM data integration** | Shield pressure, articulation | wireless mesh + TBM interface |

---

## Related Pages
- [Dunnicliff Chapter 23](../reference-manuals/dunnicliff/chapter-14-applications.md)
- [GTI Doctor — Ask about tunnel monitoring](../gti-doctor.md)

---

*Source: Compiled from Dunnicliff (616 chunks), Foundation Engineering (USACE/FHWA, public domain), Soil Mechanics (USACE/FHWA, public domain), NCHRP Synthesis 89, and field reference manuals.*
