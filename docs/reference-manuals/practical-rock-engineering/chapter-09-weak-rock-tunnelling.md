---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-09-weak-rock-tunnelling/
---

# Chapter 9 — Tunnels in Weak Rock & Squeezing Ground

## 9.1 Squeezing Ground Mechanics

When deep tunnels are excavated through weak rock masses (shales, phyllites, schists, mudstones, or heavily sheared fault gouge), induced boundary tangential stresses ($\sigma_\theta$) exceed the rock mass compressive strength ($\sigma_{cm}$).

Under these conditions, the rock does not fail by brittle spalling. Instead, it undergoes **time-dependent ductile squeezing**—large plastic shear strains yielding inward into the opening, resulting in severe convergence ($> 5\% - 20\%$ of tunnel diameter), buckling of steel sets, and shear rupture of rigid concrete liners.

### Hoek's Squeezing Index:
Hoek and Marinos (2000) correlated the ratio of rock mass compressive strength to in-situ overburden stress ($\sigma_{cm} / \gamma H$) with expected tunnel diametral strain ($\epsilon = \Delta D / D$):

$$\frac{\sigma_{cm}}{\gamma H} = \frac{\sigma_{ci} \cdot s^a}{\gamma H}$$

| Ratio $\sigma_{cm} / \gamma H$ | Tunnel Strain $\Delta D / D$ | Severity Category & Operational Impact |
|--------------------------------|------------------------------|-----------------------------------------|
| $> 1.0$ | $< 1\%$ | Few support problems; standard rockbolts and mesh |
| $0.5 - 1.0$ | $1\% - 2.5\%$ | Minor squeezing; light steel sets or pattern bolts with shotcrete |
| $0.3 - 0.5$ | $2.5\% - 5\%$ | Moderate squeezing; heavy support installed close to face |
| $0.15 - 0.3$ | $5\% - 10\%$ | Severe squeezing; yielding steel arches, forepoling umbrellas |
| $< 0.15$ | $> 10\%$ | Very severe squeezing; face collapse, yielding slots in shotcrete |

---

## 9.2 The Convergence-Confinement Method (CCM)

The Convergence-Confinement Method is the standard analytical design framework coupling three fundamental curves:

```
Internal Support Pressure pi
      ^
  p_0 |  \ Ground Reaction Curve (GRC)
      |    \
      |      \        Support Characteristic Curve (SCC)
 p_eq |------- \-----/
      |         \   /
      |          \ / (Equilibrium Point: u_eq, p_eq)
      |           v
      +-------------------------> Radial Convergence u_r
                 u_0  u_eq
```

1. **Ground Reaction Curve (GRC)**: Shows the decrease in internal support pressure $p_i$ required to maintain equilibrium as radial wall convergence $u_r$ increases from initial state ($p_i = p_0, u_r = 0$) to unconfined state ($p_i = 0, u_r = u_{\max}$).
2. **Longitudinal Deformation Profile (LDP)**: Relates radial convergence $u_r(x)$ to distance from the advancing tunnel face $x$. Approximately $25 - 35\%$ of total convergence occurs *ahead* of the face before support can be installed.
3. **Support Characteristic Curve (SCC)**: Represents the elastic-plastic load-deformation response of the installed ground support (rockbolts, shotcrete, steel arches). Support must be installed at initial convergence $u_0$ corresponding to face setback distance.

---

## 9.3 Rigid vs. Yielding Ground Support Philosophy

Attempting to halt squeezing in severe ground with ultra-stiff, rigid liners is impossible; the immense rock mass thrust ($p_0 = \gamma H$) will crush any economically feasible concrete shell.

### The Modern Yielding Support Strategy:
1. **Ductile yielding elements**: Steel sets equipped with frictional sliding connections (TH-arches) or yielding steel canisters (LSC cylinders) that deform plastically under a controlled resistance force ($200 - 400\text{ kN}$).
2. **Longitudinal slots in shotcrete**: Gaps left in shotcrete lining parallel to the tunnel axis allow radial closure without inducing compressive crushing in the shotcrete shell. Once convergence stabilizes, the slots are concreted closed.
3. **Yielding rockbolts (Swellex, D-Bolts)**: Deform up to $15 - 20\%$ strain without tensile rupture, maintaining continuous confinement on the fractured plastic annulus.

---

## 9.4 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Squeezing ground | Đất đá ép lún | Time-dependent plastic inward deformation of rock under high overstress |
| Convergence-Confinement Method (CCM) | Phương pháp đường cong phản ứng nền (CCM) | Analytical framework balancing rock convergence with support reaction |
| Ground Reaction Curve (GRC) | Đường cong phản ứng nền (GRC) | Relationship between internal support pressure and radial wall displacement |
| Longitudinal Deformation Profile (LDP) | Biểu đồ biến dạng theo trục dọc hầm (LDP) | Radial wall convergence as a function of distance from advancing face |
| Yielding support | Kết cấu chống giữ dẻo hấp thu biến dạng | Ductile ground support designed to deform plastically without failing |
