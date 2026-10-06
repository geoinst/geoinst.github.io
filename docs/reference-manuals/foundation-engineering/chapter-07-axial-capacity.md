---
lang: en
lang_alt: vi/reference-manuals/foundation-engineering/chapter-07-axial-capacity/
---
# Chapter 7 — Deep Foundations: Axial Capacity

## 7.1 The capacity equation

The **ultimate axial capacity** of a single pile is the sum of shaft and base
resistance:

$$Q_{ult} = Q_s + Q_p - W$$

where $Q_s$ is the **shaft (skin friction) resistance**, $Q_p$ the **end-bearing
(toe) resistance**, and $W$ the pile weight (often neglected). The **allowable
capacity** is $Q_{ult}$ divided by a factor of safety, and must also satisfy the
settlement criterion.

## 7.2 Shaft resistance in clay

In clay, shaft resistance is usually computed with the **total-stress (α) method**:

$$Q_s = \alpha \, c_u \, A_s$$

where $c_u$ is the undrained shear strength, $A_s$ the shaft area, and $\alpha$ an
adhesion factor (typically ~0.5, decreasing with $c_u$). The **effective-stress
(β) method** is also used, especially for long-term conditions.

## 7.3 Shaft resistance in sand

In sand, shaft resistance is computed with the **effective-stress (β) method**:

$$Q_s = \beta \, \sigma'_v \, A_s = K \tan\delta \, \sigma'_v \, A_s$$

where $\sigma'_v$ is the effective vertical stress, $K$ the lateral earth-pressure
coefficient, and $\delta$ the pile–soil friction angle. The **λ** and **α** methods
are alternatives for specific conditions.

## 7.4 End bearing

End bearing depends on whether the pile tip rests on rock, dense sand, or clay:

- **In clay:** $Q_p = 9 \, c_u \, A_p$ (with $c_u$ at the base).
- **In sand:** $Q_p = q'N_q A_p$ (or correlations with SPT/CPT), capped to account
  for the limited depth over which the bearing pressure mobilizes.
- **On rock:** capacity from the rock's unconfined compressive strength with
  reduction factors.

## 7.5 Capacity from in-situ tests

Static analysis is checked and often calibrated against field tests:

- **SPT and CPT correlations** — capacity estimated from penetration resistance.
- **Static pile load tests** — the definitive measurement, with the load applied in
  increments and settlement recorded.
- **Dynamic testing (PDA)** — high-strain dynamic tests during driving give
  capacity and integrity.
- **Statnamic and rapid load tests** — alternatives where static testing is
  impractical.

## 7.6 Instrumented load tests

The most informative load tests are **instrumented**: strain gages or **sister
bars** along the shaft and **telltales** or **extensometers** measure the load
distribution between shaft and toe, separating the two components directly (see the
[FHWA](../fhwa/index.md) reference, Chapter 8, and **Appendix D** examples).

## 7.7 Factors of safety and LRFD

Allowable-stress design uses a factor of safety on the ultimate capacity (commonly
2.5–4 for working loads). **LRFD** instead applies **resistance factors** to the
shaft and base components separately, reflecting their different reliability.

## 7.8 Key takeaways

- **$Q_{ult} = Q_s + Q_p$** — shaft friction plus end bearing.
- Use the **α/β/λ methods** for shaft, and **9$c_u$ / $q'N_q$** for base.
- **Calibrate** static analysis with **load tests, SPT/CPT correlations, and dynamic
  testing**.
- **Instrumented load tests** separate shaft from toe — the gold standard.
- Allowable-stress uses a **factor of safety**; LRFD uses **resistance factors**.
