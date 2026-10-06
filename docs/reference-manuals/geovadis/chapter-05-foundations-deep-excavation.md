---
lang: en
lang_alt: vi/reference-manuals/geovadis/chapter-05-foundations-deep-excavation/
---

# Foundations, Deep Excavations and Retaining Systems

!!! abstract "Session Summary"
    Session 4 of *GeoVadis (GAIC 2025)* encompasses critical advances across foundation systems, deep excavations, and earth retaining structures. Contributions examine piled raft performance under combined vertical-lateral (V-H) loads, soil-cement composite piles, trench stability in diaphragm walls with enlarged panels, bi-directional static load testing (BDSLT), deep soil mixing with steel insertions for 10-meter cut slopes, and thermal behavior of energy micropile arrays.

---

## 1. Piled Raft Foundations Under Combined V-H Loading (A. Garg, V.A. Sawant, S. Mehndiratta)

### 3D Finite Element Interaction Mechanics
Tall structures, bridge towers, and wind turbine jackets impose severe concurrent vertical ($V$), horizontal ($H$), and moment ($M$) loads on piled rafts. Garg et al. conduct coupled 3D elastoplastic FE simulations to analyze load-sharing between raft base and pile group:
- **Raft-Soil Contact Mobilization:** Under pure vertical loads, the raft transmits $30\% - 45\%$ of total gravity loads directly to surface soil. Under high lateral shear ($H/V > 0.2$), raft base shear friction engages rapidly, shedding up to $40\%$ of horizontal demand before significant lateral pile deflection mobilizes.
- **Pile Group P-y Softening:** Cyclic lateral displacement induces soil plastic yielding in the top $3D - 5D$ pile depth, diminishing pile group lateral stiffness by $25\% - 35\%$.
- **Design Guidelines:** Optimizing pile length distribution (longer central settlement-reducing piles, stiffer perimeter shear-resisting piles) minimizes raft differential settlement and perimeter cracking.

---

## 2. Soil-Cement Composite Piles (S. Koga, K. Watanabe, T. Naito, N. Tsuchiya)

### Concept & Centrifuge Modeling
Soil-cement composite piles comprise a rigid precast concrete core or steel pipe inserted concentric to an outer deep-mixed soil-cement column. Koga and Watanabe utilize geotechnical centrifuge testing ($50g$) and full-scale 1g models to elucidate vertical and lateral load-transfer mechanisms:

```
        Vertical Load P
              │
              ▼
    ┌───────────────────┐
    │ Concrete/Steel    │ ◄─── High Axial Stiffness Core (Ec)
    │ Core Pile         │
    │                   │
    ├─┬───────────────┬─┤
    │ │ Soil-Cement   │ │ ◄─── Enlarged Column Shell (E_sc, D_col)
    │ │ Outer Shell   │ │      Expands Bearing Perimeter & Tip Area
    ├─┼───────────────┼─┤
    │ │               │ │
    │ │ Soil Shear    │ │ ◄─── High Frictional Mobilization across
    │ │ Resistance    │ │      Rough Soil-Cement/Ground Interface
    └─┴───────────────┴─┘
```

### Key Mechanical Insights
1. **Vertical Load Transfer:** Axial stress is initially borne by the high-modulus inner core, then transferred progressively into the soil-cement shell via core-grout interface friction. The enlarged base diameter ($D_{col} = 2 - 3 \times D_{core}$) expands the end-bearing area by $400\% - 900\%$.
2. **Lateral Resistance:** Under horizontal loads, the outer soil-cement column mobilizes high passive resistance in the upper strata, reducing pile head lateral deflection by over $50\%$ compared to a bare precast pile.

---

## 3. Trench Stability in Diaphragm Walls with Enlarged Panels (A. Iwata, K. Watanabe, T. Watanabe)

### Diaphragm Walls with Enlarged T- and Cross-Shaped Panels
To resist massive bending moments in ultra-deep urban excavations, diaphragm walls often incorporate enlarged flange panels (T-panels, cruciform panels). However, the increased trench surface area elevates the risk of slurry trench collapse during excavation:
- **Slurry Pressure Maintenance:** 3D limit equilibrium and finite element analyses indicate that hydrostatic slurry head must exceed the phreatic groundwater table by at least $1.5\,\text{m}$ to prevent localized inward plastic sloughing at re-entrant corners.
- **Polymer vs. Bentonite Slurry:** Polymer slurries with viscoelastic modifiers maintain superior rheological stability and filter cake continuity across variable sand-gravel lenses, preventing slurry loss and collapse.

---

## 4. Deep Soil Mixing with Steel Insertion for 10m Excavation Support (Z.W. He, J. Si, K.W. Leong)

### Retaining System for Constrained Urban Sites
He et al. present a successful design and field monitoring case history for a 10-meter deep basement excavation in sensitive urban clay:
- **System Architecture:** Overlapping triple-shaft deep mixed soil-cement columns ($D = 850\,\text{mm}$) reinforced with inserted structural steel H-beams (SMW method) installed at alternating column centers.
- **Tieback Anchoring:** Two levels of prestressed ground anchors drilled through the composite wall provide lateral restraint.
- **Field Performance:** Inclinometer measurements recorded a maximum lateral retaining wall deflection of only $18\,\text{mm}$ ($< 0.2\% H$), well within the allowable serviceability limit for adjacent building protection.

---

## 5. Bi-Directional Static Load Pile Testing (BDSLT) (A.K. Chakraborti, S.K. Golchha, A. Uppadhyay)

### Osterberg Cell (BDSLT) Testing of High-Capacity Bored Piles
Conventional top-down static load tests on deep bored piles ($Q_{ult} > 25,000\,\text{kN}$) require colossal reaction kentledge or tension anchor piles, posing severe safety and cost challenges. Chakraborti et al. evaluate deep bored pile tests using hydraulically expandable Osterberg cells (O-cells) embedded at the pile bottom:
- **Self-Balancing Principle:** The O-cell pushes upward against the upper shaft skin friction while simultaneously pushing downward against pile tip end-bearing and lower shaft friction.
- **Equivalent Top-Load Curve:** Using the Schmertmann / O-cell synthesis method, upward and downward load-movement curves are combined into an equivalent conventional top-load movement curve:
  $$S_{top}(Q) = S_{up}(Q_{shaft}) + S_{elastic\_shortening}$$
- **Strain Gauge Instrumentation:** Multi-level sister bars installed throughout the pile shaft accurately delineate unit shaft friction ($f_s$) degradation along stratified clay-shale strata.

---

## 6. Excavation and Foundation Instrumentation Summary

| Subsurface Structure | Primary Diagnostic Sensor | Secondary Sensor | Key Engineering Parameter |
| :--- | :--- | :--- | :--- |
| **Piled Raft Foundation** | Earth Pressure Cells (Raft base) | Pile Head Vibrating Wire Strain Gauges | Raft/pile load sharing ratio, contact pressure |
| **Diaphragm Wall (H-beam / Barrette)** | Inclinometer Casing (Within wall) | Load Cells on Anchor Heads | Lateral deflection profile, anchor load loss |
| **Deep Excavation Ground Response** | Multi-Point Magnetic Extensometers | Surface Tiltmeters on Adjacent Structures | Subsurface vertical ground settlement profile |
| **BDSLT / O-cell Pile Test** | Displacement Transducers across Cell | Multi-Level Sister Bars in Cage | Upward/downward stroke, unit skin friction $f_s$ |
| **Deep Soil Mixing (SMW Wall)** | Inclinometers in Steel H-beams | Vibrating Wire Piezometers behind Wall | Wall deflection, groundwater drawdown |
