---
lang: en
lang_alt: vi/reference-manuals/fhwa-mse-walls/chapter-10-references-appendices/
---
# Chapter 10 — References & Appendices

## References

The manual's reference list spans the reinforced-soil literature: Vidal's
original reinforced-earth work; the FHWA *Reinforced Soil Structures* volumes;
the AASHTO *Bridge Design Specifications*; geosynthetic design guidelines; and
the research literature on pullout, creep, durability, and connection strength.
It is the starting point for any parameter that must be justified beyond the
manual's own tables.

## Appendix A — Determination of pullout resistance factors

**A.1 Empirical procedures to determine $F^{*}$ and $\alpha$.** For routine
design, the pullout friction factor $F^{*}$ and the scale correction factor
$\alpha$ are obtained from the soil's friction angle and the reinforcement type,
using the manual's empirical charts. This is the default route when pullout tests
are not warranted.

**A.2 Experimental procedures to determine $F^{*}$ and $\alpha$.** Where the
soil–reinforcement combination is unusual, or where the empirical values are not
conservative, **pullout tests** are performed: the reinforcement is embedded in
the candidate fill and pulled out under a known normal stress, and $F^{*}$ (and,
for extensible reinforcement, $\alpha$) is back-calculated from the measured
resistance. The appendix gives the test setup, the interpretation, and the
normalization.

**A.3 Connection resistance and strength.** The connection between reinforcement
and facing may be the **weakest link** in the system. The appendix describes
connection tests for partial- and full-friction segmental block/reinforcement
connections, and how to derive the design connection strength from the
load–displacement and rupture data.

## Appendix B — Determination of the creep strength reduction factor

**B.1 Background.** Geosynthetic reinforcement creeps — it strains continuously
under sustained load — so its long-term strength is lower than its short-term
strength. The **creep reduction factor** $RF_{CR}$ quantifies the loss.

**B.2 Step-by-step procedures for extrapolating stress-rupture data.** Because a
structure must perform for decades, the long-term strength cannot be measured
directly. The appendix gives the standard procedure: run **stress-rupture tests**
at elevated temperatures, use **time–temperature superposition** (shift factors)
to construct a master curve, and **extrapolate** it to the design life to find
the creep limit load.

**B.3 Use of creep data from "similar" products.** Where product-specific data are
unavailable, data from similar polymers and structures may be used with
justification.

**B.4 Creep extrapolation examples.** Two fully worked extrapolations — one for a
**PET** (polyester) geosynthetic and one for a **polyolefin** (polypropylene/
polyethylene) geosynthetic — take raw stress-rupture data through shifting and
extrapolation to a creep limit load, and thence to $RF_{CR}$.

## Appendix C — Approximate cost range of geotextiles and geogrids

Dated cost ranges for geosynthetic reinforcement, for order-of-magnitude
estimating. Re-base to current local prices before use.

## Appendix D — Typical dimensions of steel reinforcements

Standard cross-sections, dimensions, and areas of the steel strips, bar mats,
and wire grids used in metallic-reinforced systems — the tabulated data behind
the corrosion-allowance calculation in
[Chapter 3](chapter-03-soil-reinforcement-principles.md).

## Appendix E — Example reinforced soil slope analysis with the RSS computer program

A complete worked reinforced-slope analysis using the FHWA RSS program: input
geometry and soil properties, the reinforcement layout, the critical-surface
search, and the resulting factor of safety — the computer counterpart to the
hand examples in [Chapter 7](chapter-07-design-rss.md).

## Key takeaways

- **Pullout factors** come from charts by default, from **tests** when the
  combination is unusual — Appendix A.
- **Creep strength** must be **extrapolated** from accelerated tests, not assumed
  — Appendix B.
- **Connection strength** can govern; test it — Appendix A.3.
- Cost data (Appendix C) and standard dimensions (Appendix D) are **dated
  reference data** — re-base and re-verify before use.
- Appendix E is the **worked computer analysis** that closes the design loop.

---

## Related reading in this knowledge base

- [FHWA Geotechnical Instrumentation Reference Manual](../fhwa/index.md) — the
  instrument families that Chapter 9's monitoring program selects from.
- [Dunnicliff — Geotechnical Instrumentation](../dunnicliff/index.md) — the
  systematic planning philosophy behind the monitoring program.
- [Foundation Engineering](../foundation-engineering/index.md) — earth pressure,
  retaining walls, and slope stability from the public-domain USACE/FHWA corpus.
- [Practical Rock Engineering](../practical-rock-engineering/index.md) — the
  rock-side counterpart for rock slopes, anchors, and shotcrete.
- [Monitoring Dam Performance](../monitoring-dam-performance/index.md) — how
  movement and pore-pressure data become decisions.
- [ADAQS (VI)](../../vi/adaqs/index.md) — automated monitoring and trigger
  levels for long-term surveillance.
