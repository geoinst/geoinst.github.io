---
lang: en
lang_alt: vi/reference-manuals/soil-mechanics/chapter-11-stiffness/
---
# Chapter 11 — Stiffness & Stress–Strain

## 11.1 Why stiffness matters

**Stiffness** — how much a soil deforms for a given stress change — governs
**settlement**, the **distribution of load** between structural elements, and the
**movement** around excavations. It is measured by a **modulus**, and unlike
strength, it is **highly nonlinear** and **strain-dependent**.

## 11.2 The elastic parameters

For small strains, soil is described by:

- **Young's modulus** $E$ — the slope of stress–strain in the loading direction.
- **Poisson's ratio** $\nu$ — the ratio of lateral to axial strain (typically 0.2–0.5;
  0.5 for undrained).
- **Shear modulus** $G = E / [2(1+\nu)]$ — the resistance to shear distortion, often
  the most useful parameter for dynamic and small-strain problems.
- **Bulk modulus** $K$ — resistance to volumetric change.

## 11.3 Nonlinearity and strain level

Soil stiffness **decreases** as strain increases:

- **Very small strain** ($< 0.001\%$) — maximum stiffness $G_0$ or $E_0$, measured by
  **seismic methods** (bender element, seismic CPT, MASW).
- **Small strain** — relevant to machine foundations and dynamic loading.
- **Working strain** ($0.01–1\%$) — relevant to most foundation settlement; stiffness
  is a fraction of $G_0$.
- **Large strain** — near failure; relevant to stability.

Design must use the modulus **appropriate to the strain level** of the problem — a
common source of error is using a single "modulus" for all cases.

## 11.4 Obtaining modulus values

- **Laboratory** — triaxial or oedometer tests give $E$ or constrained modulus over a
  strain range.
- **Field** — pressuremeter, dilatometer, plate load test, and **seismic** methods
  give in-situ values, often preferable because they avoid sampling disturbance.
- **Correlations** — with SPT $N$ or CPT tip resistance, useful as a first estimate.

## 11.5 Key takeaways

- **Stiffness governs settlement** and load distribution.
- Soil stiffness is **nonlinear and strain-dependent** — $G_0$ at small strain, far
  lower near failure.
- Use the modulus **appropriate to the strain level** of the problem.
- **Seismic methods** give the small-strain modulus; **field tests** give working
  values.
- **Correlations** with SPT/CPT are a starting point, not a substitute for testing.
