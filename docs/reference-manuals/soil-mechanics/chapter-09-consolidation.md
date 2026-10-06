---
lang: en
lang_alt: vi/reference-manuals/soil-mechanics/chapter-09-consolidation/
---
# Chapter 9 — Consolidation

## 9.1 What consolidation is

**Consolidation** is the **time-dependent** volume change of a saturated fine-grained
soil as **excess pore pressure dissipates** and the load transfers from the water to
the solid skeleton. It is the mechanism behind the long-term settlement of clays and
is governed by **Terzaghi's one-dimensional consolidation theory**.

## 9.2 The oedometer test

The **one-dimensional consolidation test (oedometer)** loads a confined sample in
stages and records the compression with time. From it come:

- the **compression index** $C_c$ (virgin compression slope);
- the **recompression index** $C_r$ (unloading–reloading slope);
- the **preconsolidation pressure** $\sigma'_p$ — the maximum past effective stress;
- the **coefficient of consolidation** $c_v$ — the rate parameter.

## 9.3 Magnitude of settlement

For a normally consolidated clay, the primary consolidation settlement is:

$$S_c = \frac{C_c H}{1+e_0}\log\frac{\sigma'_{v0}+\Delta\sigma}{\sigma'_{v0}}$$

For an over-consolidated clay, the **recompression index** is used up to
$\sigma'_p$, and $C_c$ beyond it. The **over-consolidation ratio** $OCR =
\sigma'_p / \sigma'_{v0}$ tells whether the clay is NC ($OCR=1$) or OC ($OCR>1$).

![Figure: soil-mechanics-consolidation](../../assets/figures/soil-mechanics-consolidation.svg)

**Figure.** Consolidation: the e–log σ′ curve giving $C_c$, $C_r$, and the preconsolidation pressure, and the time–settlement curve from which $c_v$ is derived (after USACE EM 1110-1-1904).

## 9.4 Rate of consolidation

The **rate** is governed by the **coefficient of consolidation** $c_v$ and the
**drainage path length**. The **time factor** $T_v = c_v t / H_{dr}^2$ relates
degree of consolidation $U$ to time. Because $H_{dr}$ appears squared, **doubling
the drainage path quadruples the time** — the reason **vertical drains**
([Chapter 14](chapter-14-testing-program.md)) accelerate consolidation so
dramatically.

## 9.5 Secondary compression

After primary consolidation, **secondary compression (creep)** continues at roughly
constant effective stress. It is significant in **organic and soft clays** and is
described by the **secondary compression index** $C_\alpha$. For some soils it
dominates the long-term settlement.

## 9.6 Key takeaways

- **Consolidation** is time-dependent settlement from **pore-pressure dissipation**.
- The **oedometer** gives $C_c$, $C_r$, $\sigma'_p$, and $c_v$.
- Settlement magnitude follows the **$C_c$ / $C_r$ logarithmic** formula.
- **Rate** is governed by $c_v$ and the **drainage path** ($T_v = c_v t / H_{dr}^2$).
- **Secondary compression** can dominate in organic soils.
