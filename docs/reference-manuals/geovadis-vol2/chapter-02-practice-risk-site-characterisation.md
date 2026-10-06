---
lang: en
lang_alt: vi/reference-manuals/geovadis-vol2/chapter-02-practice-risk-site-characterisation/
---

# Practice, Risk and Site Characterisation

!!! abstract "Session Summary"
    Session 7 of *GeoVadis (GAIC 2025)* bridges cutting-edge diagnostic technologies with professional geotechnical practice and risk management. Highlights include time-lapse Electrical Resistivity Tomography (ERT) for internal seepage imaging, advanced surface wave geophysics (MASW), Dilatometer Test (DMT) dissipation for overconsolidation profiling, mechanoluminescent visualization of pile driving mechanics, and geotechnical Building Information Modelling (BIM).

---

## 1. Time-Lapse ERT for Embankment Seepage Monitoring (V. Bherde, B. Umashankar)

### Non-Invasive Internal Flaw Detection
Piping erosion, localized sinkholes, and phreatic surface anomalies inside earth dams and levees frequently develop undetected prior to catastrophic breach. Bherde and Umashankar conduct model-scale investigations using 2D/3D time-lapse Electrical Resistivity Tomography (ERT):
- **Resistivity Contrast:** Water saturation dramatically decreases bulk electrical resistivity ($\rho$), creating sharp contrasts between dry unsaturated fill ($\rho > 500\,\Omega\cdot\text{m}$) and seepage-saturated zones ($\rho < 50\,\Omega\cdot\text{m}$).
- **Inversion Resolution:** By optimizing electrode array geometries (Wenner-Schlumberger vs. Dipole-Dipole), the system detects piping void inception ($D \approx 50\,\text{mm}$) and captures the advance velocity of the wetting front in real time without perforating the dam core.

```
          Infiltration Water Source
                     │
                     ▼
       ┌──────────────────────────────┐
       │ Dense Earth Dam Embankment   │ ◄─── High Resistivity (Dry: > 500 Ω·m)
       │                              │
       │    Electrode Array String    │
       │    ▼   ▼   ▼   ▼   ▼   ▼   ▼  │
       │                              │
       │      ░░░░░░░░░░░░░░░░        │ ◄─── Wetting Front / Seepage Zone
       │      ░ Seepage Plume ░        │      Low Resistivity (< 50 Ω·m)
       │      ░░░░░░░░░░░░░░░░        │      Inverted in Real-Time 2D Tomogram
       └──────────────────────────────┘
```

---

## 2. Advanced Surface Wave Geophysics (MASW) (P. Vishwakarma; C.P. Lin, et al.)

### Shear Wave Velocity ($V_s$) Profiling
Multichannel Analysis of Surface Waves (MASW) provides non-destructive subsurface stiffness profiling without costly deep boreholes:
- **Dispersion Inversion Optimization:** Vishwakarma evaluates Teaching-Learning-Based Optimization (TLBO) algorithms to invert experimental Rayleigh wave dispersion curves into small-strain shear wave velocity ($V_s$) profiles down to $30\,\text{m}$ depth.
- **Seismic Site Classification:** Lin and co-authors deploy new-generation active/passive surface wave sensors to compute $V_{s30}$, identifying soft soil amplification zones, buried bedrock channels, and shear modulus degradation ($G_{max} = \rho V_s^2$).

---

## 3. Flat Dilatometer Test (DMT) Dissipation in Soft Marine Clay (K. Das, G.R. Dodagoudar, et al.)

### Direct In-Situ Overconsolidation Ratio ($OCR$)
Determining preconsolidation stress ($\sigma'_p$) and horizontal coefficient of consolidation ($c_h$) in sensitive alluvial and marine clays through laboratory oedometer testing is prone to sample disturbance. Das et al. conduct Marchetti Flat Dilatometer Tests (DMT) with timed pressure dissipation ($A$-readings):
- **Horizontal Stress Index ($K_D$):** In-situ overconsolidation ratio correlates directly with horizontal stress index:
  $$OCR = (0.5 \cdot K_D)^{1.56}$$
- **Pore Pressure Dissipation:** Time required for $50\%$ pressure decay ($t_{50}$) yields reliable horizontal coefficient of consolidation ($c_h$) estimates that closely match back-calculated settlement rates from nearby instrumented highway embankments.

---

## 4. Mechanoluminescent Imaging of Pile Penetration (A. Kondo, E. Kohama, D. Takano, R.J. Bathurst)

### Optical Grain-Scale Contact Visualization
Visualizing shear strain localization and crush zones beneath advancing pile tips has historically required complex X-ray radiography. Kondo et al. develop an innovative optical method using sand grains coated with **mechanoluminescent phosphor** ($\text{SrAl}_2\text{O}_4:\text{Eu}$):
- **Luminescent Stress Response:** Upon mechanical shear and compressive contact stress, the phosphor emits visible green light proportional to localized contact stress magnitude.
- **High-Speed Photometry:** High-speed cameras capture dynamic stress concentration bulbs and intense shear band formation radiating outward from the pile tip during steady penetration into dense sand.

---

## 5. Standard Penetration Test (SPT): Forensic Practice Appraisal (M.M. Hoque, M.M. Rahman)

### Global Standards vs. Developing Region Realities
The Standard Penetration Test ($N$-value) remains the most ubiquitous site characterization parameter in worldwide foundation design. Hoque and Rahman review field practices across Bangladesh and South Asia, highlighting critical discrepancies from ASTM D1586:
- **Hammer Energy Ratio ($ER$):** Manual cathead-and-rope trip mechanisms deliver actual energy ratios between $45\%$ and $58\%$, compared to the standardized $60\%$ automatic trip hammer benchmark ($N_{60}$).
- **Borehole Cleaning & Wash Boring:** Incomplete bottom cleaning and hydrostatic head imbalance in casing pipes induce bottom piping, reducing measured $N$-values by up to $50\%$.
- **Corrected Standardized Value:** Designers must systematically enforce correction formulas:
  $$N_{60} = N_{raw} \cdot \frac{ER}{60} \cdot C_B \cdot C_S \cdot C_R$$
  where $C_B, C_S, C_R$ account for borehole diameter, sampler liner, and rod length.

---

## 6. Site Characterisation Field Instrumentation Matrix

| Site Characterisation Tool | Primary Geophysical / In-Situ Sensor | Complementary Lab / Field Probe | Derived Geotechnical Parameter |
| :--- | :--- | :--- | :--- |
| **Time-Lapse ERT Array** | Multi-Electrode Resistivity Cable | Piezometers at Anomaly Locations | Internal saturation, seepage velocity, piping |
| **MASW Seismic Array** | Linear Geophone Array ($4.5\,\text{Hz}$) | Downhole P-S Seismic Logger | Shear wave velocity $V_s$, small-strain modulus $G_0$ |
| **Flat Dilatometer (DMT)** | Stainless Steel Dilatometer Blade | Piezocone Penetrometer (CPTu) | In-situ $OCR$, horizontal consolidation $c_h$ |
| **Mechanoluminescent Array**| High-Speed CCD Photometric Sensor | Dynamic Load Cells at Pile Head | Contact stress bulb, localized shear banding |
| **Calibrated SPT Rig** | Instrumented SPT Sub (Load & Accel) | Energy Ratio Calibrator Box | Delivered energy ratio $ER$, standardized $N_{60}$ |
