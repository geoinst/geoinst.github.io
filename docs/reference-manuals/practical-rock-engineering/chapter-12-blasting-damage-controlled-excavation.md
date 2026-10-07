---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-12-blasting-damage-controlled-excavation/
---

# Chapter 12 — Blasting Damage & Controlled Excavation Techniques

## 12.1 The Physics of Blast-Induced Rock Damage

Blasting fragments rock through two distinct physical processes:

1. **High-Velocity Shock Wave**: An instantaneous compressive shock pulse ($V_p \approx 3,000 - 6,000\text{ m/s}$) travels radially outward from the detonating borehole. As it reflects off free faces as a tensile wave, it creates extensive radial micro-cracks around the blasthole.
2. **Explosion Gas Expansion Pressure**: High-pressure, high-temperature gases ($P_{\text{gas}} \approx 1,000 - 5,000\text{ MPa}$) penetrate into the shock-induced radial cracks, wedging them open and heaving the fragmented rock forward into the void.

### The Blast Damage Zone:
In production blasting, over-confined charges shatter the rock well beyond the intended excavation boundary. This creates a **blast damage envelope** ($0.5 - 2.0\text{ m}$ depth behind highwalls and tunnel arches) characterized by dilated joint apertures, shattered intact bridges, and destroyed friction angles ($D \to 1.0$ in the Hoek-Brown criterion), triggering severe rockfalls.

---

## 12.2 Controlled Blasting Methods

To preserve the structural competence of final highwalls and tunnel perimeters, controlled perimeter blasting techniques are employed:

```
A. PRE-SPLITTING (Highwalls)                B. SMOOTH BLASTING (Tunnel Perimeters)
   [o] [o] [o] [o] [o]  (Uncharged buffer)     [X]  [X]  (Production rounds fire first)
    |   |   |   |   |                          \   /
   =================== (Shear crack split)      [o]-[o]-[o] (Perimeter holes fire LAST)
   Fired BEFORE production round                Cushioned charges trim final perimeter
```

| Technique | Drilling Configuration | Explosive Loading | Timing Sequence |
|-----------|------------------------|-------------------|-----------------|
| **Pre-Splitting** | Closely spaced holes ($s \approx 8 - 12 d_{\text{hole}}$) drilled along the final design boundary line | Decoupled, cushioned light charges (air-decked or trace explosive strings) | Fired **simultaneously BEFORE** any production blastholes detonate |
| **Smooth Blasting (Contour Blasting)** | Perimeter holes spaced closely ($s \approx 15 - 16 d_{\text{hole}}$) with burden-to-spacing ratio $B/s \approx 1.2 - 1.5$ | Light decoupled cartridge charges | Fired on the **LAST delay interval** after all interior burden rock has been excavated |
| **Cushion Blasting (Slashing)** | Single row of trimming holes drilled adjacent to final wall | Lightly charged with stemming cushions | Fired after the main muckpile has been removed to trim irregular bench edges |

---

## 12.3 Peak Particle Velocity (PPV) & Damage Thresholds

Vibration waves traveling through rock are quantified by **Peak Particle Velocity (PPV)** measured via 3-axis velocity seismographs (geophones):

### USBM Empirical Vibration Scaled Distance Law:

$$\text{PPV} = K \left( \frac{R}{\sqrt{Q}} \right)^{-B}$$

Where $R$ is distance to the blast point ($\text{m}$), $Q$ is maximum explosive charge weight per delay ($\text{kg}$), and $K, B$ are site transmission constants.

### Rock Mass Damage Criteria:
- **$\text{PPV} < 50\text{ mm/s}$**: Negligible risk to fresh rock; acceptable for nearby concrete lining and engineered infrastructure.
- **$\text{PPV} \approx 100 - 250\text{ mm/s}$**: Onset of minor joint opening and ravelling of loose keyblocks along unsupported roofs.
- **$\text{PPV} \approx 400 - 700\text{ mm/s}$**: Critical threshold for permanent damage; new tensile fractures initiate in intact rock bridges.
- **$\text{PPV} > 1,000\text{ mm/s}$**: Total shattering of intact rock; equivalent to the crushing zone around explosive blastholes.

---

## 12.4 Blast Vibration Monitoring Arrays

To prevent damaging highwalls and surrounding underground caverns:
- Install triaxial geophone arrays at the crest of open pit benches to ensure perimeter blasting does not exceed $\text{PPV} \le 150\text{ mm/s}$.
- Link seismographs to digital ADAQS gateways to generate instantaneous compliance reports and optimize electronic delay detonator sequences (millisecond timing intervals).

---

## 12.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Pre-splitting | Nổ mìn tạo khe trước / Nổ tách trước | Firing decoupled perimeter holes simultaneously prior to production blasting |
| Smooth blasting | Nổ mìn tạo biên nhẵn | Firing light perimeter charges on the final delay to produce a clean arch |
| Decoupled charge | Lượng thuốc nổ không tiếp xúc thành lỗ | Explosive charge whose diameter is smaller than the blasthole diameter |
| Peak Particle Velocity (PPV) | Vận tốc dao động hạt cực đại (PPV) | Maximum velocity of ground vibration particles during wave transit |
| Scaled distance | Khoảng cách tỷ lệ | Geometric ratio relating distance to the square root of explosive charge weight |
