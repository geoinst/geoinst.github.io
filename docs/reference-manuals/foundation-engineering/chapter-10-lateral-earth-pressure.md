---
lang: en
lang_alt: vi/reference-manuals/foundation-engineering/chapter-10-lateral-earth-pressure/
---
# Chapter 10 — Lateral Earth Pressure

## 10.1 The three states of earth pressure

The pressure that soil exerts on a retaining structure depends on how much the
structure is allowed to move:

- **At-rest pressure** ($K_0$) — the wall does not move; the soil is in its natural
  state. $K_0 \approx 1 - \sin\phi'$ for normally consolidated soils.
- **Active pressure** ($K_a$) — the wall moves *away* from the soil, which expands
  and relaxes to its minimum pressure. This is the *minimum* pressure a wall must
  resist.
- **Passive pressure** ($K_p$) — the wall moves *into* the soil, which compresses
  and pushes back with its *maximum* resistance. $K_p > K_0 > K_a$.

The three coefficients are related by $K_a = 1/K_p$ for a simple frictionless case,
and both depend on the **friction angle** $\phi'$ and wall friction $\delta$.

## 10.2 Rankine and Coulomb theories

Two classical theories give the pressure coefficients:

- **Rankine** — assumes a smooth, vertical wall and a horizontal backfill; simple
  and widely used.
- **Coulomb** — allows wall friction and inclined backfill, giving more realistic
  (and often lower active) pressures; solved graphically or analytically.

Both assume the soil reaches a **plastic state** and neglect the wall–soil
interaction stiffness, so they are limits rather than exact values.

## 10.3 Surcharge, water, and layered backfill

Real walls carry more than soil self-weight:

- **Surcharge** — uniform or point loads behind the wall (traffic, stockpiles,
  adjacent footings) add lateral pressure.
- **Water pressure** — groundwater behind a wall adds full hydrostatic pressure,
  often the dominant load. **Drainage** is essential; a wall designed for soil
  pressure alone can fail when it fills with water.
- **Layered and sloping backfill** — pressures are computed layer by layer.

## 10.4 Compaction-induced pressure

Compacting backfill *behind* a wall with heavy rollers can lock in **high lateral
pressures** that exceed the active value, especially near the surface. This is a
frequent cause of unexpected wall movement, and it must be accounted for in design
and in the compaction method.

## 10.5 Key takeaways

- Three states: **at-rest, active, passive** — active is the minimum, passive the
  maximum.
- **Rankine** is simple; **Coulomb** allows wall friction and inclined backfill.
- **Water is often the dominant load** — provide drainage.
- **Surcharge** behind a wall adds pressure; account for it.
- **Compaction** can lock in pressures above active — control the method.
