---
lang: en
lang_alt: vi/reference-manuals/geovadis/chapter-06-geosynthetic-engineering/
---

# Geosynthetics, Reinforced Soil and Ground Improvement

!!! abstract "Session Summary"
    Session 5 of *GeoVadis (GAIC 2025)* covers geosynthetics, reinforced soil structures, and innovative soil improvement technologies. Key themes include micromechanical interface friction, pullout mechanics of overlapping geogrids, seismic and rainfall stability of reinforced soil walls (RSW) with geocell fascia, geotextile tube dewatering of industrial tailings, and real-world highway and hydropower penstock slope stabilization.

---

## 1. Pullout Mechanics of Overlapping Geogrids (A.O.A. Mohammed, B.K.K. Prabhakara, U. Balunaini)

### The Overlap Joint in Reinforced Soil Construction
In large-scale mechanically stabilized earth (MSE) walls and highway embankments, geogrid rolls must be spliced or overlapped due to finite roll lengths. Mohammed et al. conduct large-scale pullout tests and discrete numerical simulations to quantify pullout resistance factors ($F^*$):
- **Spread Ratio ($S_r$):** Defined as the ratio of overlapping aperture alignment. When transverse ribs align directly ($S_r = 1.0$), passive bearing resistance against front transverse ribs mobilizes synchronously.
- **Minimum Overlap Length ($L_o$):** Splicing without mechanical connectors requires a minimum overlap length of $1.0\,\text{m} - 1.5\,\text{m}$ to prevent slippage prior to reaching the geogrid ultimate tensile strength ($T_{ult}$).
- **Interface Shear Efficiency ($\alpha$):** The apparent coefficient of friction $f^* = \tau / \sigma'_n$ achieves $0.85 - 0.95$ of virgin single-sheet geogrid values, provided backfill compaction is rigorously controlled.

---

## 2. Reinforced Soil Walls with Geocell Fascia (R. Ahamad, A. Shelke, S. Khan)

### Cellular Confinement Fascia vs. Concrete Panels
Rigid concrete fascia panels in MSE walls often suffer from differential settlement, aesthetic cracking, and high embodied carbon. Ahamad et al. explore 3D cellular confinement systems (geocells) stacked as flexible fascia units:
- **Confinement Mechanism:** Geocell pockets filled with granular soil or recycled aggregate create an integrated gravity facing unit that accommodates large differential settlements ($> 5\%$) without structural distress.
- **Dynamic Response:** Under earthquake shaking, the flexible geocell fascia dissipates energy through cyclic inter-cell friction, attenuating wall face accelerations by up to $30\%$ compared to rigid modular concrete block walls.
- **Vegetative Potential:** The exposed geocell pockets can be hydroseeded to establish living green facades, mitigating urban heat island effects and enhancing surface erosion control.

---

## 3. Centrifuge Modeling of RSW Subjected to Extreme Rainfall (V.V. Turlapati, B.V.S. Viswanadham)

### Pore Pressure Buildup in Reinforced Soil Backfill
Rainfall-induced failures represent the most common collapse mode for reinforced soil walls worldwide. Turlapati and Viswanadham test model walls at $30g$ in a geotechnical centrifuge equipped with an inflight rainfall simulator:
- **Drainage Layer Deficiency:** In the absence of an internal chimney drain or permeable drainage composite, perched water tables develop rapidly behind the wall face during high-intensity storms ($100\,\text{mm/hr}$ prototype equivalent).
- **Transient Suction Loss:** The advance of the wetting front destroys apparent cohesion ($c = \psi \tan\phi^b$), shifting lateral earth pressures from active state ($K_a$) to hydrostatic saturated state, drastically increasing geogrid tensile forces.
- **Deformation Mode:** Centrifuge imaging captures progressive outward bulging and toe rotation, underscoring that permeable non-woven geotextile-drain composites are essential along reinforcement layers in marginal backfills.

```
       Extreme Rainfall Precipitation
       │   ▼        ▼        ▼        ▼
       ▼───────────────────────────────────────┐
       │ Infiltration Wetting Front Advances   │
       │   - Matric suction ψ drops to 0       │
       │   - Apparent cohesion c' vanishes     │
       │═══════════════════════════════════════│
       │ Perched Water Table / Positive Δu     │
       │   - Total lateral thrust increases    │
       │   - Effective shear resistance drops  │
       └───────────────────┬───────────────────┘
                           │
                           ▼
       Geogrid Reinforcement Tension Surges ──► Wall Toe Bulging & Rotational Creep
       (Remedy: Non-woven Geotextile Chimney Drains & Drainage Strips)
```

---

## 4. Dewatering Low-Solid Wastes with Geotextile Tubes (G.F. Segré Quilichini, S.K. Bhatia; N. Budhai)

### Slurry Volume Reduction & Tailings Management
Dredged river sediments, mining tailings, and municipal sludge feature high moisture content ($> 80\%$) and low solids. Geotextile tubes—large permeable tubes fabricated from high-strength woven polypropylene geotextiles—offer an efficient dewatering solution:
- **Chemical Conditioning:** Rapid flocculation via polymer dosing aggregates fine silt and clay particles into stable flocs, preventing premature geotextile blinding and filter pore clogging.
- **Filtration Efficiency:** Over $98\%$ of suspended solids are retained inside the tube, while clarified effluent discharges freely through geotextile pores.
- **Consolidation and Densification:** Within 30 to 90 days, sludge moisture drops below $35\%$, transforming semi-fluid slurry into dry consolidated cakes suitable for beneficial reuse or safe dry-stack landfilling.

---

## 5. Hydropower Penstock Slope Stabilization: Middle Tamor Project (M. Rijal, R. Mahajan, et al.)

### Extreme Himalayan Terrain Stabilization
At the 73 MW Middle Tamor Hydropower Project in Nepal, steep penstock alignment slopes suffered severe slope instability in jointed phyllite and colluvium:
- **Hybrid Support System:** High-strength polyester geogrids ($T_{ult} \ge 200\,\text{kN/m}$) combined with self-drilling rock anchors and flexible wire-mesh facing.
- **Erosion & Runoff Control:** Biodegradable coir mats installed across surface terraces prevented gully erosion and promoted re-vegetation during the monsoon season.
- **Monitoring Results:** Surface displacement pins and inclinometer casings verified complete stabilization throughout two subsequent monsoon seasons.

---

## 6. Geosynthetics & Ground Improvement Field Sensor Checklist

| Geosynthetic Application | Primary Structural Sensor | Environmental / Hydraulic Sensor | Key Verification Parameter |
| :--- | :--- | :--- | :--- |
| **Geogrid Reinforced Soil Wall** | High-Elongation Strain Gauges on Geogrid | Earth Pressure Cells behind Wall Fascia | Reinforcement tensile strain ($\epsilon$), lateral earth pressure |
| **Centrifuge Rainfall Testing** | Miniature Pore Pressure Transducers (PPT) | Laser Displacement Sensors (LDS) | Wetting front pore pressure ($\Delta u$), wall face deflection |
| **Geotextile Dewatering Tube** | Pressure Transducers inside Port | Turbidity Sensor on Discharging Effluent | Pumping fill pressure ($p_{fill}$), effluent total suspended solids |
| **Penstock Slope Reinforcement** | Anchor Head Load Cells | Inclinometer Casings in Slope | Residual anchor prestress, deep slip movement |
| **Encased Granular Piles** | Multi-Depth Settlement Plates | Vibrating Wire Piezometers in Soft Clay | Consolidation settlement, excess pore pressure dissipation |
