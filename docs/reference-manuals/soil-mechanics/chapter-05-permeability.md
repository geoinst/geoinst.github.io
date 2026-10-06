---
lang: en
lang_alt: vi/reference-manuals/soil-mechanics/chapter-05-permeability/
---
# Chapter 5 — Permeability

## 5.1 Darcy's law

Water flows through soil under a **hydraulic gradient** $i = \Delta h / L$. **Darcy's
law** states:

$$v = k i$$

where $v$ is the **discharge velocity** and $k$ is the **coefficient of
permeability**. The **seepage velocity** (through the voids) is $v / n$, where $n$
is porosity.

## 5.2 What controls permeability

Permeability depends on:

- **particle size and grading** — coarser, well-graded soils are more permeable;
- **void ratio** — more voids, more flow;
- **saturation** — unsaturated soils have much lower permeability;
- **soil structure** — fissures and layers can dominate.

Typical ranges span **ten orders of magnitude**: gravel ($10^{-2}$ m/s) down to clay
($10^{-10}$ m/s). This enormous range is why permeability is the hardest parameter
to estimate reliably.

## 5.3 Measuring permeability

- **Constant-head test** — for coarse, permeable soils.
- **Falling-head test** — for fine soils.
- **Field tests** — pumping tests, borehole tests, and **piezometer response**
  tests measure the in-situ value, which may differ greatly from the laboratory
  value because of structure and layering.

## 5.4 Layered soils

Where the soil is layered, flow is **anisotropic**:

- **Horizontal flow** is dominated by the most permeable layers (weighted by
  thickness).
- **Vertical flow** is dominated by the least permeable layers (weighted by
  reciprocal).

The result is usually **$k_h > k_v$**, sometimes by an order of magnitude, which
matters for consolidation rates and seepage.

## 5.5 Key takeaways

- **Darcy's law: $v = ki$** — flow is proportional to gradient.
- Permeability spans **ten orders of magnitude** — the hardest parameter to pin
  down.
- Measure it **in the field** where structure and layering matter.
- Layered soils are **anisotropic**: $k_h > k_v$.
- Permeability controls **seepage, consolidation rate, and drainage design**.
