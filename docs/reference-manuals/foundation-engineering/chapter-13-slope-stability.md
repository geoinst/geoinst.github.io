---
lang: en
lang_alt: vi/reference-manuals/foundation-engineering/chapter-13-slope-stability/
---
# Chapter 13 — Slope Stability

## 13.1 Why slopes fail

A slope fails when the **shear stress** along a potential slip surface exceeds the
**shear strength** of the soil. The **factor of safety** is the ratio of available
strength to mobilized stress:

$$F = \frac{\tau_{available}}{\tau_{mobilized}}$$

Failure can be **sudden** (brittle, in dense soils or rock) or **progressive** (soft
clays, weathered rock), and may be triggered by rainfall, excavation, loading, or
seismic action.

## 13.2 Infinite slopes

For a long, uniform slope where the slip surface is parallel to the surface, the
factor of safety has a closed-form solution. Two cases matter:

- **Dry or drained slope** — governed by the friction angle and slope angle.
- **With seepage** — pore pressures reduce effective stress and the factor of
  safety, often dramatically. This is why **drainage** is the primary stabilisation
  measure.

## 13.3 Finite slopes and the method of slices

Real slopes are analysed with **limit-equilibrium methods** that divide the potential
slip mass into **vertical slices**:

- **Ordinary method of slices (Fellenius)** — simple, conservative.
- **Bishop's simplified method** — accounts for interslice forces and is the
  workhorse of practice.
- **Spencer** and **Morgenstern–Price** — rigorous, satisfying all equilibrium
  conditions.

The analysis searches for the **critical slip surface** — the one giving the lowest
factor of safety. Computer methods (e.g. **STABL**, **SLOPE/W**) automate the
search.

![Figure: foundation-slope-stability](../../assets/figures/foundation-slope-stability.svg)

**Figure.** Slope stability by the method of slices: the driving and resisting forces on each slice, and the search for the critical slip surface (after USACE EM 1110-2-1902).

## 13.4 Short-term and long-term conditions

- **Short-term (undrained)** — immediately after construction or excavation, using
  **undrained shear strength** $c_u$; critical for soft clays.
- **Long-term (drained)** — after pore pressures equilibrate, using **effective
  stress** parameters $c', \phi'$; often critical in stiff clays and on slopes with
  seepage.

Both must be checked, and the **lower factor of safety** governs.

## 13.5 Stabilization methods

When a slope is unstable, options include:

- **Drainage** — surface and subsurface; the most effective and economical.
- **Regrading** — flattening the slope or adding a toe berm.
- **Retaining structures** — walls, sheet piles, or reinforced soil at the toe.
- **Ground improvement** — soil nails, anchors, or reinforcement
  ([Chapter 14](chapter-14-ground-improvement.md)).
- **Reinforcement** — soil nails, tie-backs, or geosynthetics.

## 13.6 Key takeaways

- Slopes fail when **shear stress exceeds shear strength**; the factor of safety is
  the ratio.
- **Seepage** reduces the factor of safety — **drainage** is the primary fix.
- Use the **method of slices** (Bishop for practice) and search for the **critical
  slip surface**.
- Check **short-term and long-term** conditions; the lower $F$ governs.
- Stabilize by **drainage, regrading, retaining structures, or reinforcement**.
