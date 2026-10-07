---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-02-intact-rock-strength/
---

# Chapter 2 — Intact Rock Strength & Laboratory Testing

## 2.1 Mechanical Testing of Intact Rock

Understanding intact rock strength provides the baseline upper boundary for all rock mass strength evaluations. The primary laboratory tests standardized by the International Society for Rock Mechanics (ISRM) and ASTM include:

1. **Uniaxial Compressive Strength (UCS / $\sigma_{ci}$)**: Performed on cylindrical core specimens with length-to-diameter ratio $L/D = 2.0 - 2.5$. Specimen ends must be ground flat within $0.02\text{ mm}$ to prevent premature edge spalling.
   
$$\sigma_{ci} = \frac{P_{\text{fail}}}{A}$$

2. **Brazilian Indirect Tensile Strength ($\sigma_t$)**: Compressing a circular rock disc across its diameter generates perpendicular uniform tensile stresses at the center:

$$\sigma_t = \frac{2 P}{\pi D t}$$

   Where $D$ is specimen diameter and $t$ is disc thickness. For most brittle rocks, uniaxial tensile strength is approximately $1/10$ to $1/20$ of its UCS ($\sigma_t \approx 0.05 - 0.10 \sigma_{ci}$).

3. **Triaxial Compressive Testing**: Cylindrical specimens jacketed in impermeable membranes subjected to confining fluid pressure ($\sigma_2 = \sigma_3$) while axial load ($\sigma_1$) is increased to failure.

---

## 2.2 The Hoek-Brown Failure Criterion for Intact Rock

In 1980, Evert Hoek and E.T. Brown introduced an empirical non-linear criterion linking major and minor principal stresses at peak failure for intact rock:

$$\sigma_1' = \sigma_3' + \sigma_{ci} \left( m_i \frac{\sigma_3'}{\sigma_{ci}} + 1 \right)^{0.5}$$

Where:
- $\sigma_1'$ = effective major principal stress at failure
- $\sigma_3'$ = effective minor principal stress (confining pressure)
- $\sigma_{ci}$ = uniaxial compressive strength of intact rock
- $m_i$ = petrographic material constant reflecting rock mineralogy, grain interlocking, and texture

### Typical Values of $m_i$ for Common Rock Types
| Rock Class | Rock Type | Typical $m_i \pm \text{sd}$ |
|------------|-----------|-----------------------------|
| **Igneous** | Granite | $32 \pm 3$ |
| | Basalt | $25 \pm 5$ |
| | Andesite | $25 \pm 5$ |
| **Sedimentary** | Sandstone | $17 \pm 4$ |
| | Siltstone | $7 \pm 2$ |
| | Shale | $6 \pm 2$ |
| | Limestone | $12 \pm 3$ |
| **Metamorphic** | Quartzite | $20 \pm 3$ |
| | Schist | $12 \pm 3$ |
| | Gneiss | $28 \pm 5$ |
| | Marble | $9 \pm 3$ |

---

## 2.3 Griffith Crack Theory & Brittle Fracture Initiation

Why is rock non-linear in triaxial compression? A.A. Griffith (1921, 1924) demonstrated that brittle failure initiates from pre-existing elliptical microcracks and grain boundary voids.

Under compressive stress fields:
1. Shear stresses along microcrack lips induce local tensile stress concentrations at crack tips.
2. When local tensile stress exceeds the molecular bond strength, wing cracks propagate stably in the direction of the major principal stress ($\sigma_1$).
3. **Crack Initiation Threshold ($\sigma_{ci,\text{init}} \approx 0.4 - 0.5 \sigma_{ci}$)**: Acoustic emissions increase; lateral strain deviates from linearity.
4. **Crack Damage Threshold ($\sigma_{cd} \approx 0.7 - 0.85 \sigma_{ci}$)**: Microcracks coalesce into macroscopic shear bands, volume strain transitions from compaction to volumetric dilation.
5. **Peak Failure ($\sigma_1 = \sigma_{\text{peak}}$)**: Full macroscopic shear rupture.

---

## 2.4 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Uniaxial compressive strength (UCS) | Cường độ nén đơn trục | Peak axial failure stress under zero confinement ($\sigma_3 = 0$) |
| Brazilian tensile test | Thí nghiệm ép chẻ kéo Brazil | Indirect tensile test compressing a circular rock disc diametrally |
| Confining pressure | Áp lực giam hãm | Minor principal stress ($\sigma_3$) applied laterally |
| Intact rock parameter $m_i$ | Thông số vật liệu đá nguyên vẹn $m_i$ | Empirical constant in Hoek-Brown criterion based on rock genesis |
| Volumetric dilation | Giãn nở thể tích | Expansion of rock volume under shear due to microcrack opening |
