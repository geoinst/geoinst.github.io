---
lang: en
lang_alt: vi/reference-manuals/cam-nang-ky-su-dia-ky-thuat/chapter-02-soil-properties/
---
# Chapter 2 — Engineering Properties of Foundation Soils

Chapter II is the soil-mechanics core of the handbook. It defines what "foundation
soil" means, then builds up from the three phases of soil to the physical indices, and
finally to the mechanical theories a designer needs.

## 2.1 What "construction soil" means

Soil (đất xây dựng) is a **three-phase system**: solid particles (hạt rắn), water
(nước) and gas/air (khí).

- If water fills every void, the soil is **saturated** (bão hoà).
- If the voids hold only air, the soil is **dry** (khô).
- If a void holds air but is sealed off from the atmosphere, that air is **occluded**
  (khí bị nhốt).

Solid particles form the **skeleton** (khung cốt liệu) of the soil. Special soils —
organic soil, peat, mud — contain organic matter that decomposes over time, giving
them very high compressibility and low strength.

## 2.2 Soil structure

### 2.2.1 Classification of solid particles

The handbook uses the **British Standard (BS)** grain-size classification:

| Fraction | Grain size $D$ |
| --- | --- |
| Boulders / cobbles (tảng, hòn) | $D > 200$ mm |
| Gravel (cuội sỏi) | $20 < D < 200$ mm |
| Coarse gravel / shingle (dăm sạn) | $2 < D < 20$ mm |
| Sand (cát) | $0.06 < D < 2$ mm |
| Silt (bụi) | $0.002 < D < 0.06$ mm |
| Clay (sét) | $D < 0.002$ mm |

Other systems place the clay/silt boundary at 0.005 mm or 0.002 mm, and the
silt/sand boundary at 0.075 mm or 0.06 mm — the boundaries are conventional. Beyond
size, two further factors matter: **grain shape** (rounded, angular, sub-rounded) and
the **mineral composition** of the particles.

### 2.2.2 Pore water and soil fabric

Water in the voids, and the way particles are arranged into a fabric, control
compressibility, permeability and strength.

## 2.3 Physical properties

### 2.3.1 The physical indices

Water content $w$, void ratio $e$, porosity $n$, unit weights $\gamma$, $\gamma_d$,
$\gamma_{sat}$, specific gravity $G_s$ — the standard index set.

### 2.3.2 Relationships between the indices

The indices are not independent: the handbook sets out the closed set of relationships
(phase relationships) that lets any index be derived from a few measured ones. These
are the same identities tabulated in the site's
[Soil Mechanics](../soil-mechanics/chapter-02-composition-index.md) reference.

## 2.4 Mechanical properties in outline

### 2.4.1 Elastic theory applied to soil

Soil is treated as an elastic half-space to obtain stress distributions.

### 2.4.2 Stress around a point — the Mohr circle

The state of stress at a point is represented by the **Mohr circle** (vòng tròn Mohr),
which gives the normal and shear stress on any plane through the point. This is the
basis of the strength criterion used throughout the book.

![Figure: soil-mechanics-mohr-coulomb](../../assets/figures/soil-mechanics-mohr-coulomb.svg)

**Figure.** Mohr–Coulomb failure envelope and Mohr circle (after FHWA-NHI-06-088).

### 2.4.3 Plastic-deformation theory for soil

Beyond the elastic range, soil deforms plastically; the handbook outlines the
plasticity framework used to describe yielding and failure.

### 2.4.4 Soil and Terzaghi's consolidation theory

**Consolidation** (cố kết) is the time-dependent compression of a saturated soil as
excess pore pressure dissipates and effective stress increases. Terzaghi's one-
dimensional theory is the foundation of settlement-versus-time prediction.

![Figure: soil-mechanics-consolidation](../../assets/figures/soil-mechanics-consolidation.svg)

**Figure.** Consolidation: $e$–$\log\sigma'$ curve and the time–settlement curve (after USACE EM 1110-1-1904).

### 2.4.5 Menard's theory for the pressuremeter test

The **pressuremeter** (nén ngang) expands a cylindrical probe in the borehole and
measures the pressure–volume response; Menard's theory converts that response into a
**pressuremeter modulus** $E_p$ and a limit pressure $P_l$ — inputs used later for
foundation and settlement analysis (Chapters 5–6).

## 2.5 Terminology

| English | Vietnamese (book) |
| --- | --- |
| three-phase system | hệ ba thành phần (hạt rắn, nước, khí) |
| saturated / dry soil | đất bão hoà / đất khô |
| occluded air | khí bị nhốt |
| soil skeleton | khung cốt liệu |
| grain-size distribution | phân loại hạt (theo cỡ hạt) |
| water content | độ ẩm |
| void ratio | hệ số rỗng |
| porosity | độ rỗng |
| unit weight (bulk / dry / saturated) | dung trọng (tự nhiên / khô / bão hoà) |
| specific gravity | tỷ trọng |
| Mohr circle | vòng tròn Mohr |
| consolidation | cố kết |
| effective stress | ứng suất hữu hiệu |
| pressuremeter modulus | mô đun nén ngang |

## 2.6 Key takeaways

- Soil is a **three-phase system**; the solid skeleton carries the load and the pore
  water carries the pressure.
- Grain-size boundaries are **conventional** — the BS set is used here.
- The physical indices form a **closed set of relationships**; a few measurements give
  the rest.
- The **Mohr circle** expresses stress at a point; the **Mohr–Coulomb** envelope gives
  strength.
- **Terzaghi consolidation** explains settlement over time; **Menard's theory** turns
  the pressuremeter curve into design parameters.
