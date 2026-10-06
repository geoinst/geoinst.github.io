---
lang: en
lang_alt: vi/reference-manuals/geovadis-vol2/chapter-01-ground-improvement-stabilisation/
---

# Ground Improvement and Chemical Stabilisation

!!! abstract "Session Summary"
    Session 6 of *GeoVadis (GAIC 2025)* addresses modern ground improvement, chemical stabilization, and bio-geochemical soil remediation. Key contributions explore subgrade mud pumping and fluidization mitigation under heavy-haul rail traffic, geopolymer-soil column supported embankments, carbon nanotubes for liquefaction prevention, non-linear vertical drain preloading design charts, and microbially induced calcite precipitation (MICP).

---

## 1. Subgrade Fluidization Mitigation Under Cyclic Rail Loading (B-H. Xu, C. Rujikiatkamjorn, B. Indraratna, et al.)

### The Mud Pumping / Subgrade Fluidization Dilemma
Under high-speed and heavy-haul freight rail traffic (axle loads $\ge 30\,\text{tonnes}$), repetitive cyclic stresses generate high excess pore water pressures ($\Delta u$) in saturated soft subgrade clays. When effective stress approaches zero ($\sigma' \to 0$), fine clay particles detach and form a fluidized soil-water slurry that pumps upward into the overlying ballast, causing severe track geometry degradation, differential track settlement, and ballast fouling:

```
        High Cyclic Train Axle Loads (30 - 35 tonnes)
                          │
                          ▼
        ┌───────────────────────────────────┐
        │ Ballast & Subballast Layers       │
        ├───────────────────────────────────┤
        │ Saturated Soft Subgrade Clay      │
        └─────────────────┬─────────────────┘
                          │
       Cyclic Shear Stress Cycles (N > 100,000)
                          ▼
        ┌───────────────────────────────────┐
        │ Rapid Excess Pore Pressure Build  │
        │ Effective Stress σ' ──► 0         │
        │ Subgrade Fluidization / Slurry    │
        └─────────────────┬─────────────────┘
                          │
       Slurry Pumps Upward Through Ballast Voids
                          ▼
        Track Geometry Failure & Rapid Settlement
        (Remedy: Chemical-Biopolymer Capping + Under-Ballast Drainage Mat)
```

### Advanced Constitutive Formulation & Mitigation
Professor Indraratna's team develops a cyclic elastoplastic fluidization model incorporating inter-particle hydraulic drag and cyclic degradation. They validate that deploying an engineered capping layer treated with biopolymers or prefabricated vertical drains accelerates pore pressure dissipation, bounding the cyclic pore pressure ratio ($r_u < 0.35$) and completely suppressing mud pumping.

---

## 2. Geopolymer-Soil Column Supported Embankments (S. Gupta, S. Kumar)

### Sustainable Alkali-Activated Soil Columns
Ordinary Portland cement (OPC) manufacturing is responsible for roughly $8\%$ of global $\text{CO}_2$ emissions. Gupta and Kumar evaluate fly ash and ground granulated blast-furnace slag (GGBS) activated with alkali solutions (sodium silicate and sodium hydroxide) to construct deep soil columns supporting highway embankments:
- **Unconfined Compressive Strength ($q_u$):** Geopolymer columns achieve $28$-day compressive strengths of $3.5\,\text{MPa} - 6.2\,\text{MPa}$, comparable or superior to conventional cement deep soil mixing (CDSM).
- **Embankment Load Transfer (Arching):** Numerical 3D PLAXIS simulations confirm that geopolymer columns effectively mobilize soil arching within the embankment granular fill, transferring over $75\%$ of the embankment weight directly to the competent bearing stratum.

---

## 3. Carbon Nanotubes (CNTs) for Sand Liquefaction Mitigation (S. Shaswat, R.P. Orense)

### Nano-Engineering of Granular Contacts
Shaswat and Orense investigate the micro-mechanical reinforcement of loose clean sands using multi-walled carbon nanotubes (MWCNTs) dispersed at low dosages ($0.05\% - 0.20\%$ by dry weight):
- **Contact Bridging Mechanism:** The high aspect ratio ($> 1,000$) and exceptional tensile modulus ($> 1\,\text{TPa}$) of CNTs create flexible nanoscale tensile bridges across adjacent quartz grains.
- **Cyclic Resistance:** Cyclic triaxial tests demonstrate that adding just $0.1\%$ MWCNTs increases the cyclic resistance ratio ($CRR_{20}$) by $65\%$, significantly retarding cyclic strain accumulation without impairing hydraulic drainage.

---

## 4. Non-Linear Consolidation Design Curves for Vertical Drains (K. Kharsyiemiong, V.A. Sawant, S. Mittal)

### Overcoming Linear Assumptions in Preloading Design
Classical Barron and Hansbo solutions assume constant permeability ($k_h$) and constant volume compressibility ($m_v$) during consolidation. In thick marine clay deposits, both permeability and compressibility decrease by orders of magnitude as void ratio decreases ($e - \log k$ and $e - \log \sigma'$ non-linearity).

Kharsyiemiong et al. formulate non-linear radial consolidation equations:

$$\frac{\partial u}{\partial t} = C_h(e) \cdot \left[ \frac{\partial^2 u}{\partial r^2} + \frac{1}{r} \frac{\partial u}{\partial r} \right]$$

- **Normalized Design Curves:** They generate dimensionless design charts plotting average degree of consolidation ($U_r$) against non-linear compression index ratio ($C_c / C_k$).
- **Engineering Impact:** Neglecting non-linearity underestimates the required preloading duration by up to $30\% - 45\%$, leading to premature surcharge removal and excessive post-construction settlement.

---

## 5. Microbially Induced Calcite Precipitation (MICP) via DEM (S. Pandey, A.K. Jha, T.N. Singh)

### Biocementation Bond Mechanics
Biocementation utilizes ureolytic bacteria (*Sporosarcina pasteurii*) to hydrolyze urea in the presence of calcium ions, precipitating calcium carbonate ($\text{CaCO}_3$) crystals at grain contact throats:

$$\text{CO(NH}_2)_2 + 2\text{H}_2\text{O} + \text{Ca}^{2+} \xrightarrow{\text{Urease}} \text{CaCO}_3 \downarrow + 2\text{NH}_4^+$$

Pandey et al. implement bonded-particle models in PFC3D (Particle Flow Code) to simulate microscale bond breakage under triaxial shear:
- **Calcite Content vs. Cohesion:** Increasing $\text{CaCO}_3$ mass content from $1.5\%$ to $5.0\%$ increases apparent cohesion from $18\,\text{kPa}$ to $280\,\text{kPa}$.
- **Shear Banding:** Biocemented contacts maintain stiff elastic behavior until a peak dilatant stress ratio is reached, followed by brittle bond debonding and transition to critical state friction.

---

## 6. Ground Improvement Field Monitoring Instrumentation Suite

| Improvement Technique | Primary Geotechnical Sensor | Secondary Diagnostic Sensor | Target Monitored Parameter |
| :--- | :--- | :--- | :--- |
| **Rail Subgrade Fluidization** | High-Frequency Vibrating Wire Piezometer | Subgrade Accelerometer | Dynamic pore pressure ratio $r_u$, vertical acceleration |
| **Geopolymer Column Embankment** | Earth Pressure Cells (Column top & Soil) | Magnetic Settlement Extensometer | Stress concentration ratio ($n = \sigma_c / \sigma_s$), settlement |
| **Vertical Drain Preloading** | Multi-Depth Piezometers | Hydrostatic Settlement Profiler | Excess pore pressure dissipation ($\Delta u$), settlement profile |
| **Compaction Grouting** | Surface Optical Tiltmeters / Inclinometers | Grout Pressure Transducer at Header | Ground heave detection, header refusal pressure ($p_{inj}$) |
| **MICP Bio-Treated Soil Mass** | Cross-Hole Ultrasonic P-Wave Transducers | Effluent Ammonium Ion Sensors | Small-strain shear stiffness ($G_0$), urea conversion efficiency |
