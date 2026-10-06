---
lang: en
lang_alt: vi/reference-manuals/geovadis/chapter-03-cold-coastal-environmental/
---

# Cold, Coastal and Environmental Geotechnical Engineering

!!! abstract "Session Summary"
    Session 2 of *GeoVadis (GAIC 2025)* tackles geopolitical and environmental challenges at the interface of geotechnics, climate change, and waste isolation. Core contributions explore freeze-thaw degradation in alpine terrains, digital image analysis of clay desiccation cracking, bentonite swelling under extreme chemical and thermal gradients, field porewater pressure monitoring during vacuum preloading, and shallow geothermal storage in unsaturated formations.

---

## 1. Freeze-Thaw Mechanics in Seasonally Frozen Soils (C. Tagar, A. Kalita, A. Dey)

### High-Altitude Infrastructure Vulnerability
Infrastructure constructed at high altitudes (such as the Sela Tunnel at 4,200 m elevation in Arunachal Pradesh, India) faces severe seasonal thermal cycling. Tagar et al. conduct multi-cycle freeze-thaw tests (temperatures cycling between $-15^\circ\text{C}$ and $+20^\circ\text{C}$) on natural subgrade soils:
- **Pore Structure Alteration:** Cryogenic ice lensing expands existing micro-pores during freezing. Subsequent thawing leaves enlarged void ratios ($e$) and breaks inter-particle cementing bonds.
- **Unconfined Compressive Strength ($q_u$) Degradation:** Strength drops exponentially over the first 5 cycles, losing up to 45% of pristine virgin strength before reaching an asymptotic residual plateau.
- **Resilient Modulus ($M_R$):** Cyclic triaxial testing confirms substantial reduction in subgrade stiffness, explaining premature rutting and fatigue cracking on alpine highway corridors.

---

## 2. Desiccation Cracking in Compacted Clay (S. Majumder, B.K. Agarwal, A. Sachan)

### Digital Image Analysis (DIA) & Digital Image Correlation (DIC)
Desiccation cracking impairs the hydraulic integrity of landfill clay liners, canal embankments, and earth dam cores. Majumder et al. deploy high-resolution optical tracking coupled with DIC strain mapping to monitor crack initiation and propagation during continuous drying:
- **Tensile Strain Threshold:** Cracks initiate when localized tensile strains exceed the tensile strain capacity ($\epsilon_{t,lim} \approx 1.2\% - 1.8\%$) at cell boundaries.
- **Crack Intensity Factor (CIF):** Quantified as the ratio of surface crack area to total specimen area ($CIF = A_{crack} / A_{total}$).
- **Suction Boundary:** Cracking initiates precisely when matric suction approaches the air-entry value ($AEV$), triggering water meniscus retreat into sub-surface pores.

```
       Moisture Evaporation (Drying) ──► Meniscus Recedes into Pores
                                           │
                                           ▼
       Matric Suction Increases (ψ = ua - uw) ──► Capillary Tension Builds
                                           │
                                           ▼
       Tensile Stress Exceeds Soil Tensile Strength (σ_t > f_t)
                                           │
                                           ▼
       Crack Inception at Desiccation Flaws ──► DIC Detects Strain Localization
                                           │
                                           ▼
       Crack Network Interconnection ──► CIF Jumps, Permeability Increases 100x
```

---

## 3. Swelling & Infiltration of Bentonite Buffers (D. Ito, N. Yamada, H. Wang, H. Komine)

### Deep Geological Repositories for Radioactive Waste
Compacted bentonite-sand mixtures serve as engineered barriers isolating high-level nuclear waste canisters. Ito et al. investigate how cation exchange ($Na^+$ vs. $Ca^{2+}$) and saline groundwater ingress alter buffer swelling pressure ($p_s$) and hydraulic conductivity ($k$):
- **Cation Valency Impact:** Saline groundwater containing divalent ions ($Ca^{2+}, Mg^{2+}$) compresses the diffuse double layer (DDL), reducing free swell volume by over 60% compared to deionized water.
- **Self-Sealing Capacity:** Despite salinization, compacted sodium bentonite retains sufficient swelling pressure ($p_s > 2\,\text{MPa}$) at dry densities $\rho_d \ge 1.6\,\text{g/cm}^3$ to seal construction joints and thermal cracks.
- **Coupled Thermal Influence (T. Nishimura):** Under elevated temperatures ($T = 60^\circ\text{C} - 80^\circ\text{C}$), suction-controlled swelling tests reveal accelerated water redistribution and thermal vapor migration away from heat sources.

---

## 4. Vacuum Preloading Consolidation: Fisherman Island Case Study (L. Karagoz, B. Indraratna, et al.)

### Field Verification of Vacuum-Assisted Consolidation
At the Port of Brisbane (Fisherman Island, Australia), reclamation over deep, ultra-soft marine clays required combined vacuum preloading with Prefabricated Vertical Drains (PVDs). Karagoz and Indraratna analyze comprehensive field monitoring data:
- **Vacuum Negative Pressure Distribution:** A sustained negative pore pressure of $-70\,\text{kPa}$ to $-80\,\text{kPa}$ is applied beneath the airtight geomembrane, propagating along PVDs to a depth of $20\,\text{m}$.
- **Effective Stress Equivalence:** Unlike physical surcharge fills that increase total stress ($\Delta \sigma$), vacuum pressure directly induces negative pore pressure ($-\Delta u$), generating an isotropic effective stress increase ($\Delta \sigma' = -\Delta u$) without inducing shear failure or outward lateral squeezing at the embankment toe.
- **Porewater Pressure Dissipation Profiling:** Vibrating wire piezometers installed at depths of $3\,\text{m}$, $8\,\text{m}$, $14\,\text{m}$, and $19\,\text{m}$ demonstrate accelerated radial consolidation matching 90% primary consolidation within 120 days.

---

## 5. Optimization of Shallow Geothermal Energy Storage (A. Deshmukh, A.J. Puppala, X. Yu, et al.)

### Underground Thermal Energy Storage (UTES)
Deshmukh et al. demonstrate that unsaturated clay formations possess ideal thermal inertia for seasonal heat storage:
- **Thermo-Hydraulic Coupling:** Heat injection increases ground temperature while driving pore moisture away from borehole heat exchangers (BHE), causing localized desaturation and reducing effective thermal conductivity ($\lambda$).
- **Heuristic Optimization:** Genetic algorithms (GA) optimize borehole spacing ($S/D = 4 - 6$) and flow rates, achieving thermal storage round-trip efficiencies exceeding 72% over annual heating/cooling cycles.

---

## 6. Environmental Geotechnics Field Monitoring Sensor Suite

| Engineering System | Primary Sensor / Diagnostic | Secondary Sensor | Target Measured Quantity |
| :--- | :--- | :--- | :--- |
| **Alpine Road Subgrade** | Time-Domain Reflectometry (TDR) | Multi-Depth Thermistor String | Freezing front depth, unfrozen water content |
| **Clay Landfill Barrier** | High-Capacity Tensiometers | In-Situ Electrical Resistivity | Matric suction ($\psi$), crack onset, leachate ingress |
| **Nuclear Waste Bentonite** | Miniature Total Pressure Cells | Psychrometers + Thermocouples | Swelling pressure ($p_s$), suction, temperature ($T$) |
| **Vacuum Preloading Site** | Vibrating Wire Piezometers | Profiler Gauges + Magnetic Extensometers | Negative pore pressure ($u$), subsurface settlement |
| **Geothermal Borehole Array**| Fiber-Optic DTS Cable | Flow Meters + Heat Flux Sensors | Continuous temperature log, heat injection rate |
