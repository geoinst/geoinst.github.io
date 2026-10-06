---
lang: en
lang_alt: vi/reference-manuals/soil-mechanics/chapter-08-stress-distribution/
---
# Chapter 8 — Stress Distribution in Soil

## 8.1 The problem

A foundation load spreads into the ground, so the **stress increase** $\Delta\sigma$
at depth is *less* than the applied pressure and is distributed over a *wider* area.
Quantifying $\Delta\sigma$ with depth is essential for **settlement** calculations
([Chapter 9](chapter-09-consolidation.md)) and for **bearing capacity**.

## 8.2 Boussinesq theory

**Boussinesq's solution** gives the stress increase in a homogeneous, elastic,
isotropic half-space due to a **point load** at the surface. From it, solutions are
built for:

- **uniformly loaded strip footings** (plane strain);
- **rectangular and circular footings**; and
- **any shape**, by superposition or influence charts.

The vertical stress increase beneath the **centre** of a flexible circular load of
radius $R$ at depth $z$ is a standard result, and rectangular-footing solutions are
tabulated as **influence factors**.

## 8.3 The 2:1 method and approximate rules

A simple, widely used approximation is the **2:1 method**, which spreads the load at
a slope of 2 vertical to 1 horizontal:

$$\Delta\sigma = \frac{Q}{(B+z)(L+z)}$$

It is crude but useful for a first estimate; more rigorous solutions are preferred
for important structures.

## 8.4 Newmark influence charts

**Newmark's influence chart** is a graphical tool: the loaded area is drawn to scale
over the chart, and the number of divisions covered gives the influence factor. It
handles irregular shapes that have no closed-form solution.

## 8.5 Stress bulbs and depth of influence

The **stress bulb** (or pressure bulb) is the contour within which $\Delta\sigma$
exceeds a chosen fraction of the applied pressure (e.g. 10% or 20%). It shows:

- the **depth of significant influence** — how deep to explore and to which layer
  settlement must be computed;
- the **lateral extent** — how far adjacent structures or utilities may be affected.

As a rule, the depth of influence is on the order of **2 to 4 times the footing
width**.

## 8.6 Key takeaways

- Foundation loads **spread and attenuate** with depth.
- **Boussinesq** theory and influence factors give $\Delta\sigma$ for common shapes.
- The **2:1 method** is a crude but useful approximation.
- **Newmark charts** handle irregular shapes.
- The **stress bulb** sets the depth of exploration and settlement computation
  (typically **2–4 B**).
