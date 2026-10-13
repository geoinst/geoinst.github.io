---
lang: en
lang_alt: vi/reference-manuals/fhwa-mse-walls/chapter-03-soil-reinforcement-principles/
---
# Chapter 3 — Soil Reinforcement Principles & System Design Properties

## 3.1 Overview

This chapter is the bridge between choosing a system and designing it. It answers
two questions:

1. **Why does reinforced soil work?** — the interaction mechanics.
2. **What properties go into the equations?** — the soil, reinforcement, and
   durability parameters that the design chapters consume.

## 3.2 Reinforced soil concepts

A frictional fill can carry compressive stress and shear, but almost no tension.
A reinforcement element can carry tension, but almost no compression. Combine
them and the composite can carry a *tensile* stress it could not carry alone —
which is why the reinforced mass behaves as if it had an **apparent cohesion**,
and can stand at an angle steeper than the fill's friction angle allows.

Two transfer mechanisms carry the load between soil and reinforcement:

- **Friction (and adhesion)** along the reinforcement surface — dominant for
  continuous strips and geotextiles.
- **Passive bearing** of soil against transverse members — dominant for grids,
  bar mats, and ribbed strips, and a significant contributor for geogrids.

The design consequence is the **pullout mechanism**: the reinforcement is held by
the soil over an *effective embedment length* behind the potential failure
surface, and the tension it carries is limited by the friction and bearing that
length can mobilize.

## 3.3 Soil–reinforcement interaction using normalized concepts

**Evaluation of pullout performance.** Pullout resistance is normalized so that
different reinforcement geometries can be compared. The pullout capacity of a
layer is expressed as

$$P_r = F^{*}\ \alpha\ \sigma_v\ L_e\ C\ R_c$$

where $F^{*}$ is the **pullout friction factor** (a dimensionless measure of
soil–reinforcement interaction), $\alpha$ is a **scale correction factor**,
$\sigma_v$ is the effective vertical stress, $L_e$ is the effective embedment
length behind the failure surface, $C$ is the reinforcement perimeter (or
effective perimeter), and $R_c$ is the **coverage ratio** (the fraction of the
reinforcement width that is actually in contact with soil, less than 1 for grids
and apertured geogrids).

The **pullout friction factor** $F^{*}$ is obtained either empirically from
measured soil friction angle and reinforcement type, or experimentally from
pullout tests (Appendix A):

- **Inextensible (steel) reinforcement** — $F^{*}$ is derived from the soil's
  friction angle, with ribbed strips adding a passive-bearing component.
- **Extensible (geosynthetic) reinforcement** — $F^{*}$ combines surface friction
  with passive bearing on the transverse members; the **scale correction factor**
  $\alpha$ accounts for the fact that extensible reinforcement mobilizes less
  than its full friction over long embedment lengths. $\alpha = 1.0$ for
  inextensible reinforcement; for geosynthetics it is taken as 1.0 near the
  surface and reduces with depth (a default of about 0.8 is commonly used).

**Estimate of pullout capacity in RSS and MSE structures.** The same $P_r$
expression is used for both structures, but the *effective embedment length*
$L_e$ is measured behind a different failure surface — the internal slip surface
for MSE walls and the critical slip surface for reinforced slopes. The available
resistance is then compared with the mobilized tension:

$$FS_{(PO)} = \frac{P_r}{T_{max}}$$

with the minimum factor of safety set by the design criteria (commonly
$FS_{(PO)} \ge 1.5$).

**Interface shear.** Where reinforcement passes across a *direct sliding* surface
or where the facing-to-reinforced-fill interface must transfer load, the
**interface shear strength** governs. It is characterized by an interface
friction angle, generally lower than the soil's own friction angle, and must be
used wherever sliding along a reinforcement plane is a credible mechanism.

## 3.4 Engineering properties from site exploration and testing

**Foundation soils.** The foundation beneath the reinforced mass carries the
weight of the whole structure and must satisfy bearing, sliding, settlement, and
global stability. Required properties: unit weight, shear strength (drained and
undrained), compressibility, and the depth to a competent bearing stratum.

**Reinforced backfill soil.** The reinforced fill is a **structural material**,
not just fill. It must be frictional and free-draining. The specification
typically limits:

- **Fines content** and **plasticity index** (plastic fines reduce friction and
  drain poorly).
- **Gradation** (to ensure drainage and workability).
- **Compaction** (to develop the design friction angle and limit settlement).

A typical granular fill might have a friction angle of 34°–40°; the design value
must be justified by testing, not assumed.

**Retained fill.** The soil behind the reinforced zone generates the earth
pressure the structure resists. Its unit weight and friction angle are design
inputs for external stability, and its drainage determines whether hydrostatic
pressures must be added.

**Electrochemical properties.** For **steel** reinforcement, the backfill's
corrosivity governs the sacrificial thickness and coating requirement; the manual
limits pH, resistivity, chlorides, sulphates, and organic content. For
**geosynthetic** reinforcement, the chemistry governs polymer durability, and
limits are likewise imposed. These limits are why "any granular fill" is not good
enough.

## 3.5 Establishment of structural design properties

**Geometric characteristics.** Reinforcement width, spacing (vertical and
horizontal), length, cross-sectional area, and (for grids) the aperture geometry
and rib dimensions. For steel, the cross-section is reduced over the design life
by corrosion (see below).

**Strength properties.** The reinforcement's design strength is its **long-term**
strength, not its short-term ultimate strength:

- **Steel** — the design tensile strength is the yield strength of the
  *remaining* cross-section after the **sacrificial corrosion loss** over the
  design life has been deducted. Both galvanized coating loss and carbon-steel
  loss must be accounted for, at rates that depend on the backfill's
  electrochemical properties.
- **Geosynthetics** — the allowable tensile strength is the ultimate strength
  reduced by partial factors:

$$T_{allow} = \frac{T_{ult}}{RF_{CR}\ \cdot\ RF_{ID}\ \cdot\ RF_{D}}$$

where $RF_{CR}$ is the **creep** reduction factor, $RF_{ID}$ the **installation
damage** factor, and $RF_{D}$ the **durability** (chemical/biological ageing)
factor. The manual provides default values (Table 11) that may be used only when
the reinforcement and fill meet specified minimum requirements; otherwise the
factors must be established by testing — creep from stress-rupture
extrapolation (Appendix B), installation damage from field-damage tests, and
durability from immersion tests.

**Connection strength.** Where the reinforcement is mechanically connected to the
facing, the **connection strength** (which may be lower than the reinforcement's
own strength) governs, and must be established by connection tests — see
[Chapter 4](chapter-04-design-mse-walls.md) and Appendix A.

## 3.6 Key takeaways

- The composite works because **friction and passive bearing** grip the
  reinforcement; every strength equation is a statement about that grip.
- Normalize pullout as $P_r = F^{*}\alpha\sigma_v L_e C R_c$, and check
  $FS_{(PO)} = P_r/T_{max}$ against the design minimum.
- The **reinforced fill is a structural material** — specify its gradation,
  plasticity, compaction, and electrochemistry.
- Use **long-term** reinforcement strength: steel loses cross-section to
  corrosion; geosynthetics lose strength to creep, installation damage, and
  ageing.
- Establish reduction factors by **testing** unless the default-value
  preconditions are met.
