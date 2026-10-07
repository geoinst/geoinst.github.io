---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-04-rock-mass-properties/
---

# Chapter 4 — Rock Mass Properties & The Geological Strength Index (GSI)

## 4.1 The Generalised Hoek-Brown Failure Criterion (2002 Edition)

For heavily fractured rock masses where individual structural blocks are small relative to the excavation footprint, the rock mass behaves as an isotropic equivalent pseudo-continuum. Hoek, Carranza-Torres, and Corkum (2002) formulated the generalised Hoek-Brown failure envelope:

$$\sigma_1' = \sigma_3' + \sigma_{ci} \left( m_b \frac{\sigma_3'}{\sigma_{ci}} + s \right)^a$$

Where:
- $\sigma_{ci}$ = intact rock uniaxial compressive strength
- $m_b$ = reduced value of the material constant $m_i$ for the rock mass:
  
$$m_b = m_i \exp \left( \frac{\text{GSI} - 100}{28 - 14D} \right)$$

- $s$ and $a$ are empirical constants describing rock mass fracturing and interlock:
  
$$s = \exp \left( \frac{\text{GSI} - 100}{9 - 3D} \right)$$

$$a = \frac{1}{2} + \frac{1}{6} \left( e^{-\text{GSI}/15} - e^{-20/3} \right)$$

- $D$ is the **disturbance factor** ($0.0 \le D \le 1.0$) accounting for blast-induced micro-fracturing and stress-relaxation during excavation.

---

## 4.2 The Geological Strength Index (GSI) System

The Geological Strength Index (GSI) replaces quantitative classification systems (RMR, Q) that were found to degrade in very poor, weak rock masses ($RMR < 25$). GSI relies on two visual geological observations:

1. **Rock Mass Structure (Macro-Scale Interlocking)**:
   - *Intact or massive*: Few widely spaced discontinuities.
   - *Blocky*: Well-interlocked cubical blocks formed by three intersecting orthogonal joint sets.
   - *Very blocky*: Four or more joint sets creating multi-faceted angular blocks.
   - *Disturbed / folded*: Folded, sheared, or faulted rock mass with angular blocks.
   - *Disintegrated*: Poorly interlocked, heavily crushed gravel-sized fragments.
2. **Surface Quality of Discontinuities (Joint Wall Condition)**:
   - Evaluated from *Very Good* (rough, unweathered, fresh walls) down to *Very Poor* (slickensided, soft clay gouge infill).

```
+-----------------------------------------------------------------------------------------+
|                               GEOLOGICAL STRENGTH INDEX (GSI)                           |
+---------------------+-------------------+---------------------+-------------------------+
| STRUCTURE           | Good Surface Cond | Fair Surface Cond   | Poor / Clayey Condition |
+---------------------+-------------------+---------------------+-------------------------+
| BLOCKY              |   GSI = 60 - 80   |    GSI = 50 - 65    |      GSI = 35 - 50      |
| VERY BLOCKY         |   GSI = 50 - 65   |    GSI = 40 - 55    |      GSI = 25 - 40      |
| DISTURBED / SEAMED  |   GSI = 35 - 50   |    GSI = 25 - 40    |      GSI = 15 - 30      |
| DISINTEGRATED       |   GSI = 20 - 35   |    GSI = 15 - 25    |      GSI < 15           |
+---------------------+-------------------+---------------------+-------------------------+
```

---

## 4.3 Equivalent Mohr-Coulomb Parameters ($c', \phi'$)

Because most geotechnical numerical software (FLAC, PLAXIS, RS2) requires Mohr-Coulomb parameters, Hoek et al. derived equivalent cohesion ($c'$) and friction angle ($\phi'$) by fitting linear tangent lines to the non-linear Hoek-Brown curve over an upper stress range $\sigma_{3,\max}'$:

$$\phi' = \arcsin \left[ \frac{6 a m_b (s + m_b \sigma_{3n}')^{a-1}}{2(1 + a)(2 + a) + 6 a m_b (s + m_b \sigma_{3n}')^{a-1}} \right]$$

$$c' = \frac{\sigma_{ci} \left[ (1 + 2a)s + (1 - a)m_b \sigma_{3n}' \right] (s + m_b \sigma_{3n}')^{a-1}}{(1 + a)(2 + a) \sqrt{1 + \left( 6 a m_b (s + m_b \sigma_{3n}')^{a-1} \right) / \left( (1 + a)(2 + a) \right)}}$$

---

## 4.4 Rock Mass Deformation Modulus ($E_{rm}$)

Estimating the deformation modulus of the rock mass is crucial for calculating tunnel wall convergence and foundation settlement. The Hoek-Diederichs empirical equation (2006) provides:

$$E_{rm} = E_i \left( 0.02 + \frac{1 - D/2}{1 + e^{(60 + 15D - \text{GSI})/11}} \right)$$

Where $E_i$ is intact rock Young's modulus ($\text{MPa}$). If laboratory $E_i$ is unavailable, it can be approximated from the Modulus Ratio ($MR$): $E_i = MR \cdot \sigma_{ci}$.

---

## 4.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Geological Strength Index (GSI) | Chỉ số Cường độ Địa chất (GSI) | Index (10–100) based on rock structure and joint condition |
| Disturbance factor $D$ | Hệ số tổn thương do nổ mìn $D$ | Factor (0–1) reducing rock mass strength due to blasting damage |
| Equivalent continuum | Môi trường tựa liên tục tương đương | Continuum model representing heavily jointed rock masses |
| Deformation modulus | Mô đun biến dạng khối đá | Elastic modulus representing total deformation of rock mass |
