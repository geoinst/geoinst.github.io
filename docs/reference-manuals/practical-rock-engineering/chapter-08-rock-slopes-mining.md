---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-08-rock-slopes-mining/
---

# Chapter 8 — Rock Slopes in Civil & Open Pit Mining Engineering

## 8.1 The Scale Spectrum of Mining Slopes

Open pit rock slopes operate across three distinct geometric scales:

1. **Bench Scale ($10 - 30\text{ m}$ height)**: Stability controlled by kinematic planar, wedge, and toppling failures along individual joint surfaces. The primary function is to provide catch-berm retention width ($b \ge 0.2 H + 4.5\text{ m}$) catching ravelling rocks.
2. **Inter-Ramp Scale ($50 - 200\text{ m}$ height)**: Governed by fault persistence, groundwater pressures behind the face, and haulage road integrity.
3. **Overall Slope Scale ($300 - 1,000\text{ m}$ depth)**: Massive global stability governed by non-linear rock mass shear failure (Hoek-Brown criterion), regional fault zones, and regional aquifer recharge.

---

## 8.2 Primary Failure Mechanisms in Rock Slopes

```
A. PLANAR SLIDING           B. WEDGE SLIDING            C. TOPPLING FAILURE
    |  /                       |   / \                     | ||||
    | / (Dip psi_p)            |  /   \ (Intersec)         | |||| (Steep joints
    |/                         | /     \                   |/////  dipping in)
```

### 1. Planar Failure
Occurs along a single persistent joint striking parallel ($\pm 20^\circ$) to the slope face with daylighting dip ($\phi < \psi_p < \psi_f$):

$$FS = \frac{c A + (W \cos\psi_p - U - V \sin\psi_p) \tan\phi}{W \sin\psi_p + V \cos\psi_p}$$

Where:
- $W$ = weight of the sliding rock block
- $A$ = base sliding area
- $U$ = uplift pore water force on the sliding plane: $U = \frac{1}{2} \gamma_w z_w A$
- $V$ = horizontal hydrostatic cleft water force acting in tension cracks behind the crest: $V = \frac{1}{2} \gamma_w z_w^2$

### 2. Wedge Failure
Occurs along the line of intersection of two dipping joint planes dipping flatter than the slope face but steeper than their combined friction angle.

### 3. Toppling Failure
Occurs where joint sets dip steeply *into* the slope face ($\psi_d + \psi_f \ge 90^\circ + \phi$). Gravitational moment causes tall rock columns to tilt outward, opening basal cross-joints and toppling downhill.

### 4. Circular / Composite Rock Mass Failure
Occurs in heavily fractured, highly weathered, or altered rock masses ($GSI < 40$) where structural fabric does not dictate a preferred planar slide path. Analyzed via Bishop, Morgenstern-Price, or shear strength reduction (SSR) numerical modeling.

---

## 8.3 The Catastrophic Role of Groundwater

Groundwater is the single greatest driving factor in open pit slope collapses:
1. **Reduces Effective Stress**: Fluid pore pressure ($u$) directly subtracts from normal clamping stress: $\sigma' = \sigma - u$.
2. **Hydrostatic Cleft Force ($V$)**: Rain filling tension cracks behind the pit crest introduces huge driving lateral forces with zero friction resistance.
3. **Accelerates Chemical Alteration**: Weathering of clay gouge infill reduces residual friction angles from $25^\circ$ down to $8^\circ$.

### Depressurization Drainage Design
- Sub-horizontal drain holes ($75 - 100\text{ mm}$ diameter, perforated PVC casing) drilled $50 - 150\text{ m}$ into highwalls drop the phreatic line, increasing the slope Factor of Safety by $20 - 40\%$ without moving rock.

---

## 8.4 Monitoring Open Pit Slopes

| Instrument System | Measured Parameter | Role in Early Warning |
|-------------------|--------------------|------------------------|
| **Ground-Based Radar (SSR)** | Displacement along Line of Sight (LOS) | Scans entire pit 24/7; provides real-time heat maps of accelerating velocity ($mm/hr$) |
| **Robotic Total Stations (RTS)** | 3D coordinate vector $(x,y,z)$ | High-precision monitoring of prisms installed on haul roads and crests |
| **Vibrating Wire Piezometers (VWP)** | Deep pore water pressure ($u$) | Verifies effectiveness of horizontal drainage drilling and pumping dewatering wells |
| **In-Place Inclinometers (IPI)** | Deep shear displacement vs depth | Identifies exact depth of basal shear surface beneath pit floor |

---

## 8.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Catch berm | Cơ tầng lưu giữ đá rơi | Horizontal bench left between steep slopes to catch fallen rock |
| Planar failure | Phá hoại trượt phẳng | Sliding of a rock block along a single continuous plane |
| Toppling failure | Phá hoại trượt lật | Rotational overturning of steep rock columns dipping into slope |
| Tension crack | Vết nứt tách đỉnh | Tensile rupture opening behind the crest prior to sliding |
| Depressurization drain | Lỗ khoan tháo khô hạ áp | Sub-horizontal borehole drilled into rock to lower water table |
