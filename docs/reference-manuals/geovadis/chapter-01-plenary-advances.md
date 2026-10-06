---
lang: en
lang_alt: vi/reference-manuals/geovadis/chapter-01-plenary-advances/
---

# Plenary Papers: Advances in Ground Engineering & Energy Geotechnics

!!! abstract "Session Summary"
    The Plenary Session of *GeoVadis (GAIC 2025)* brings together keynote contributions from global authorities addressing foundational geotechnical engineering challenges: quality verification in deep ground improvement, earthquake-induced slope instability governed by groundwater, sustainable urban geothermal harvesting, radial drainage consolidation mechanics, and advanced experimental characterization of unsaturated geomaterials.

---

## 1. Quality Assessment & Control in Deep Mixing and Jet Grouting (F.H. Lee)

### Engineering Background & Core Challenges
Deep mixing (cement-soil columns) and jet grouting are extensively deployed across Asia for excavation support walls, cutoff barriers, and foundation ground improvement in soft alluvial and marine clays. However, the resulting columns exhibit substantial spatial variability in compressive strength ($q_u$), column continuity, and geometric diameter due to non-uniform in-situ jetting energy dissipation and soil stratification.

### Diagnostic & Verification Techniques
Professor Lee synthesizes conventional and modern non-destructive evaluation (NDE) methodologies:
- **Continuous Core Drilling:** The industry benchmark, requiring at least 85% core recovery to determine spatial strength profiles.
- **Wet Grab Sampling:** Fresh slurry extraction immediately post-jetting to evaluate batch uniformity prior to hardening.
- **Electrical Resistivity Tomography (ERT) & Cross-Hole Sonic Logging (CSL):** Non-destructive imaging of column geometric continuity, necking defects, and column verticality.

### Engineering Implications & Reliability
The coefficient of variation ($COV$) of unconfined compressive strength ($q_u$) in deep mixed ground typically ranges between $0.30$ and $0.65$. Structural and settlement calculations that ignore this variability significantly overestimate the design factor of safety. The paper establishes reliability-based partial factors ensuring performance-based serviceability limit state (SLS) and ultimate limit state (ULS) compliance.

---

## 2. Groundwater Effects on Coseismic Slope Instability: 2024 Noto Peninsula Earthquake (I. Towhata, S. Oji, T. Hosoya)

### The 2024 Noto Peninsula Event
On January 1, 2024, a major earthquake ($M_w 7.5$) struck the Noto Peninsula in Ishikawa Prefecture, Japan, triggering thousands of coseismic landslides and debris flows that isolated communities and devastated critical coastal infrastructure.

### The Decisive Role of Groundwater
Professor Towhata and co-authors demonstrate that slope failures were not solely driven by inertial shaking forces:
- **Antecedent Precipitation:** Heavy antecedent winter precipitation and snowmelt had elevated the phreatic surface, saturating weathered Neogene sedimentary rocks and volcanic tuff.
- **Transient Pore Water Pressure Spikes:** Strong ground shaking generated severe excess pore water pressures ($\Delta u$) along permeable/impermeable geological boundaries, dramatically reducing effective normal stress ($\sigma' = \sigma - u$).
- **Delayed Failures:** Several major slope failures mobilized hours after the primary shock, underscoring the role of groundwater seepage redistribution and localized drainage obstruction.

```
                          Pre-Earthquake State: High Phreatic Line
                          ┌───────────────────────────────────────┐
                          │ Rain / Snowmelt Infiltration          │
                          │   ▼        ▼        ▼        ▼        │
             Ground       ┌─────────────────────────────────────┐ │
             Surface  ───►│ Saturated Weathered Overburden      │ │
                          │═════════════════════════════════════│ │
                          │ Phreatic Water Table (Elevated)     │ │
                          └─────────────────────────────────────┘ │
                                            │                     │
                     Coseismic Dynamic Shaking (Mw 7.5)           │
                                            ▼                     │
                          ┌─────────────────────────────────────┐ │
                          │ Dynamic Excess Pore Pressure (Δu)   │ │
                          │ Effective Stress σ' = σ - (u + Δu)  │ │
                          │ Shear Strength τ_f Drops Critically │ │
                          │ ──► Planar & Rotational Slides ──►  │ │
                          └─────────────────────────────────────┘ │
                          └───────────────────────────────────────┘
```

---

## 3. Sustainable Urban Energy Foundations (L. Laloui, E. Ravera, A.F. Rotta Loria)

### Concept of Thermo-Active Geo-Structures
Energy geo-structures—such as energy piles, energy diaphragm walls, and energy tunnel linings—integrate heat exchanger pipes (closed-loop fluid circuits) directly within structural foundation elements to provide dual functionality:
1. Primary structural support of mechanical superstructure loads.
2. Renewable thermal energy exchange with the surrounding ground for building space heating and cooling via Ground Source Heat Pumps (GSHP).

### Thermo-Mechanical Soil-Structure Interaction
Thermal variations ($\Delta T$) induce cyclic thermal expansion and contraction within the structural concrete:
- **Restrained Thermal Stresses:** When thermal axial expansion is restrained by pile tip resistance and shaft friction, significant compressive thermal stresses develop:
  $$\Delta \sigma_{th} = - E_{pile} \cdot \alpha_c \cdot \Delta T$$
  where $E_{pile}$ is the elastic modulus and $\alpha_c$ is the coefficient of thermal expansion of concrete.
- **Soil Creep and Cyclic Plasticity:** Repetitive seasonal thermal cycling alters the stiffness and shear mobilization of surrounding clays, requiring careful verification against thermal fatigue and differential settlement.

---

## 4. Consolidation Under Radial Drainage (R.G. Robinson, G. Sridhar, R.P. Aparna)

### Radial Drainage Mechanics in Soft Ground
Radial consolidation accelerated by Prefabricated Vertical Drains (PVD) is standard practice for preloading soft marine clays and dredge fills. Professor Robinson and colleagues review Barron's and Hansbo's classical solutions:

$$\bar{U}_r = 1 - \exp\left( -\frac{8 \, T_r}{\mu} \right)$$

where $T_r = c_h t / d_e^2$ is the radial time factor, $d_e$ is the equivalent drain influence diameter, and $\mu$ is the geometry and smear resistance factor:

$$\mu \approx \ln\left(\frac{n}{s}\right) + \frac{k_h}{k_s}\ln(s) - \frac{3}{4} + \pi z (2l - z)\frac{k_h}{q_w}$$

### Key Practical Insights
- **Smear Zone Permeability ($k_h / k_s$):** The ratio of horizontal undisturbed permeability to smear zone permeability typically ranges from $2$ to $5$, severely retarding consolidation if mandrel disturbance is uncontrolled.
- **Well Resistance ($q_w$):** In long vertical drains ($> 20\,\text{m}$), hydraulic discharge capacity of the core becomes a governing bottleneck.

---

## 5. Experimental Mechanics of Unsaturated Soils (T. Nishimura)

### Suction-Controlled Laboratory Testing
Professor Nishimura presents advanced experimental techniques for characterizing unsaturated soil behavior:
- **Axis Translation Technique:** Separates pore air pressure ($u_a$) and pore water pressure ($u_w$) across high-air-entry ceramic disks to control matric suction ($\psi = u_a - u_w$).
- **Soil-Water Characteristic Curve (SWCC):** Captures hysteretic wetting and drying loops governing water retention.
- **Extended Mohr-Coulomb Shear Strength:**
  $$\tau_f = c' + (\sigma - u_a)\tan\phi' + (u_a - u_w)\tan\phi^b$$
  where $\phi^b$ defines the rate of shear strength increase with matric suction.

---

## 6. Field Instrumentation Checklist for Ground Engineering Advances

| Application | Recommended Primary Sensor | Secondary / Redundant Sensor | Key Engineering Parameter |
| :--- | :--- | :--- | :--- |
| **Deep Mixed & Jet Grout Columns** | Cross-Hole Sonic Logging (CSL) | Coring + Lab UCS Testing | Column continuity, $q_u$, necking |
| **Coseismic Slopes** | Vibrating Wire Piezometer | Inclinometer Casing | Pore water pressure ($\Delta u$), slip depth |
| **Thermo-Active Energy Piles** | Vibrating Wire Strain Gauges + Sister Bars | Distributed Temperature Sensing (DTS fiber) | Thermal axial strain ($\epsilon_{th}$), temp ($T$) |
| **PVD Vacuum Preloading** | Multi-Depth Piezometers | Magnetic Settlement Extensometers | Consolidation dissipation ($U_r$), settlement |
| **Unsaturated Soil Slopes** | Tensiometers / High-capacity Psychrometers | Time-Domain Reflectometry (TDR) | Matric suction ($\psi$), volumetric moisture ($\theta$) |
