---
lang: en
lang_alt: vi/reference-manuals/geovadis/chapter-02-ai-computational-geomechanics/
---

# AI and Computational Geomechanics

!!! abstract "Session Summary"
    Session 1 of *GeoVadis (GAIC 2025)* showcases the rapid convergence of data-driven intelligence and physics-based numerical simulations in geotechnics. Key topics include Artificial Neural Network (ANN) compaction parameter prediction, Discrete Element Method (DEM) micromechanics of plate anchors and granular flows, machine learning evaluation of cyclic liquefaction, state-parameter CPT inversions, and thermomechanical clay constitutive modeling.

---

## 1. Machine Learning for Granular Geomaterials (H. Hunt, B. Indraratna, et al.)

### The Paradigm Shift in Constitutive Modeling
Traditional continuum constitutive laws (e.g., Cam-Clay, Mohr-Coulomb, Hypoplasticity) struggle to capture complex grain-scale phenomena such as particle crushing, fabric anisotropy, stress-path dependency, and cyclic degradation without introducing excessive empirical parameters. Hunt, Indraratna, and co-authors provide a critical review of ML approaches in granular mechanics:

```
    ┌───────────────────────────┐      ┌───────────────────────────┐
    │ Continuum Phenomenology   │      │ Grain Micromechanics      │
    │  • Cam-Clay / Hardening   │      │  • DEM Contact Networks   │
    │  • Empirical calibration  │      │  • Particle breakage / CR │
    └─────────────┬─────────────┘      └─────────────┬─────────────┘
                  │                                  │
                  ▼                                  ▼
    ┌──────────────────────────────────────────────────────────────┐
    │ Physics-Informed Machine Learning (PIML / ANN)               │
    │  • Preserves conservation of energy & thermodynamic laws     │
    │  • Ingests micro-CT grain morphology & acoustic emissions    │
    │  • Generalizes across multi-axial stress paths & cycles      │
    └──────────────────────────────────────────────────────────────┘
```

### Key Findings & Limitations
1. **Data Scarcity & Domain Overfitting:** While models achieve high correlation ($R^2 > 0.95$) on specific laboratory datasets, generalizability to untested field stress paths requires physics-informed constraints (e.g., thermodynamic consistency, non-negative plastic dissipation).
2. **Grain Morphology Integration:** Integrating 3D micro-CT morphological descriptors (sphericity, roundness, surface roughness) into convolutional networks dramatically improves prediction of critical state friction angles ($\phi'_{cs}$).

---

## 2. Uplift Mechanics of Deep Horizontal Plate Anchors via DEM (R.S. Sowmya, R. Gopika, T.K. Sudheesh)

### Anchor Embedment and Rupture Mechanism
Deep horizontal plate anchors are widely used in transmission towers, offshore mooring systems, and retaining walls. Sowmya et al. deploy 3D Discrete Element Modeling (DEM) to reveal the micromechanical soil movement above anchors at varying embedment ratios ($H/B$):

- **Shallow Anchor Behavior ($H/B < 3$):** Failure surface propagates directly to the ground surface, exhibiting general shear rupture and significant surface heaving.
- **Deep Anchor Behavior ($H/B \ge 5$):** Localized shear banding and compaction bulb form immediately above the plate. Failure is governed by local cavity expansion and arching rather than daylighting surface rupture.

### Breakout Factors
The breakout factor $N_\gamma = Q_u / (\gamma A H)$ stabilizes at deep embedment:

$$Q_u = A \cdot \left[ \gamma H N_\gamma + c' N_c \right]$$

DEM contact force network visualizations reveal strong force chains radiating diagonally from the anchor edges, transferring tensile uplift into lateral confining compressive arches.

---

## 3. ANN Prediction of Soil Compaction Parameters (H. Paneru, N.P. Bhandary)

### Optimization of Compaction Controls
Standard Proctor and Modified Proctor compaction tests are time-consuming and labor-intensive. Paneru and Bhandary evaluate Multi-Layer Perceptron (MLP) architectures to predict Optimum Moisture Content ($OMC$) and Maximum Dry Density ($MDD$) from basic index properties:
- **Input Variables:** Liquid Limit ($LL$), Plastic Limit ($PL$), Plasticity Index ($PI$), Clay Fraction ($CF$), Sand Fraction ($SF$), Specific Gravity ($G_s$).
- **Model Architecture:** Levenberg-Marquardt backpropagation with Bayesian regularization.
- **Predictive Performance:** The ANN model achieved $R^2 = 0.93$ for $MDD$ and $R^2 = 0.91$ for $OMC$, providing rapid field pre-screening for highway embankments and subgrades.

---

## 4. Machine Learning for Cyclic Liquefaction Susceptibility (S. Sah, V. Bherde, U. Balunaini)

### Cyclic Triaxial Data Training
Evaluating liquefaction triggering under irregular seismic pulses traditionally relies on cyclic stress ratio ($CSR$) vs. number of cycles ($N_L$) curves. Sah et al. train Random Forest (RF) and Support Vector Machine (SVM) classifiers on extensive cyclic triaxial datasets:
- **Feature Set:** Initial mean effective confining stress ($\sigma'_{m0}$), cyclic stress ratio ($CSR$), relative density ($D_r$), fines content ($FC$), and loading frequency ($f$).
- **Pore Water Pressure Ratio ($r_u$):** The model accurately forecasts the transition from stable cyclic mobility ($r_u < 0.6$) to rapid runaway liquefaction ($r_u \to 1.0$).

---

## 5. State-Parameter CPT Interpretation in Sand (B. Dalnayak, V. Singh, S. Chatterjee)

### Inversion of In-Situ State
The cone penetration test (CPT) provides continuous tip resistance ($q_c$) and sleeve friction ($f_s$). Utilizing large-deformation finite element analysis (ALE / CEL formulation), Dalnayak et al. simulate the steady penetration of the standard $60^\circ$ cone into sand to calibrate the state parameter ($\psi = e - e_c$):

$$Q_{p} = \frac{q_c - \sigma_{v0}}{\sigma'_{v0}} = k \cdot \exp(-m \cdot \psi)$$

where $k$ and $m$ are sand-specific calibration coefficients. This numerical framework eliminates uncertainty in determining in-situ relative density and liquefaction triggering resistance without requiring undisturbed frozen sampling.

---

## 6. Synthesis: Computational Mechanics & Field Monitoring Synergies

| Computational / AI Model | Physical Geotechnical Problem | Calibrating Field Instrumentation |
| :--- | :--- | :--- |
| **PIML / Neural Constitutive Models** | Cyclic degradation of foundation soils | Resonant column tests, Downhole seismic arrays |
| **DEM Anchor Uplift Models** | Plate anchor / micropile pullout | Calibrated load cells, High-precision displacement LVDTs |
| **ANN Compaction Predictors** | Subgrade and embankment compaction | Nuclear density gauge, Sand cone test, Plate load test |
| **ML Liquefaction Classifiers** | Earthquake liquefaction triggering | Piezometer array (excess pore pressure $r_u = \Delta u / \sigma'_0$) |
| **Large-Deformation FE (CPT)** | State parameter ($\psi$) profiling | Piezocone (CPTu) tip resistance $q_t$, pore pressure $u_2$ |
