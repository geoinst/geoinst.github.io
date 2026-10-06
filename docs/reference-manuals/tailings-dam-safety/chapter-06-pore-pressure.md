---
lang: en
lang_alt: vi/reference-manuals/tailings-dam-safety/chapter-06-pore-pressure/
---
# Chapter 6 — Pore Pressure and Liquefaction-Potential Monitoring

## 6.1 Why pore pressure is the central parameter

The dominant tailings failure mechanisms — **static and seismic liquefaction** —
are governed by pore pressure. When loose, saturated tailings carry high pore
pressure (low effective stress), they can lose strength catastrophically.
Monitoring pore pressure is therefore the cornerstone of tailings surveillance.

## 6.2 Piezometer types

| Type | Principle | Best for |
|------|----------|---------|
| **Vibrating-wire (VW)** | Frequency change of a tensioned wire | Long-term automated monitoring; robust |
| **Pneumatic** | Gas pressure balances water pressure | Remote, no power needed |
| **Standpipe (open)** | Water level in a pipe | Simple, direct, but slow to equilibrate |
| **Hydraulic (twin-tube)** | Liquid-column balance | Multiple points, established method |

## 6.3 Liquefaction potential indicators

Pore-pressure monitoring supports liquefaction assessment through:

- **Pore-pressure ratio** $r_u = u / \sigma'_v$ — the ratio of pore pressure to
  initial vertical effective stress; high or rising $r_u$ signals lost strength.
- **Excess pore pressure** generated during or after seismic events, measured by
  piezometers with fast response.
- **Correlation with in-situ tests** (SPT, CPT, shear-wave velocity) that
  characterize the looseness of the deposit.

!!! warning "Saturation is everything"
    A VW or pneumatic piezometer that is not saturated gives meaningless results.
    The **saturation** procedure — removing air from the porous filter and
    connecting tube — must be done carefully at installation ([Dunnicliff Ch. 9](../dunnicliff/index.md)).
    A never-properly-saturated piezometer is a silent gap in the program.

## 6.4 Placement

Piezometers are placed to detect the failure modes of [Chapter 2](chapter-02-facilities-and-failures.md):

- **Within the deposit and beach** to track the phreatic surface and zones of
  high $r_u$.
- **At the embankment toes** (especially upstream-method raises) to detect
  pressure buildup in the weakest material.
- **In the foundation** where weak or liquefiable layers are present.
- **Multiple depths** in a single borehole (multi-level / MPBX) to profile pore
  pressure with depth.

## 6.5 Reading and interpretation

Readings are converted to **piezometric head** (equivalent water-surface
elevation). Key interpretations:

- **Steady rise without a pond rise** → possible blockage, increased seepage, or
  sensor fault.
- **Pore-pressure lag** behind pond level → indicates drainage and permeability.
- **$r_u$ approaching values used in design** → liquefaction concern.
- **Rapid post-seismic excess pressure** → triggers immediate evaluation.

## 6.6 Common failures

- **Air ingress / loss of saturation** → drifting or unresponsive readings.
- **Borehole short-circuiting** → reads the wrong zone.
- **Cable / electronics damage** → the most common automated-instrument fault.

## 6.7 Key takeaways

- Pore pressure governs the dominant liquefaction failures.
- Track pore-pressure ratio $r_u$ as a liquefaction indicator.
- Saturate every piezometer correctly; verify it.
- Place instruments at the beach, toes, and foundation — where modes originate.
