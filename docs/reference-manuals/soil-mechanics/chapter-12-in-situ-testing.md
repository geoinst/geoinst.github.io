---
lang: en
lang_alt: vi/reference-manuals/soil-mechanics/chapter-12-in-situ-testing/
---
# Chapter 12 — In-Situ Testing & Parameter Selection

## 12.1 Why test in situ

Laboratory tests are run on small, disturbed samples. **In-situ tests** measure the
soil in its natural state, over a larger volume, avoiding sampling disturbance. They
are often the **primary** source of design parameters, with laboratory tests used to
confirm and refine.

## 12.2 The main in-situ tests

- **Standard Penetration Test (SPT)** — a split-spoon sampler driven by a 63.5 kg
  hammer; the blow count $N$ indexes density and strength. Cheap, universal, but
  crude and operator-sensitive.
- **Cone Penetration Test (CPT / CPTu)** — a cone pushed continuously, measuring tip
  resistance, sleeve friction, and (with a piezocone) pore pressure. Excellent for
  profiling and for **soft soils**.
- **Vane shear test (VST)** — measures undrained strength $c_u$ in soft clays.
- **Pressuremeter (PMT)** — expands a cylindrical probe to give in-situ modulus and
  strength.
- **Dilatometer (DMT)** — a flat blade pushed into the soil gives soil type and
  parameters.
- **Plate load test** — a direct measure of the load–settlement response.

## 12.3 Correlations

Many parameters are estimated from SPT or CPT through **empirical correlations**:

- friction angle $\phi'$ and relative density from $N$ or $q_c$;
- undrained strength $c_u$ from $N$ or cone resistance;
- modulus $E$ from $N$ or $q_c$;
- **liquefaction resistance** from $N$ or $q_c$ and the cyclic stress ratio.

Correlations are **region- and soil-specific**; they must be used with judgment and
verified locally.

## 12.4 Selecting design parameters

Parameter selection is an **engineering judgment**, not a lookup:

- **Bound the uncertainty** — use the range of measured values, not a single number.
- **Match the parameter to the analysis** — drained vs. undrained, peak vs. residual,
  small-strain vs. working-strain stiffness.
- **Prefer direct measurement** over correlation where the parameter is critical.
- **Consider variability and scale** — a small sample may not represent the mass.
- **Document the basis** — record how each parameter was chosen.

## 12.5 Key takeaways

- **In-situ tests** measure undisturbed soil over a large volume — often the primary
  source of parameters.
- **SPT** is universal and crude; **CPT** is precise and continuous; **VST, PMT, DMT**
  target specific parameters.
- **Correlations** are useful but region-specific — verify locally.
- Select parameters by **judgment**: bound uncertainty, match the analysis, prefer
  measurement, and document the basis.
