---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-01-what-is-rock-engineering/
---

# Chapter 1 — What is Rock Engineering?

## 1.1 Historical Context & Discipline Evolution

Rock engineering emerged as a distinct engineering discipline in the mid-20th century. Prior to this, underground mining and tunneling were largely treated as crafts guided by empirical rules of thumb, while surface excavations borrowed uncritically from soil mechanics.

The catastrophic failures of the mid-20th century demonstrated the lethal shortcomings of treating rock masses as homogeneous soils:

1. **Malpasset Dam Failure (France, 1959)**: A thin concrete arch dam collapsed catastrophically upon its first filling, killing 423 people. The dam concrete did not fail; rather, an unmapped foliation shear zone and unfavorably oriented foliation planes beneath the left abutment uplifted under reservoir cleft water pressure.
2. **Vajont Slide Disaster (Italy, 1963)**: A colossal rock mass of 270 million $\text{m}^3$ detached along clay interbeds within limestone bedding planes, sliding into the reservoir at 110 km/h. The resulting 250 m displacement wave overtopped the dam and eradicated downstream valleys, causing over 2,000 casualties.
3. **Coalbrook Colliery Collapse (South Africa, 1960)**: A massive cascading collapse of over 4,000 coal pillars over 3 $\text{km}^2$ trapped and killed 437 miners within minutes, proving that tributary area pillar designs without confinement criteria fail catastrophically.

These disasters forced civil and mining engineers to recognize that **the mechanical behavior of a rock mass is dominated not by the strength of the rock material itself, but by the structural discontinuities (joints, faults, bedding planes) dissecting it and the fluid pressures acting within those discontinuities.**

---

## 1.2 Rock Material vs. Rock Mass

The central paradigm shift articulated by Dr. Evert Hoek is the fundamental distinction between:

- **Intact Rock (Rock Material)**: The unbroken rock element between structural discontinuities, typically sampled as intact drill core cylinders ($\approx 50\text{ mm}$ diameter). It behaves as a continuous, brittle-elastic solid whose compressive strength is determined by mineral bonding and microscopic microcracks.
- **Rock Mass**: The in-situ structural medium comprising intact rock blocks partitioned by intersecting networks of joints, shears, bedding surfaces, and faults. A rock mass is **discontinuous, anisotropic, inhomogeneous, and non-elastic**.

```
+--------------------------------------------------------------+
|                         ROCK MASS                            |
|                                                              |
|   +---------------+      / /      +---------------+          |
|   |  Intact Rock  |     / /       |  Intact Rock  |          |
|   |     Block     |    / / Joint  |     Block     |          |
|   +---------------+   / /  Plane  +---------------+          |
|          \ \         / /                 \ \                 |
|           \ \ Fault / /                   \ \ Bedding        |
|   +---------------+      / /      +---------------+          |
|   |  Intact Rock  |     / /       |  Intact Rock  |          |
|   |     Block     |    / /        |     Block     |          |
|   +---------------+   / /         +---------------+          |
+--------------------------------------------------------------+
```

---

## 1.3 The Scale Effect in Rock Mechanics

As the scale of the engineering problem increases from laboratory test specimens to bench faces and deep cavern envelopes, the measured compressive strength and deformation modulus drop dramatically.

$$\text{Strength}_{\text{Rock Mass}} \ll \text{Strength}_{\text{Intact Laboratory Core}}$$

- At a scale of $0.05\text{ m}$ (laboratory core), intact tensile and compressive micro-mechanics govern.
- At a scale of $1 - 5\text{ m}$ (tunnel perimeter or mine bench), kinematically releaseable polyhedral blocks dictate stability.
- At a scale of $> 30\text{ m}$ (deep open pit slope or large underground crusher chamber), heavily jointed rock behaves as an equivalent pseudo-continuum governed by the Hoek-Brown rock mass criteria.

---

## 1.4 The Observational Method in Rock Engineering

Because pre-construction exploration boreholes sample less than $0.001\%$ of the rock mass volume, complete geological foreknowledge is mathematically impossible. Rock engineering therefore relies on the **Observational Method** (Peck, 1969):

1. Establish designs based on the most probable geological and geotechnical model.
2. Formulate explicit hypotheses regarding acceptable deformation thresholds.
3. Install geotechnical instrumentation arrays (piezometers, extensometers, convergence points).
4. Continuously measure ground response during progressive excavation.
5. Implement pre-planned Trigger Action Response Plans (TARP) when monitored rates exceed baseline limits.

---

## 1.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Intact rock | Đá nguyên vẹn | Unbroken rock material between structural discontinuities |
| Rock mass | Khối đá | In-situ medium composed of intact blocks and discontinuity systems |
| Discontinuity | Mặt bất liên tục | General term for joints, bedding, shears, and faults |
| Cleft water pressure | Áp lực nước khe nứt | Hydrostatic and hydrodynamic fluid pressure acting inside joint apertures |
| Observational Method | Phương pháp quan trắc | Design methodology coupling construction progress with real-time field measurements |
