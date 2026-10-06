---
lang: en
lang_alt: vi/reference-manuals/geovadis/chapter-04-earthquake-soil-dynamics/
---

# Earthquake Geotechnical Engineering and Soil Dynamics

!!! abstract "Session Summary"
    Session 3 of *GeoVadis (GAIC 2025)* presents breakthrough developments in earthquake engineering, cyclic soil plasticity, and vibration mitigation. Focus areas include sustainable biopolymer treatment against cyclic liquefaction, packing index quantification in granular soils, sand-rubber mixture (SRM) wave barriers, seismic isolation using disconnected piled rafts and geocells, and field monitoring of blast-induced ground vibrations.

---

## 1. Biopolymer Mitigation of Silty Sand Liquefaction (N.V. Dasari, M.D. Tellam, K.K. Gonavaram)

### Green Soil Stabilization Alternative
Chemical grouting and cement stabilization incur substantial carbon footprints and risk groundwater contamination. Dasari et al. investigate natural **chitosan** (a biopolymer derived from crustacean chitin shells) as an eco-friendly soil stabilizer to mitigate liquefaction in loose silty sands ($FC = 15\% - 25\%$):
- **Hydrogel Bridging Mechanism:** Upon mixing and curing, chitosan forms viscous biopolymer hydrogel filaments that coat granular quartz surfaces and bridge inter-particle pore throats.
- **Cyclic Resistance Ratio ($CRR_{15}$):** Strain-controlled cyclic triaxial testing reveals that treating loose silty sand with $1.0\%$ chitosan increases the cyclic resistance ratio ($CRR$) by up to $180\%$.
- **Pore Water Pressure Retardation:** The rate of excess pore water pressure generation ($\Delta u / \sigma'_0$) slows dramatically, preventing catastrophic loss of effective confinement during earthquake cycles.

```
       Untreated Loose Silty Sand               Chitosan Biopolymer Treated Sand
       ┌───────────────────────────┐            ┌───────────────────────────┐
       │   ○       ○       ○       │            │   ○───────○═══════○       │
       │     ○       ○       ○     │   ─────►   │   │  Biopolymer   │       │
       │   ○       ○       ○       │            │   ○═══Hydrogel════○       │
       │ (Loose grain contacts)    │            │ (Interlocking bonded webs)│
       └─────────────┬─────────────┘            └─────────────┬─────────────┘
                     │                                        │
             Earthquake Shaking                       Earthquake Shaking
                     ▼                                        ▼
       ┌───────────────────────────┐            ┌───────────────────────────┐
       │ Rapid Δu spike (ru ──► 1) │            │ Damped Δu (ru < 0.40)     │
       │ Shear liquefaction failure│            │ Elastic-plastic integrity │
       └───────────────────────────┘            └───────────────────────────┘
```

---

## 2. Packing Index for Liquefaction Resistance (M.U. Rehman, R.K. Kandasami, S. Banerjee)

### Beyond Relative Density ($D_r$)
Relative density ($D_r$) often correlates poorly with the liquefaction resistance of sands with varying grain angularity and broad particle size distributions. Rehman et al. propose a micro-mechanically informed **Packing Index ($I_p$)**:

$$I_p = \frac{e_{max} - e}{e_{max} - e_{min}} \cdot \left( \frac{d_{50}}{d_{10}} \right)^{\alpha} \cdot \Phi_s$$

where $\Phi_s$ is particle sphericity and $\alpha$ is a gradation coefficient.
- **Micro-CT Verification:** 3D X-ray tomography demonstrates that sands with identical $D_r$ but lower sphericity form higher coordination numbers ($Z_c$) and stiffer contact force arches.
- **Correlation with $CRR$:** The packing index achieves a unified correlation with cyclic resistance ratio across both uniform clean sands and well-graded silty sands ($R^2 = 0.94$).

---

## 3. Vibration Screening via Sand-Rubber Mixture (SRM) Trenches (A. Boominathan, J.S. Dhanya, et al.)

### Dynamic Wave Barrier Mechanics
Ground-borne vibrations induced by impact pile driving, high-speed rail lines, and heavy machinery induce structural resonance and acoustic fatigue in adjacent urban structures. Boominathan et al. deploy open vs. infilled wave-screening trenches using Sand-Rubber Mixtures (SRM):
- **Impedance Mismatch:** Shredded scrap tyre crumbs mixed with coarse sand ($30/70$ by weight) create an acoustic impedance mismatch ratio ($\rho v_s$) of less than $0.35$ relative to virgin subsoil.
- **Rayleigh Wave Attenuation:** Numerical 3D finite element and experimental field trials reveal that an SRM trench of normalized depth $H / \lambda_R \ge 0.75$ attenuates Rayleigh wave amplitude by up to $68\%$ in the passive screening zone.
- **Geotechnical Stability:** Unlike open trenches that require shoring or collapse in high groundwater tables, SRM trenches maintain self-supporting vertical trench walls while filtering vibration.

---

## 4. Seismic Performance of Disconnected Piled Raft Foundations (A.K. Suman, J.S. Rajeswari)

### Cushion Layer Seismic Isolation
In high-seismicity regions, connecting rigid piles directly to the foundation raft concentrates immense inertial shear forces and bending moments at the pile heads:
- **Disconnected Cushion Design:** A compacted gravel-geogrid cushion layer ($0.5\,\text{m} - 1.0\,\text{m}$ thickness) is inserted between the raft underside and the pile heads.
- **Inertial Decoupling:** Dynamic centrifuge tests and finite element simulations confirm that the cushion layer slips plastically during peak spectral accelerations, bounding the maximum shear transfer into the piles.
- **Moment Reduction:** Pile head bending moments are reduced by $50\% - 75\%$ compared to rigidly connected piled rafts, eliminating brittle shear failures at the raft-pile junction while providing adequate settlement control under static gravity loads.

---

## 5. Blast-Induced Vibration Monitoring (A. Anil, T. Naskar, A. Boominathan, A. Joseph)

### Demolition Dynamic Signatures
During controlled blast demolition of heavy industrial chimneys and coal towers, explosive energy generates transient shock waves that propagate through complex geological strata:
- **Triaxial Velocity Sensors:** Orthogonal geophones (transverse, vertical, radial) record Peak Particle Velocity ($PPV$) and frequency spectra.
- **USBM Attenuation Law:** Field data fit the scaled distance equation:
  $$PPV = K \cdot \left( \frac{R}{\sqrt{Q}} \right)^{-B}$$
  where $Q$ is explosive charge per delay (kg) and $R$ is standoff distance (m).
- **Vibration Control:** Real-time array telemetry verifies that vibration frequencies remain above natural structural frequencies ($> 20\,\text{Hz}$), avoiding structural resonance in adjacent plant buildings.

---

## 6. Soil Dynamics Instrumentation Matrix

| Dynamic Phenomenon | Primary Monitoring Sensor | Complementary Instrument | Output Parameter |
| :--- | :--- | :--- | :--- |
| **Seismic Liquefaction Triggering** | High-Frequency Vibrating Wire Piezometer | Downhole Accelerometer Pair | Dynamic $\Delta u$, cyclic shear strain $\gamma_{cyc}$ |
| **Vibration Barrier Verification** | Triaxial Surface Geophones ($4.5\,\text{Hz}$) | Digital Seismograph | Peak Particle Velocity ($PPV$), FFT frequency |
| **Disconnected Piled Raft** | Dynamic Earth Pressure Cells | Pile-Toe Sister Bar Strain Gauges | Raft contact stress, pile axial load transfer |
| **Impact Pile Driving Attenuation**| Piezoelectric Accelerometers | Laser Doppler Vibrometer | Ground vibration peak acceleration ($a_{max}$) |
| **Subsurface Shear Wave Velocity**| Downhole Geophone / Cross-hole Probe | P-S Suspension Logger | Shear wave velocity $V_s$, small-strain modulus $G_{max}$ |
