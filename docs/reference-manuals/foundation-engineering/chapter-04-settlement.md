---
lang: en
lang_alt: vi/reference-manuals/foundation-engineering/chapter-04-settlement/
---
# Chapter 4 — Shallow Foundations: Settlement

## 4.1 Why settlement usually governs

For most structures on good ground, **bearing capacity is not the controlling
criterion — settlement is**. A footing can be far from shear failure yet still
settle enough to crack finishes, distort frames, or misalign machinery. Design
therefore computes settlement and compares it with the **tolerable movement** for
the structure.

## 4.2 The three components of settlement

Total settlement has three parts:

1. **Immediate (elastic) settlement** — occurs as the load is applied, from elastic
   compression and lateral deformation of the soil. Significant in sands and
   unsaturated soils.
2. **Primary consolidation settlement** — time-dependent drainage and volume change
   in saturated fine-grained soils, governed by **Terzaghi's one-dimensional
   consolidation theory**. Can take months to years.
3. **Secondary (creep) settlement** — continued volume change at constant effective
   stress, especially in organic and soft clays.

![Figure: foundation-settlement](../../assets/figures/foundation-settlement.svg)

**Figure.** The three components of foundation settlement — immediate, primary consolidation, and secondary — accumulate over time (after USACE EM 1110-1-1904).

## 4.3 Immediate settlement

Immediate settlement is computed from **elastic theory**:

$$S_e = q B \frac{1-\nu^2}{E} I_s$$

where $q$ is the applied pressure, $B$ the footing width, $E$ and $\nu$ the soil's
elastic modulus and Poisson's ratio, and $I_s$ an influence factor depending on
footing shape and rigidity. In sands, $E$ is often estimated from **SPT or CPT**
correlations.

## 4.4 Primary consolidation settlement

For a normally consolidated clay:

$$S_c = \frac{C_c H}{1+e_0}\log\frac{\sigma'_{v0}+\Delta\sigma}{\sigma'_{v0}}$$

where $C_c$ is the compression index, $H$ the layer thickness, $e_0$ the initial
void ratio, $\sigma'_{v0}$ the initial effective stress, and $\Delta\sigma$ the
stress increase. For over-consolidated clays the **recompression index** $C_r$ is
used up to the preconsolidation pressure. **Time rate** is governed by the
coefficient of consolidation $c_v$.

## 4.5 Settlement of granular soils

In sands, consolidation is essentially immediate, and settlement is estimated from
**empirical correlations** with SPT $N$, CPT tip resistance, or **plate load tests**,
with corrections for footing width and water table. Because sands are notoriously
variable, these estimates carry wide uncertainty.

## 4.6 Tolerable movement and differential settlement

Design is governed not by absolute settlement but by:

- **total settlement** — must not impair the structure's function;
- **differential settlement** — the *difference* between adjacent points, which
  causes distortion, is usually the critical measure;
- **angular distortion** — differential settlement divided by the span between
  points.

Limits depend on the structure type (buildings, bridges, machinery) and are given in
the design manuals and codes.

## 4.7 Key takeaways

- **Settlement, not bearing capacity, usually governs** shallow-foundation design.
- Total settlement = **immediate + primary consolidation + secondary**.
- Use **elastic theory** for immediate, **consolidation theory** for clays,
  **empirical correlations** for sands.
- **Differential settlement and angular distortion** are the real serviceability
  criteria.
- Monitor actual settlement with **settlement platforms and extensometers** (see the
  [FHWA](../fhwa/index.md) reference).
