---
lang: en
lang_alt: vi/reference-manuals/foundation-engineering/chapter-03-bearing-capacity/
---
# Chapter 3 — Shallow Foundations: Bearing Capacity

## 3.1 The bearing-capacity problem

A shallow foundation (typically a footing with depth $D_f$ less than its width $B$)
must transfer the structural load to the ground without **shear failure** of the
supporting soil. The **ultimate bearing capacity** $q_{ult}$ is the pressure at
which the soil fails; the **allowable bearing pressure** is $q_{ult}$ divided by a
factor of safety, also checked against settlement
([Chapter 4](chapter-04-settlement.md)).

## 3.2 Failure modes

Bearing failure occurs in one of three ways, depending on soil density and
compressibility:

- **General shear** — a well-defined wedge and slip surface; a sudden, brittle
  failure. Typical of dense sands and stiff clays.
- **Local shear** — a less developed slip surface with significant settlement before
  failure. Typical of medium-dense soils.
- **Punching shear** — the footing punches into the soil with little surface heave.
  Typical of loose sands and soft clays.

![Figure: foundation-bearing-failure](../../assets/figures/foundation-bearing-failure.svg)

**Figure.** Bearing-capacity failure modes: general shear (brittle), local shear, and punching shear (ductile) (after USACE EM 1110-1-1905).

## 3.3 The bearing-capacity equation

The classical solution expresses $q_{ult}$ as a sum of three terms:

$$q_{ult} = c N_c s_c + q N_q s_q + \tfrac{1}{2} \gamma B N_\gamma s_\gamma$$

where $c$ is cohesion, $q$ is the surcharge at foundation level, $\gamma$ is the
unit weight, $B$ is the footing width, $N_c, N_q, N_\gamma$ are **bearing-capacity
factors** (functions of the friction angle), and the $s$ terms are **shape factors**.
Several formulations are in use — **Terzaghi**, **Meyerhof**, **Hansen**, and
**Vesić** — differing in the factors and in how they treat shape, depth, inclination,
and eccentricity.

## 3.4 The water table

Groundwater reduces the effective stress in the failure zone, lowering capacity.
The two extremes are:

- water table **at the base** of the footing, and
- water table **at the ground surface**.

In between, the unit weight terms are reduced by a factor depending on the depth of
the water table relative to $B$. The design must use the **highest anticipated water
level** for the critical (lowest) capacity.

## 3.5 Eccentric and inclined loads

Real footings carry **eccentric** loads (moments) and sometimes **inclined** loads.
The standard approach is to replace the actual footing with an **effective area**
$B' \times L'$ (Meyerhof), centred under the load resultant, and to apply
inclination factors. Eccentricity reduces both the effective bearing area and the
capacity.

## 3.6 Bearing capacity from in-situ tests

Where samples are difficult, capacity is estimated from field tests:

- **SPT** — correlations between $N$ and allowable pressure, adjusted for water
  table and overburden.
- **CPT** — capacity from cone tip resistance.
- **Plate load test** — a direct, in-situ measurement of the load–settlement
  response of the actual soil, extrapolated to the prototype footing with care.

## 3.7 Key takeaways

- **Ultimate capacity ÷ factor of safety = allowable pressure** — but settlement
  often governs.
- Know the **failure mode**: general, local, or punching shear.
- The capacity equation is **three terms** (cohesion, surcharge, self-weight) with
  shape/depth/inclination factors.
- Use the **highest water table** in the design.
- Convert **eccentric loads** to an effective area.
- **Plate load tests** measure real soil response; use them with judgment.
