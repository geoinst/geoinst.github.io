---
lang: en
lang_alt: vi/reference-manuals/tailings-dam-safety/chapter-15-oil-sands-northern-alberta/
---
# Chapter 15 — Case Study: Oil Sands Tailings Dams of Northern Alberta

!!! note "About this case study"
    This chapter is an **original case study** written for this reference. It
    synthesises publicly available practice guidance for the oil sands industry of
    northern Alberta — principally the CDA Bulletin article *"Application of CDA
    Dam Safety Guidelines to the Geotechnical Design of Oil Sands Tailings Dams in
    Northern Alberta"* (Eshraghian & Becker, Golder Associates, **Canadian Dam
    Association Bulletin, Winter 2016**) and the companion conference paper
    *"Application of Geotechnical Instrumentation in Monitoring In-Pit Dykes
    Performance"* (Soe Moe & Biggar, 2013). It is a **teaching case study**, not a
    reproduction of those sources and not a design document. The oil sands region
    is regulated by the **Alberta Energy Regulator (AER)** under the *Dam Safety
    Technical Guideline*; always work from the current AER/CEA guidance.

Oil sands tailings dams are, in the words of the source paper, *"among the world's
third largest proven oil reserves"* — a scale that makes their containment
structures some of the most demanding tailings dams anywhere. Yet they are **not
water-retention dams**, and the distinction is the whole point of this case study:
they are built over decades around an active mining operation, they contain a
material that can liquefy, and they are held to a dam-safety regime written with
water dams in mind. Applying that regime intelligently — rather than mechanically
— is the engineering story.

---

## 15.1 The setting: why northern Alberta is a special case

### 15.1.1 Location and scale

The oil sands deposits (bituminous sands) lie in **northern Alberta**, within the
**Athabasca** region primarily, with smaller areas in **Cold Lake** and **Peace
River**. Current economic conditions limit most active mining to deposits within
about **75 m of the surface**; roughly **20 % of the resource is accessible to
surface mining**, the rest by in-situ methods. The figure below (from Alberta
Geological Survey data, after Eshraghian & Becker) shows the three deposit areas.

> **Figure reference.** The source article's Figure 1 maps the Athabasca, Cold Lake
> and Peace River oil sands areas across Alberta. (Not reproduced here.)

### 15.1.2 The mining and extraction process

The oil sands operations include **mining, extraction, upgrading** and supporting
infrastructure. The **mining sequence** is a chain of disturbances:

1. **Overburden (sands, till, clay) is stripped and stockpiled** separately.
2. The **oil sands are mined** by truck-and-shovel, dragline or bucket-wheel
   excavator.
3. **Extraction** uses hot water, caustic and/or diluent, followed by
   **hydrotransport** and **primary and secondary separation**.
4. **Tailings** — sand, fines, water and residual bitumen — are piped as **slurry**
   to disposal areas.

The **mining schedule is dictated by the extraction plant**, not by the dam
engineer: sand, fines, overburden and coarse tailings are stored in different
facilities at different rates, and the sequence continues for decades.

### 15.1.3 Two climates, two histories (the geological context)

The geotechnical behaviour that matters is dominated by **glaciation**. The
Athabasca deposit is **mantled by glacial deposits**: low-plasticity **till** of the
**Murray Formation** (glaciolacustrine, younger than the Clearwater Formation) and
the **Clearwater Formation** clays beneath it, which are understood to be
**glacially over-consolidated** and **pre-sheared** under successive ice advances.
The clays' **closely spaced fissures** can control stability even though the clays
are otherwise strong — a lesson from glacial geology that recurs in every slope in
the region.

Two further geological facts drive design:

- **Karst** — the **Devonian Waterways Formation** below includes **limestone and
  anhydrite**; **dissolution** (karst) can control the geotechnical stability of
  tailings dams. (The **Fort McMurray** area is the site of an active collapse
  feature, the **"3 km subsidence"** documented in regional seismic-hazard work.)
- **Seismicity** — the Athabasca region is **as far as ~600 km from the Canadian
  Rocky Mountain seismic belt**, so ground motions are **regional**, not near-field.
  The **Krinitzsky–Chang (1996)** **McMurray Region Seismic Hazard Study** provides
  the seismic parameters on which modern design is based, and the **Geological
  Survey of Canada** assessment places the **Fort McMurray region among the
  lowest-probability seismic hazard areas of Canada** (National Building Code of
  Canada, Open File 4459).

---

## 15.2 Two dam traditions: water-retention vs oil sands

The organising insight of the source paper is that **CDA guidelines were written
for water-retention dams**, and oil sands tailings dams differ in ways that make
direct application inappropriate. Four contrasts matter:

| Dimension | Water-retention dam | Oil sands tailings dam |
|---|---|---|
| **Construction period** | Short (weeks to ~3 years) | **Decades** (20–50+ years of operation) |
| **Operating life** | Given, tens of years | Continues as long as the **operation** lives (design life 25–40 y, often longer) |
| **Design basis** | **Uses reservoir water level** as the load case | Has **no normal reservoir level**; the phreatic surface **moves** as the beach and pond change |
| **Failure consequence** | Flood from stored water | **Movement of tailings** (with or without free water) — environmental and reclamation consequence |

These differences cascade into how the **design flood**, **freeboard** and
**loading conditions** are treated. A tailings dam does not have a "normal water
level" in the water-dam sense; the design must instead follow the **operational
life of the sand dam**, with the phreatic surface maintained throughout that life.

---

## 15.3 Tailings deposits and dam types

Tailings are discharged as **slurry** into a disposal area. The **coarse fraction
(sand) settles out quickly**, building a **sand beach**; **fines settle out slowly**
and accumulate in the **tailings pond**. Depending on the **depositional method**
(spigotting, sub-aerial, sub-aqueous), four deposit types are recognised:

- **Sand tailings** — the coarse beach and dykes.
- **Fine tailings** (fluid fine tailings, FFT — see [Chapter 2](chapter-02-facilities-and-failures.md)).
- **Composite tailings** — sand and fines blended for **strength and fast
  reclamation**.
- **Soft tailings** — the fine, soft, low-density deposits in the pond centre.

The **tailings dams** themselves are built by the **conventional earthfill
techniques** of Chapter 2 — spigotting the sand and constructing dykes by
**sequential raising** — but with one constraint foreign to most tailings
practice: the **fill is often placed as a slurry** and **beach sand is often used
as placed** rather than dried and compacted, so the "fill" is much more like a
deposited, saturated material than a compacted embankment.

> **Cyclic deposition.** The largest downstream-consequence structures are
> typically the **external tailings dykes** — larger, higher
> **upstream-construction** dams containing **total tailings** (fine tailings and
> sand). During **early years**, an upstream tailings dyke **cannot sustain the
> full load**, so the **fines-to-sand ratio and deposition** are managed.

---

## 15.4 What fails, and why: the failure modes

The paper classifies oil sands tailings dam failure modes into **two families**:

1. **Internal dam failure** — failure surface **from inside the dam** and
   **continuing through** the dam and its foundation, **into the
   tailings**.
2. **Upstream-slope instability** — failure surface from **the dam crest towards
   the pond**, with the deposit **acting as a resisting mass**; during early
   construction, **a high phreatic surface close to the dam crest** can cause this.

To this, add the modes common to all tailings dams (Chapter 2):

- **Overtopping**, **external erosion**, **static liquefaction** of loose beach
  and sand layers, **seismic liquefaction** (though the region is of low
  seismicity), and **internal erosion and piping**.
- **Karst-driven instability** where the underlying Devonian limestone/anhydrite
  dissolves.

The paper's key design implication: **the deposit itself must be included in the
stability analyses**, because the **tailings pond and beach impose a load and a
pore-pressure field** on the dam. A water-retention dam is analysed with water on
one side; a tailings dam must be analysed with **a heterogeneous, changing,
potentially liquefiable material** on one side.

---

## 15.5 Applying the CDA guidelines: what transfers, what must change

The paper systematically maps the **CDA (2007) Guidelines loading cases** against
what oil sands dams actually experience. The result is the practical heart of the
case study.

| CDA (2007) case | Water dam | Oil sands dam | Comment |
|---|---|---|---|
| **During and of construction** | Static loading + operating-basis static during dam raising | **1.3 / 1.3** | The dam must withstand static loads **during construction and operation due to gravity** applied to the dam |
| **Long-term** | Piezometric surface at maximum (long-term) operation | **1.5 / 1.5** | Long-term design assumes **the phreatic surface reverts to a natural (no-free-water) level** — there is no permanent reservoir |
| **Full or partial rapid drawdown** | 1.2–1.3 / 1.2–1.3 | **Not applicable** | Oil sands dams have **no mechanism** for a controlled reservoir drawdown, so this case does not apply |
| **Seismic (pseudo-static / post-earthquake)** | 1.0 / 1.0 | 1.2–1.3 / 1.2–1.3 | Lower probability but **high consequence**; design assumes tailings that are **susceptible to liquefaction** |

**Seepage considerations (the paper's §4.3).** Because the deposit and dykes are
saturated, the paper treats **seepage** as second in importance only to stability:

- **Steady-state seepage** through the dam, dykes and foundation is analysed with
  **flow nets or numerical methods**.
- **Under-drainage, drains and collection systems** are provided and maintained.
- A **high phreatic surface** can develop **active seepage and reduce stability**;
  a **low phreatic surface** reduces that risk.
- The **pond-filling method** (sub-aqueous deposition) itself **reduces seepage**.

**Seismic considerations.** Although the Athabasca region has **low seismicity**,
the **high consequence of failure** means **pseudostatic and post-earthquake**
analyses are warranted. The paper notes that a **limit-equilibrium stability
analysis is adequate** for most dam design, and that the **target minimum factor of
safety** for each case is set accordingly — but that **more sophisticated methods**
(and **in-situ testing** to estimate susceptibility) may be needed for
liquefaction-prone deposits.

> **Acceptable factors of safety.** The paper's Table 1 (reproduced in concept
> above) gives the **minimum target factors of safety** for water and oil sands
> tailings dams side by side. Note the explicit statement that **oil sands dams
> built using fill placement methods are not analysed using the same factor of
> safety as water-retention dams**, and that the factors are **target minimums**,
> not guarantees.

---

## 15.6 Operational challenges: the observational approach

The paper's §5 is about **operational practice**, and it is where a design case
study becomes a monitoring case study.

### 15.6.1 The case for the observational approach

Because the **operating life and raising rates of oil sands dams** change throughout
the long construction period, the paper argues that the **observational approach** (the
"learn-as-you-go" method formalised by Peck, 1969) is **more appropriate to oil
sands dams than to water-retention dams**. The approach maximises design
efficiency by **updating analyses from measured performance**; **unlike most
water-retention dams**, whose conditions change little after construction, oil
sands conditions **change continuously**.

The method's pre-conditions are demanding: the **engineer must identify
in advance what will happen and why**, predefine the **plan of action for every
credible departure**, and **continuously review** the monitoring against that
plan.

### 15.6.2 Performance monitoring

The paper stresses that monitoring must be **"in good detail and frequently
consistent with the design"** — and flags the trap that **observational
monitoring for dams during initial fill has not always been well done**. The
monitoring plan should:

- **Confirm the design** — verify each safety assumption.
- **Supplement** — detect departures early.
- **Fit the timeline** — be appropriate to the **planned pace** of the dam
  (initial fill, early operation, long-term).
- **Relate to the observational approach** — linked to a **risk assessment
  methodology** so that management can act.

### 15.6.3 Development of tailings liquefaction and the fills/consequences

The paper connects **depositional method to liquefaction**. Where tailings are
deposited **sub-aqueously**, the pond is **saturated and loose**, and **static
liquefaction** is possible for the **fragile, low-density** material. Whatever the
deposition method, **monitoring of pore pressure** and **deposit density** is the
core of liquefaction control (Chapter 6).

### 15.6.4 In-situ testing to verify the design

The paper's §5.4 is a practical contribution: **in-situ testing** (CPT, CPTu,
seismic cone, etc.) to **verify the deposit's state** (density, strength,
liquefaction susceptibility) **is essential** and is done **during operations**,
not just at design. As the paper says: *"The purpose of in-situ testing is to
verify the design and assumptions... and to build confidence that the design basis
and assumptions can be achieved."* This is the observational approach applied to
the **deposit** as well as to the **dam**.

---

## 15.7 The in-pit dyke experience: monitoring in practice (Albian)

The companion paper — *"Application of Geotechnical Instrumentation in Monitoring
In-Pit Dykes Performance"* (Soe Moe & Biggar, 2013) — reports how this playbook is
executed at the **CNRL Albian** in-pit dykes in the Athabasca region. This is the
closest thing to a **site-level case study** available in the public record, and it
shows the theory in operation:

- **Instrumentation matched to failure modes.** Piezometers (vibrating-wire,
  typically) to track **pore pressure and phreatic surface**; **inclinometers
  and settlement gauges** to track **deformation**; **survey monuments** for
  surface movement — all tied to the identified failure modes and reported against
  thresholds.
- **In-pit dykes** are built **inside the mined-out pit** and raised with the
  operation, so their behaviour is intimately coupled to **the deposition
  sequence** and to **the pit floor geology**.
- **Monitoring as construction control.** Because the fill is deposited and the
  deposit changes, monitoring is not merely verification — it is **part of the
  construction method**, telling the operator when to advance, pause, or
  modify deposition.
- **The observational approach requires the monitoring to be fast enough** to
  detect a departure **in time to act** — a point the CDA paper makes explicitly.

---

## 15.8 The reclamation arc (what makes oil sands different)

Underlying all of this is a purpose a water dam does not share: **reclamation**.
As the paper's Figure 2 shows, a tailings dam is ultimately meant to become a
**"reclaimed landscape"** — the **tailings pond surface** is part of the closure
design, and the **dam itself becomes a landform**. This is why:

- The **deposit's long-term behaviour** (consolidation, strength gain, density)
  matters as much as the dam's.
- **Composite tailings** and **beach conditioning** are used to build strength for
  **fast reclamation**.
- The **"no water-retention dam"** framing is not just a legal nicety — the
  structure is not intended to hold a permanent reservoir at closure.

---

## 15.9 Lessons for any tailings engineer

Even outside northern Alberta, the case study teaches transferable lessons:

1. **Know which guideline you are inheriting.** The CDA case shows that a
   reputable dam-safety standard may need *interpretation* before it fits a
   tailings facility — and that **not all loading cases apply**.
2. **Let the operational reality shape the design.** Decades-long construction,
   rate-controlled deposition and a moving phreatic surface are design inputs,
   not details.
3. **Include the deposit in your analysis.** A tailings dam's "load" is a changing,
   often liquefiable material — analyse it, and **verify its state by in-situ
   testing**.
4. **Seepage is second only to stability.** Under-drainage, drains and pond
   management are structural, not cosmetic.
5. **Adopt the observational approach deliberately** — with predefined actions,
   fast enough monitoring and continuous review.
6. **Instrumentation is construction control**, not just compliance.
7. **Design for closure from day one** — the dam becomes the landform.

---

## 15.10 Key takeaways

- Oil sands tailings dams in northern Alberta are **large, decade-long,
  operation-driven structures** — not water-retention dams.
- **CDA guidelines apply, but require interpretation**: the design-flood,
  freeboard and **drawdown** cases do not transfer; grading is set by the **dam's
  actual loading cases**.
- **Tailings liquefaction, seepage, and karst** are the controlling geotechnical
  concerns; **seismicity is low but consequence is high**.
- The **observational approach** is more appropriate here than for water dams
  because conditions change continuously.
- **In-situ testing and performance monitoring** verify the design and underpin
  the observational approach.
- The **Albian in-pit dykes** demonstrate monitoring used as **construction
  control**.
- **Reclamation** is the purpose the design must serve.

---

## Sources

- **Eshraghian, A. & Becker, D.E. (Golder Associates)** — *Application of CDA Dam
  Safety Guidelines to the Geotechnical Design of Oil Sands Tailings Dams in
  Northern Alberta*, **Canadian Dam Association Bulletin, Winter 2016**, pp. 26–41.
- **Soe Moe, K.W. & Biggar, K.W. (2013)** — *Application of Geotechnical
  Instrumentation in Monitoring In-Pit Dykes Performance*, conference paper (CNRL
  Albian).
- **Canadian Dam Association (2007)** — *Dam Safety Guidelines* and *Technical
  Bulletin: Geotechnical Design of Dams*.
- **Alberta Energy Regulator** — *Dam Safety Technical Guideline* and
  *Guide to the Management of Tailings Facilities* (with MAC).
- **Krinitzsky & Chang (1996)** — *McMurray Region Seismic Hazard Study*.
- **Geological Survey of Canada** — *National Building Code of Canada seismic
  hazard*, Open File 4459.

> **Regulatory currency.** The AER Dam Safety Technical Guideline and the CDA
> guidelines are revised periodically. Verify the **current edition** before any
> design or submission.
