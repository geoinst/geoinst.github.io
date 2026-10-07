---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-03-discontinuity-shear-strength/
---

# Chapter 3 — Shear Strength of Discontinuities

## 3.1 Mechanics of Shearing Along Joint Surfaces

In rock masses with persistent joint sets, structural failures (bench slides, wedge dropouts, toppling blocks) occur by sliding along pre-existing discontinuities rather than by fracturing through intact rock substance.

The shear resistance ($\tau$) along an unbonded rock joint is governed by three factors:
1. **Normal Stress ($\sigma_n'$)**: Effective compressive stress clamping the joint lips together.
2. **Basic Friction Angle ($\phi_b$)**: Inter-grain friction angle measured on smooth, planar, saw-cut surfaces of the same rock (typically $25^\circ - 35^\circ$).
3. **Surface Roughness & Asperity Dilatancy**: Geometric undulations (asperities) forcing the opposing joint walls to ride up over each other (dilate) during shearing, or shear through the asperities at high normal stresses.

---

## 3.2 Patton’s Bilinear Model

F.D. Patton (1966) showed that regular teeth-shaped asperities inclined at angle $i$ produce a bilinear shear strength envelope:

### Low Normal Stress ($\sigma_n' < \sigma_T$): Sliding Over Asperities
Shear displacement forces the blocks to dilate vertically over asperity teeth:

$$\tau = \sigma_n' \tan(\phi_b + i)$$

### High Normal Stress ($\sigma_n' \ge \sigma_T$): Shearing Through Asperities
Normal stress suppresses dilation; the asperity teeth shear off across their roots:

$$\tau = c_j + \sigma_n' \tan(\phi_r)$$

Where $c_j$ is apparent cohesion from asperity root shearing and $\phi_r$ is residual friction angle.

---

## 3.3 The Barton-Bandis Non-Linear Shear Strength Criterion

Because real rock joints have irregular, multi-scale roughness rather than uniform teeth, Nick Barton and S. Bandis (1976, 1982, 1990) established the empirical non-linear criterion:

$$\tau = \sigma_n' \tan \left[ \text{JRC} \cdot \log_{10} \left( \frac{\text{JCS}}{\sigma_n'} \right) + \phi_b \right]$$

Where:
- $\text{JRC}$ = Joint Roughness Coefficient, varying from $0$ (mirror smooth) to $20$ (very rough, undulating).
- $\text{JCS}$ = Joint Wall Compressive Strength, determined using a Schmidt rebound hammer directly on the unweathered or weathered joint wall.
- $\phi_b$ = Basic friction angle of flat, unweathered rock surfaces.
- $\sigma_n'$ = Effective normal stress across the joint aperture.

### Scale Correction for Field Joints
Laboratory shear box tests ($L_0 = 100\text{ mm}$) overestimate roughness compared to blocky field discontinuities ($L_n = 1 - 5\text{ m}$):

$$\text{JRC}_n = \text{JRC}_0 \left( \frac{L_n}{L_0} \right)^{-0.02 \text{JRC}_0}$$

$$\text{JCS}_n = \text{JCS}_0 \left( \frac{L_n}{L_0} \right)^{-0.03 \text{JRC}_0}$$

---

## 3.4 Infilled Joints & Gouge Fillings

When weathering or fault shearing deposits fine-grained infill (clay gouge, talc, chlorite) between joint walls, asperity interlock is lost.

- If infill thickness $t < \text{asperity height } a$, rock-to-rock contact still contributes to shear resistance.
- If infill thickness $t \ge 1.5 a$, shear strength drops to the drained or undrained shear strength of the gouge material alone ($\phi' \approx 8^\circ - 18^\circ$ for smectite clays). This forms the critical slip planes responsible for historical landslides like the Vajont disaster.

---

## 3.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Discontinuity shear strength | Sức kháng cắt của mặt bất liên tục | Shear resistance along joints, bedding, and faults |
| Basic friction angle $\phi_b$ | Góc ma sát cơ bản $\phi_b$ | Friction angle on smooth, planar saw-cut surfaces |
| Asperity | Mấu nhám | Micro- and macro-scale geometric undulation on a joint face |
| Joint Roughness Coefficient (JRC) | Hệ số độ nhám khe nứt (JRC) | Dimensionless index (0–20) quantifying joint surface profile |
| Joint Wall Compressive Strength (JCS) | Cường độ nén thành vách khe nứt (JCS) | Uniaxial compressive strength of the rock surface forming the joint wall |
| Fault gouge | Sét dập vỡ đứt gãy / Vữa đứt gãy | Soft, highly sheared clayey material filling a fault zone |
