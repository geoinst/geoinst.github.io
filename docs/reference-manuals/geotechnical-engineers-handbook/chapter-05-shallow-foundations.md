---
lang: en
lang_alt: vi/reference-manuals/cam-nang-ky-su-dia-ky-thuat/chapter-05-shallow-foundations/
---
# Chapter 5 — Shallow Foundation Analysis

Chapter V is the first of the analysis chapters. It defines a shallow foundation, then
covers bearing capacity from several independent methods and settlement from several
independent methods — the two checks every shallow foundation must pass.

## 5.1 Basic concepts

### 5.1.1 Definition of a shallow foundation

The handbook uses the geometry of the foundation itself:

- **Footing width** $B$, **footing length** $L$, **embedment depth** $D$ (measured from
  the base to ground surface).
- A foundation is **shallow** when $\dfrac{D}{B} < 4$.
- A **strip footing** (móng băng) has $\dfrac{L}{B} > 5$.
- An **isolated footing** (móng đơn) has $\dfrac{L}{B} < 5$.
- Special shapes: circular $B = 2R$; square $B = L$; rectangular $B < L < 5B$.
- A **mat / raft** (móng bè) is a large foundation carrying a whole structure or part of
  it.

The handbook notes these limits are **relative**, not absolute.

### 5.1.2 Behaviour of a shallow foundation under load

Foundation displacement depends on the level of loading. The **load–settlement curve**
(đường quan hệ tải trọng – chuyển vị) identifies:

- the **ultimate load** $Q_L$ — the maximum load the foundation can carry before the
  soil fails;
- the **allowable load** — the load giving acceptable settlement and an adequate factor
  of safety against $Q_L$.

### 5.1.3 Failure of the foundation soil

The failure mechanism beneath a shallow foundation — general shear, local shear,
punching — and how the failure surface develops.

### 5.1.4 Ultimate load on a horizontal strip footing in uniform ground

The general ultimate-load formula for a centred vertical load on a horizontal strip
footing in homogeneous soil, from which the classical bearing-capacity equations are
derived.

![Figure: foundation-bearing-failure](../../assets/figures/foundation-bearing-failure.svg)

**Figure.** Bearing-capacity failure mechanisms beneath a shallow foundation.

## 5.2 Bearing capacity of shallow foundations

The handbook deliberately gives **several independent routes** to the same answer, so
that results can be cross-checked:

### 5.2.1 From soil-mechanics theory
The classical theoretical bearing-capacity solution.

### 5.2.2 From the cone penetration test (CPT)
Empirical correlations between cone resistance $q_c$ and bearing capacity.

### 5.2.3 From the Menard pressuremeter (PMT)
Using the limit pressure $P_l$ and pressuremeter modulus $E_p$.

### 5.2.4 From the SPT
Using the blow count $N$ — the most common route in Vietnamese practice.

### 5.2.5 On rock
Bearing capacity of a footing founded on rock.

## 5.3 Settlement of shallow foundations

### 5.3.1 Stress distribution beneath the foundation — Boussinesq
The elastic (Boussinesq) stress distribution used to find the increase in vertical stress
with depth.

### 5.3.2 Consolidation settlement by the layer-summation method
Dividing the compressible stratum into sub-layers and summing their contributions.

![Figure: foundation-settlement](../../assets/figures/foundation-settlement.svg)

**Figure.** Settlement components beneath a footing.

### 5.3.3 Elastic settlement by the general method
### 5.3.4 Settlement from the Menard pressuremeter
### 5.3.5 A rapid method for estimating settlement
### 5.3.6 Allowable settlement

## 5.4 Terminology

| English | Vietnamese (book) |
| --- | --- |
| shallow foundation | móng nông |
| strip footing | móng băng |
| isolated / pad footing | móng đơn |
| mat / raft | móng bè |
| embedment depth | chiều sâu chôn móng |
| ultimate load | tải trọng giới hạn |
| allowable bearing pressure | áp lực cho phép |
| bearing capacity | sức chịu tải |
| load–settlement curve | đường quan hệ tải trọng – chuyển vị |
| settlement | độ lún |
| layer-summation method | phương pháp phân tầng |
| allowable settlement | độ lún cho phép |

## 5.5 Key takeaways

- Shallow vs deep is defined by **$D/B < 4$**; strip vs isolated by **$L/B$**.
- Design has **two independent checks**: bearing capacity and settlement.
- The handbook gives **multiple methods for each** so results can be cross-checked —
  theory, **CPT**, **PMT**, **SPT**, rock.
- **SPT** is the most widely used route in Vietnamese practice.
- Settlement prediction rests on **Boussinesq** stress distribution plus
  **layer-summation** (or the pressuremeter method).
