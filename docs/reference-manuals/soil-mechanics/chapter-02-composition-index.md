---
lang: en
lang_alt: vi/reference-manuals/soil-mechanics/chapter-02-composition-index/
---
# Chapter 2 — Soil Composition & Index Properties

## 2.1 The phase diagram

Soil is described by the **phase diagram**, which separates the volume into solids,
water, and air. The key volume ratios are:

- **Void ratio** $e = V_v / V_s$ — the volume of voids per unit volume of solids.
- **Porosity** $n = V_v / V$ — the fraction of the total volume that is voids.
- **Degree of saturation** $S = V_w / V_v$ — the fraction of voids filled with
  water.

![Figure: soil-mechanics-phase-diagram](../../assets/figures/soil-mechanics-phase-diagram.svg)

**Figure.** The soil phase diagram: solids, water, and air volumes and weights, and the relationships between void ratio, porosity, and saturation (after FHWA-NHI-06-088).

## 2.2 Unit weights and water content

- **Water content** $w = W_w / W_s$ — the mass of water per unit mass of solids.
- **Bulk (total) unit weight** $\gamma$ — the total weight per unit volume.
- **Dry unit weight** $\gamma_d = \gamma / (1 + w)$ — the weight of solids per unit
  volume; the key compaction control parameter.
- **Saturated unit weight** $\gamma_{sat}$ — when all voids are water-filled.
- **Submerged (buoyant) unit weight** $\gamma' = \gamma_{sat} - \gamma_w$.

## 2.3 Particle-size distribution

**Sieve analysis** (for coarse soil) and **hydrometer analysis** (for fines) give
the **grading curve**. From it:

- **$D_{10}$, $D_{30}$, $D_{60}$** — the particle sizes at which 10%, 30%, and 60%
  pass.
- **Coefficient of uniformity** $C_u = D_{60}/D_{10}$ — how well-graded the soil is.
- **Coefficient of curvature** $C_c$ — the shape of the curve.

A **well-graded** soil (a wide range of particle sizes) compacts denser and drains
better than a **uniformly graded** one.

## 2.4 Atterberg limits and consistency

For fine-grained soils, the **Atterberg limits** define the water contents at which
the soil changes consistency:

- **Liquid limit (LL)** — from plastic to liquid.
- **Plastic limit (PL)** — from semi-solid to plastic.
- **Plasticity index** $PI = LL - PL$ — the range of water content over which the
  soil is plastic.

A high $PI$ indicates a **compressible, plastic clay**; a low $PI$ indicates a
**silt or low-plasticity soil**. The limits are used directly in classification
([Chapter 3](chapter-03-classification.md)).

## 2.5 Key takeaways

- The **phase diagram** relates voids, water, and solids; $e$, $n$, and $S$ describe
  the packing.
- **Dry unit weight** is the key compaction parameter.
- **Grading** ($C_u$, $C_c$) tells how well-graded and drainable a coarse soil is.
- **Atterberg limits** ($LL$, $PL$, $PI$) describe the plasticity of fines.
- Index properties are cheap, fast, and **strongly correlated** with engineering
  behaviour.
