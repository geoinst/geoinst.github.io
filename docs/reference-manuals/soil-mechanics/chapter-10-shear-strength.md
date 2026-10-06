---
lang: en
lang_alt: vi/reference-manuals/soil-mechanics/chapter-10-shear-strength/
---
# Chapter 10 — Shear Strength

## 10.1 The Mohr–Coulomb criterion

**Shear strength** is the soil's resistance to sliding — the property that governs
bearing capacity, slope stability, and earth pressure. The **Mohr–Coulomb** criterion
expresses it as:

$$\tau_f = c' + \sigma'_n \tan\phi'$$

where $c'$ is **effective cohesion**, $\sigma'_n$ is the **effective normal stress**,
and $\phi'$ is the **effective friction angle**. For total-stress (undrained)
conditions, the same form uses $c_u$ and $\phi_u = 0$:

$$\tau_f = c_u$$

![Figure: soil-mechanics-mohr-coulomb](../../assets/figures/soil-mechanics-mohr-coulomb.svg)

**Figure.** The Mohr–Coulomb failure envelope: shear strength $\tau_f = c' + \sigma'\tan\phi'$, with the failure circle tangent to the envelope (after FHWA-NHI-06-088).

## 10.2 Drained vs. undrained strength

The choice of strength parameters depends on **drainage**:

- **Drained** — pore pressures have equilibrated; use **effective** parameters
  $c', \phi'$. Critical for **long-term** conditions and for sands.
- **Undrained** — no drainage during loading; use **total** parameters, usually
  **$c_u$** with $\phi = 0$. Critical for **short-term** conditions in saturated
  clays.

The **lower factor of safety** from both governs the design.

## 10.3 Laboratory tests

- **Direct shear** — simple, gives $c'$ and $\phi'$; drainage controllable.
- **Triaxial compression** — the most versatile: **UU** (unconsolidated undrained)
  for $c_u$; **CU** (consolidated undrained) with pore-pressure measurement for
  effective parameters; **CD** (consolidated drained) for drained strength.
- **Unconfined compression** — a quick $c_u$ for clays.
- **Ring shear** — for residual strength on pre-existing slip surfaces.

## 10.4 Factors affecting shear strength

- **Density and stress history** — denser and more over-consolidated soils are
  stronger.
- **Cementation and structure** — natural bonding adds apparent cohesion.
- **Anisotropy and fissures** — strength varies with direction; fissures weaken the
  mass.
- **Rate of loading** — undrained strength depends on loading rate.
- **Residual strength** — on a pre-existing slip surface, strength drops to the
  **residual** value, which governs reactivated landslides.

## 10.5 Key takeaways

- **$\tau_f = c' + \sigma'\tan\phi'$** (effective) or **$\tau_f = c_u$** (undrained).
- Choose **drained vs. undrained** by the drainage condition; the lower $F$ governs.
- **Triaxial** tests give the full range: UU, CU, CD.
- Density, stress history, structure, and rate all affect strength.
- On slip surfaces, use **residual** strength.
