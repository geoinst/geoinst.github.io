---
lang: en
lang_alt: vi/reference-manuals/cfem/chapter-25-instrumentation-monitoring/
---
# Chapter 25 — Geotechnical Instrumentation and Monitoring (Digest)

*Source: CFEM 2022 (4th Edition), Chapter 25, by Pierre Choquet, Dr.-Eng., P. Eng.
This page is an original digest with an **elaborated reference section**; it is not
a reproduction of the copyrighted chapter.*

Geotechnical design embraces uncertainty. That uncertainty is assessed during
construction and operation using instruments. Chapter 25 surveys the instruments
commonly used to monitor the short- and long-term behaviour of the ground
supporting man-made structures, together with the data-collection and acquisition
systems behind them.

The chapter is organised around **six measured parameters**, and this digest follows
that structure before turning to the *autonomous* half of the subject — how readings
are taken, transmitted, and presented without a person in the field.

---

## 25.1 — Introduction

The six principal monitoring parameters, and the instruments that measure them:

| Parameter | Typical instruments |
|---|---|
| **Groundwater pressure** | Piezometers (standpipe, vibrating-wire, pneumatic, push-in, fully-grouted) |
| **Displacement** (surface and depth; x, y, z; relative or absolute) | Extensometers, settlement gauges, inclinometers, tiltmeters, geodetic methods |
| **Strain** (on ground or structure surfaces, or embedded) | Strain gauges |
| **Load** (structural element → ground) | Load cells (tie-back anchors, test piles) |
| **Total pressure** (ground–structure contact) | Hydraulic total pressure cells |
| **Temperature** (surface, or profile with depth) | Thermistors |

The chapter also covers **geodetic methods** — total stations, levelling, differential
RTK GPS, and newer methods such as LiDAR, ground-based InSAR and satellite InSAR —
because they are used alongside geotechnical and structural instrumentation.

---

## 25.2 — Information sources *(elaborated)*

> **This is the section that makes the chapter a reference tool.** Rather than a
> plain bibliography, §25.2 is a *guided* reading list organised by document type.
> Below, each entry is grouped and annotated with what it is and why it matters.

### 25.2.1 — The foundational textbook

- ***Geotechnical Instrumentation for Monitoring Field Performance*** — **John
  Dunnicliff (1993)**, Wiley, 577 pp. — the discipline's standard work, universally
  known as the **"Red Book"**. Chapter 25 treats it as the single most recognised
  source in the field.
- **Dunnicliff's quarterly columns** in *Geotechnical News* (CGS) — 93 columns,
  indexed and searchable in the public section of the
  [CGS website](https://www.cgs.ca/instrumentation_news.html). A running practitioner
  archive that extends the book.

### 25.2.2 — Textbooks and major guideline volumes

| Reference | Coverage |
|---|---|
| **De Rubertis, K. (Ed.), 2018** — *Monitoring Dam Performance: Instrumentation and Measurements*, ASCE, 442 pp. | The chapter's main source for **metrological properties** (§25.5) and geodetic monitoring; the ASCE/USSD dam-safety reference |
| **Sharon, R. & Eberhardt, E. (Eds), 2020** — *Guidelines for Slope Performance Monitoring*, CSIRO Publishing / CRC Press, 331 pp. | Slope-specific monitoring philosophy and practice |
| **Stark, Oommen & Ning, 2021** — *Remote Sensing for Monitoring Embankments, Dams, and Slopes*, ASCE GSP 322, 114 pp. | Remote-sensing state of practice (InSAR, LiDAR, photogrammetry) |
| **ICE Manual of Geotechnical Engineering** (Burland et al., 2012) — Ch. 94 *Principles of Geotechnical Monitoring* (16 pp.) and Ch. 95 *Types of Geotechnical Instrumentation and Their Usage* (26 pp.) | A second canonical treatment; Ch. 94 also covers contract practices |
| **Walker & Awange, 2020** — *Surveying for Civil and Mine Engineers*, Springer, 411 pp. | Geodetic/surveying methods (§25.17) |
| **Glisic & Inaudi, 2007** — *Fibre Optic Methods for Structural Health Monitoring*, Wiley, 281 pp. | The reference for **fibre-optic sensing** (§25.4.4) |
| **Ferretti et al., 2007** — *InSAR Principles: Guidelines for SAR Interferometry Processing*, ESA TM-19 | The principles behind **satellite InSAR** (§25.17.5) |
| **Chartered Institution of Civil Engineering Surveyors, 2017** — *Client Guide to Instrumentation and Monitoring*, Survey Liaison Group, London, 28 pp. | Client-side procurement and scope guidance |

### 25.2.3 — Standards

**ASTM Subcommittee D18.23 (Field Instrumentation)** — the US standard test
methods and practices directly governing specific instruments:

| Standard | Subject |
|---|---|
| **D4403-20** | Standard Practice for Extensometers Used in Rock |
| **D6230-13** | Standard Test Method for Monitoring Ground Movement Using Probe-Type Inclinometers |
| **D6598-19** | Standard Guide for Installing and Operating Settlement Points for Monitoring Vertical Deformations |
| **D7299-12** | Standard Practice for Verifying Performance of a Vertical Inclinometer Probe |
| **D7764-12** | Standard Practice for Pre-Installation Acceptance Testing of Vibrating Wire Piezometers |

**ISO Technical Committee 182 / WG2 — the *ISO 18674* series** ("Geotechnical
investigation and testing — Geotechnical monitoring by field instrumentation"), the
international counterpart, published part by part:

| Part | Subject | Status at time of writing |
|---|---|---|
| **ISO 18674-1:2015** | Part 1: General rules | Published |
| **ISO 18674-2:2016** | Part 2: Measurements along a line — extensometers | Published |
| **ISO 18674-3:2017** | Part 3: Measurements across a line — inclinometers | Published |
| **ISO 18674-4** | Part 4: Measurement of pore water pressure — piezometers | Published |
| **ISO 18674-5** | Part 5: Stress change measurements by total pressure cells | Published |
| Part 6 / 7 / 8 / 9 | Hydraulic settlement gauges / strain gauges / load cells / geodetic monitoring instruments | **Planned** |

**DIN (Deutsches Institut für Normung)** — vibration standards cited for §25.19:

- **DIN 45669-1:1995** — Mechanical vibration and shock measurement
- **DIN 4150-1:2001** — Structural vibration, Part 1: prediction of vibration parameters
- **DIN 4150-2:1999** — Human exposure to vibration in buildings *(under revision)*
- **DIN 4150-3:2016** — Vibrations in buildings, Part 3: effects on structures

**Other agency standards and guidelines:**

- **Transportation Research Board (TRB), 2008** — *Use of Inclinometers for
  Geotechnical Instrumentation on Transportation Projects* (Machan & Bennett) — a
  comprehensive technical note on inclinometer practice.
- **USGS, 2008** — *Instrumentation Guidelines for the Advanced National Seismic
  System (ANSS)*, Open-File Report 2008–1262, 48 pp. — the source of the **Class
  A–D strong-motion system classification** used in §25.18.
- **COSMOS, 2016** — *Guidelines and General Considerations for Strong-Motion
  Instrumentation of Tall Buildings* — strong-motion guidance for tall structures.
- **US Bureau of Mines RI 8507, 1980** (Siskind et al.) — *Structure Response and
  Damage by Ground Vibration from Mine Blasting* — the classic blasting-vibration
  reference underlying §25.19.

### 25.2.4 — Regulation and manual references (dam safety)

The chapter's list of **downloadable dam-safety instrumentation guidelines** — the
regulatory manuals that a monitoring programme is ultimately accountable to:

| Manual | Publisher / year | Size |
|---|---|---|
| **EM 1110-2-1908** — *Instrumentation of Embankment Dams and Levees* | U.S. Army Corps of Engineers, 2020 | 290 pp. |
| **EM 1110-2-4300** — *Instrumentation for Concrete Structures* | U.S. Army Corps of Engineers, 1987 *(under revision)* | 306 pp. |
| *Embankment Dam Instrumentation Manual* (Bartholomew, Murray & Goins) | U.S. Bureau of Reclamation, 1987 *(under revision)* | 269 pp. |
| *Concrete Dam Instrumentation Manual* (Bartholomew & Haverland) | U.S. Bureau of Reclamation, 1987 | 153 pp. |
| *Engineering Guidelines for the Evaluation of Hydropower Projects*, Ch. 9 *Instrumentation and Monitoring* (2005); Ch. 14 *Dam Safety Performance Monitoring Program* (2017) | FERC | 86 / 188 pp. |
| **ICOLD Bulletin 158** — *Dam Surveillance Guide* (2018) | ICOLD | 109 pp. |
| **7 White Papers** on Development and Implementation of Dam Safety Monitoring Programs (2008–2020) | U.S. Society on Dams (USSD) | series |
| *Manual de Mecánica de Suelos: Instrumentación y Monitoreo del Comportamiento de Obras Hidráulicas* (2012) | Comisión Nacional del Agua, Mexico | 322 pp. |

> **Cross-reference.** The site digests several of these directly — see
> [Monitoring Dam Performance](../monitoring-dam-performance/index.md) (ASCE MOP-135)
> and [Tailings Dam Safety](../tailings-dam-safety/index.md) (ICOLD Bulletin 194).

### 25.2.5 — Symposia series

Comprehensive instrumentation research has been published through the **"Field
Measurements in Geomechanics" (FMGM)** symposia: Zurich 1983, Kobe 1987, Oslo 1991,
Bergamo 1995, Singapore 1999, Oslo 2003, Boston 2007, Berlin 2011, Sydney 2015 and
Rio de Janeiro 2018 — organised by volunteers (mostly academics) and published
commercially. The next symposium was scheduled for London 2022 under ISSMGE
sponsorship. These proceedings are where instrumentation **case histories** are
reported in detail.

---

## 25.3 — Human factors

Chapter 25 devotes early attention to **human factors**, drawing on three Dunnicliff
chapters: systematic planning, specifications for procurement, and contractual
arrangements. Its argument is enduring: simple mechanical/hydraulic instruments once
worked in the hands of diligent engineers with a clear sense of purpose; as
technology advanced, "an increasing number of instrumentation programmes have been
in the hands of people with incomplete motivation and sense of purpose," and many
failures became **failures of the instrument–person marriage** rather than of the
instruments. Written decades ago, the chapter notes the point is *"if not even more
so"* today, given the faster pace of construction.

---

## 25.4 — Measuring principles

Geotechnical instruments rest on **electrical, mechanical, hydraulic and pneumatic**
principles. The two dominant *electrical* principles:

- **Vibrating wire (VW)** — by far the most prevalent. A pre-tensioned steel wire
  (typically **0.25 mm** diameter, 5–15 cm long) is excited by two electromagnetic
  coils; the wire resonates at a frequency (**1,000–2,000 Hz**) that varies with
  tension. Proven in European concrete dams after WWII for robustness and long-term
  stability; now spans pore pressure, settlement, extension/compression, strain,
  load, stress and earth pressure. Temperature is often built in via a sealed
  thermistor.
- **MEMS accelerometers** — superseded servo-accelerometers and electrolytic tilt
  sensors around 2010 for **tilt and inclination**, with equal or better metrology
  plus better robustness and temperature-offset behaviour. Circuits can include a
  microcontroller and ADC, giving **digital output** on an RS-485 bus.
- **Digital-output instruments** (a related family) — piezoresistive water-level
  sensors with 4–20 mA output, multi-parameter water-quality probes, and digital
  thermistor strings, using **RS-485** or the USGS-developed **SDI-12** protocol.
- **Fibre-optic sensing** — immune to lightning and electrical transients; available
  as point sensors, **semi-distributed** (Bragg-grating) and **fully distributed**
  (Brillouin scattering, strain/temperature every metre over cables up to **30 km**).

---

## 25.5 — Metrological properties

Because instruments are often **irreplaceable** once installed, excellent metrology
is expected. The properties (after De Rubertis, 2018), with typical VW values:

| Property | Meaning | Typical VW value |
|---|---|---|
| **Resolution** | Smallest distinguishable change | Many times finer than accuracy |
| **Accuracy** | Match to an acceptable standard | **±0.1 % F.S.** (NIST-traceable) |
| **Precision** (random error) | Closeness to the mean of repeated readings | **±0.025 % F.S.** |
| **Repeatability** | Agreement of consecutive measurements | Same as precision (VW) |
| **Linearity** (non-linearity) | Departure from a straight line | **0.1–0.5 % F.S.** |
| **Bias** | Average indicated vs actual value | Same as accuracy (in practice) |
| **Long-term stability** | Output drift over years at constant input | Established by decades of case histories |

The chapter's key insight for monitoring: **change, not absolute value, is usually
what matters** — which makes *precision* more important than accuracy.

---

## 25.6–25.7 — Static vs dynamic; the instrument chain

**Static monitoring** dominates geotechnics (slow ground response), while
**dynamic** monitoring covers earthquakes, blasting and machine vibration.
Terminology is clarified along the chain: **sensor → transducer → transmitter →
instrument**, a distinction the chapter uses consistently in later sections.

---

## 25.8 — Groundwater pressure (piezometers)

The chapter's longest instrument section, covering:

- **Casagrande standpipe piezometers** — the simple, robust baseline.
- **Electric pressure transducers** — VW and other types.
- **VW piezometer in a Casagrande standpipe** — hybrid installation.
- **Zoned installation** in a borehole — isolating a measurement zone with grout
  seals.
- **Push-in piezometers** — rapid deployment where the ground permits.
- **Fully-grouted piezometers** — the method (Contreras, Mikkelsen, McKenna,
  Vaughan, Penman references in the list) that has become standard for many
  embankment-dam installations.
- **Negative pore pressure / suction** — the hardest measurement, with its own
  technique.

---

## 25.9 — Tilt and inclination

- **Tiltmeters** — for structures and local tilt.
- **Inclinometers** — the workhorse for lateral ground movement, read at fixed
  increments (e.g. 0.5 m / 2 ft) with probe-type systems.
- **In-place inclinometers and ShapeArrays** — permanently installed profiles, with
  the chapter giving **selection considerations** for each (§25.9.3.1–25.9.3.2).

---

## 25.10 — Settlement, heave and differential settlement

Covered instruments: **probe extensometers**, **borehole extensometers**, **liquid
settlement cells**, **differential liquid settlement cells**, and **horizontal
inclinometers** — together spanning the range from surface settlement to deep
heave.

---

## 25.11–25.14 — Cracks, strain/load, earth pressure, temperature

- **Crack and joint opening** — crackmeters, jointmeters, soil extensometers.
- **Strain and load** — strain gauges, load cells (concrete, steel, anchors).
- **Earth pressure** — total pressure cells, push-in pressure cells.
- **Temperature** — thermistors and thermistor strings (also the reference
  parameter for many other instruments' compensation).

---

## 25.15 — Automated data acquisition and telemetry

**ADAS (Automated Data Acquisition Systems)** are field-deployable devices that
collect and store measurements from many sensors via cable or radio, and optionally
transmit them to a remote computer without human intervention. Required features:

- **Signal management** for mixed sensor types (VW, MEMS digital, 4–20 mA, 0–5/0–10 V analog, RS-485/SDI-12 digital).
- **Battery power** (alkaline, lithium, or lead-acid + solar).
- **On-board data storage**.
- **Low-throughput communications** — radio, cell modem or satellite, on a schedule.
- **Optional local alarm/control**.
- A continuum from **1-channel standalone loggers to 1,000+ channel networks**.

The chapter distinguishes a **datalogger** (one device carrying all/most features)
from an **ADAS** (an elaborate logger that can also form a **network**, manage alarm
conditions, and **control external devices** — SMS, valve actuation, siren/flashing
light). *Note the market trend:* small loggers now carry features once found only in
ADAS networks.

**Small dataloggers** (§25.15.1) — 1–10 channels, low power, "D"-cell 3.6 V
batteries giving **≥1 year autonomy**, operating range **−40 °C to +80 °C**, and
increasingly a low-power licence-free radio (a few km in open terrain, ~1 km urban).

**Integrated ADAS networks** (§25.15.2) — two architectures:

1. **Few central acquisition systems + long cable runs** — drawbacks: cable cost,
   trenching/conduit, **lightning-transient risk near the surface**, added
   resistance, and splice-error risk. The chapter's recommendation is explicit:
   **keep sensor cables short** and add more acquisition points.
2. **Hub-to-node radio networks** using small radio-enabled loggers near the
   instruments — either a **star** configuration or a **mesh** network where loggers
   relay for each other to a **gateway**, then to the office by cellular, satellite,
   Wi-Fi or LAN.

---

## 25.16 — Software for data management, visualisation, alarming and reporting

Most loggers/ADAS emit **delimited value files** (`*.csv`, `*.dat`) with a timestamp
column and one column per channel — often **raw** readings, which most users prefer
to keep. Spreadsheets suffice for small jobs; larger or longer projects need
dedicated software, which typically offers:

- **Dashboard** (project overview, real-time values, sensors on alarm)
- **Real-time display** with a colour code (**Green: OK / Yellow: threshold / Red: alarm**)
- **Trend lines** (reading vs time, with scroll and zoom)
- **Alarm** checking with automatic **SMS/email**
- **Virtual variables** (calculated from one or more sensors)
- **Access controls** (user profiles)
- **File converter** (import from most logging systems, spreadsheets, manual records)
- **Correlation (XY) graphs** (e.g. piezometric level vs rain; strain vs temperature)
- **Profile views** (in-place inclinometers, ShapeArrays)
- **Automated reports** on schedules
- **Smartphone/tablet** visualisation and **cloud hosting**
- **Multi-language** support
- **Import of geodetic (total station) and InSAR data**
- **GIS / Google Earth** geo-localisation

---

## 25.17 — Geodetic measurements

Ground-surveying methods detecting horizontal and vertical movement across a
**survey control network** of monuments or on-structure points:

- **Total stations and levels** — the core survey instruments; robotics, reflectorless
  and automatic target recognition enable **automated** operation. Typical accuracy:
  **1–5 arc-seconds** in angle; **1–1.5 mm + 1–2 ppm** in distance.
- **Rotating lasers** — for alignment and grade.
- **Laser scanners** — dense 3D capture (see Adamson et al., 2019, in the reference list).
- **GNSS** — absolute positioning.
- **Satellite InSAR** — comparison of repeat SAR images; X-, C- and L-band;
  **pixel size 0.25–20 m** (commonly 1–3 m), **precision 1–20 mm**; **>50,000 points
  per km²** over areas exceeding hundreds of km²; measurement along the radar beam
  (≈50–70° from horizontal), so true vertical displacement needs trigonometry;
  revisit **a few days to 14+ days**. Ascending+descending constellations add
  horizontal information.
- **Ground-based InSAR** — terrestrial radar interferometry for local coverage.
- **UAV photogrammetry** — aerial survey for deformation (see Stafford et al., 2019).

---

## 25.18–25.19 — Strong motion and vibration

- **Strong-motion accelerographs** — 3D accelerometer + recorder, capturing **peak
  particle acceleration** (in *g*) and the time history. Best practice: one unit in
  the **free field**, plus one at the structure's **highest point** and intermediate
  positions, **GPS-synchronised** when multiple units are used. Classified **A–D**
  per **USGS (2008)** for the ANSS network; Canada operates the **CNSN** (100+
  high-gain seismographs, 60+ accelerographs).
- **Vibration monitors** — triaxial velocity sensor (**geophone**) + datalogger,
  measuring **particle velocity in cm/s** (blasting, traffic, ambient vibration —
  governed by the DIN 4150 series).

---

## 25.20 — Presentation of instrumentation data

The chapter's closing argument: **all data must share a common timestamp**, and that
timestamp is the **only link** between monitoring data and construction activities
(which unload and then reload the ground). Environmental factors — **temperature and
rainfall** — must also be recorded, because unloading can open cracks that rainwater
then exploits (Figure 25-23). Integrating monitoring data with construction activities
and environmental factors **remains a challenge for most commercial plotting
programs** — and any programme must **allocate adequate resources** so that data is
presented and interpreted without ambiguity.

---

## Key takeaways

- **Six parameters, one discipline.** Groundwater pressure, displacement, strain,
  load, total pressure and temperature — each with its own instrument families.
- **§25.2 is the chapter's most reusable asset** — a guided map of the standards
  (ASTM D18.23, ISO 18674, DIN 4150), textbooks (Dunnicliff, De Rubertis, Sharon &
  Eberhardt, Hoek), regulation manuals (USACE, Reclamation, FERC, ICOLD) and
  symposia behind monitoring practice.
- **Vibrating wire and MEMS dominate** electrical measurement; fibre-optic sensing
  is the emerging third family.
- **Precision beats accuracy** for monitoring, because *change* is what matters.
- **Keep sensor cables short and distribute acquisition** — long surface runs invite
  lightning damage and splice errors.
- **Automation is a spectrum**, from a 1-channel logger to a 1,000+ channel ADAS
  network with alarms and control.
- **Timestamp everything, and record temperature and rainfall** — otherwise the
  data cannot be interpreted against construction activity.
- **Human factors decide success.** The instrument–person marriage matters as much
  as the instrument.

---

## Full reference list

*Reproduced as the chapter's bibliography, for lookup. Standards are revised on their
own cycles — verify the current edition.*

**Adamson, D., Alfaro, M., Blatz, J., Bannister, K.** — Construction and Post-Construction Deformations of an MSE Wall using Terrestrial Laser Scanning. *Geo St John's 2019*, Canadian Geotechnical Society.

**Anderson, C., Vessely, M., Christiansen, C., 2020** — Advances in Unstable Slope Instrumentation and Monitoring. TRB / NCHRP, National Academies, Washington DC.

**Burland, J., Chapman, T., Skinner, H., Brown, M. (Eds), 2012** — *ICE Manual of Geotechnical Engineering*, Ch. 94 (Dunnicliff, Marr & Standing) and Ch. 95 (Dunnicliff). ICE Publishing, London.

**Choquet, P., Juneau, F., Debreuille, P.J., Bessette, J., 1999** — Reliability, Long-term Stability and Gage Performance of Vibrating Wire Sensors with Reference to Case Histories. *Proc. 5th Int. Symp. on Field Measurements in Geomechanics*, Singapore.

**Choquet, P., Taylor, R.M., 2014** — Automatic Data Acquisition Systems (ADAS) for Dam and Levee Monitoring. *Geo-Congress 2014*, ASCE, 180–191.

**Client guide to instrumentation and monitoring**, 2017 — Chartered Institution of Civil Engineering Surveyors for the Survey Liaison Group, London.

**Contreras, I.A., Grosser, A.T., VerStrate, R.H., 2007** — The use of the fully-grouted method for piezometer installation. *Proc. 7th Int. Symp. on Field Measurements in Geomechanics*, Boston. *(See also the 2008, 2011, 2012 and 2020 updates by the same authors.)*

**COSMOS, 2016** — *Guidelines and General Considerations for Strong-Motion Instrumentation of Tall Buildings*.

**De Rubertis, K. (Ed.), 2018** — *Monitoring Dam Performance — Instrumentation and Measurements*, ASCE, 442 pp.

**DIN** — DIN 45669-1:1995; DIN 4150-1:2001; DIN 4150-2:1999 (under revision); DIN 4150-3:2016.

**Dunnicliff, J., 1993** — *Geotechnical Instrumentation for Monitoring Field Performance*, Wiley, 577 pp.

**Dunnicliff, J., 1994** — Contract Practices for Geotechnical Instrumentation. *Geotechnical News*, Vol. 12, No. 3.

**Elwood, D.E.Y. & Martin, C.D., 2016** — Ground response of closely spaced twin tunnels constructed in heavily overconsolidated soils. *Tunnelling and Underground Space Technology*, 51, 226–237.

**Ferretti, A., Monti-Guarnieri, A., Prati, C., Rocca, F., 2007** — *InSAR Principles: Guidelines for SAR Interferometry Processing and Interpretation*. ESA TM-19.

**Glisic, B., Inaudi, D., 2007** — *Fibre Optic Methods for Structural Health Monitoring*, Wiley, 281 pp.

**McKenna, G.T., 1995** — Grouted-in Installation of Piezometers in Boreholes. *Canadian Geotechnical Journal* 32, 355–363.

**McRae, J.B., Simmonds, T., 1991** — Long-term Stability of Vibrating-wire Instruments: One Manufacturer's Perspective. *Proc. 3rd Int. Symp. on Field Measurements in Geomechanics*, Vol. 1:283–293, Balkema.

**Mikkelsen, P.E., 2002** — Cement-Bentonite Grout Backfill for Borehole Instruments. *Geotechnical News*, Vol. 20, No. 4, 38–42.

**Mikkelsen, P.E. & Green, E.G., 2003** — Piezometers in Fully Grouted Boreholes. *6th Int. Symp. on Field Measurements in Geomechanics*, Oslo.

**Pantony, B., Fraser, S., Sinacori, J., 2021** — Satellite InSAR for Geotechnical and Structural Monitoring. *Canadian Geotechnique*, Vol. 2, No. 1.

**Penman, A.D.M., 2002** — Measurement of Pore Water Pressures in Embankment Dams. *Geotechnical News*, Vol. 20, No. 4, 43–49.

**Pieraccini, M., Miccinesi, L., 2019** — Ground-Based Radar Interferometry: A Bibliographic Review. *Remote Sensing* 11(9).

**Richards, D.J., Clark, J., Powrie, W., Heymann, G., 2007** — Performance of push-in pressure cells in overconsolidated clay. *Geotechnical Engineering* 160, GE1, 31–41.

**Richards, D.J., Powrie, W., Roscoe, H., Clark, J., 2007** — Pore water pressure and horizontal stress changes during construction of a contiguous bored pile multi-propped retaining wall in Lower Cretaceous clays. *Géotechnique* 57(2), 197–205.

**Ridley, A.M., 2015** — Soil suction — what it is and how to successfully measure it. *9th Symp. on Field Measurements in Geomechanics*, Australian Centre for Geomechanics, Perth, 27–46.

**Schuyler, J.N. & Gularte, F., 2000** — Automated Tiltmeter Monitoring of Bridge Response to Compaction Grouting. *SPIE 7th Annual Int. Symp. on Smart Structures and Materials*, Newport Beach, CA.

**Sellers, J.B., 1994** — Load Cell Calibrations. *Geotechnical News*, Vol. 12, No. 3.

**Sellers, J.B., Taylor, R., 2008** — MEMS Basics. *Geotechnical News*, Vol. 26, No. 1.

**Sharon, R., Eberhardt, E. (Eds), 2020** — *Guidelines for Slope Performance Monitoring*, CSIRO Publishing / CRC Press, 331 pp.

**Siskind, D.E., Stagg, M.S., Kopp, J.W., Dowding, C.H., 1980** — *Structure Response and Damage by Ground Vibration from Mine Blasting*. US Bureau of Mines RI 8507.

**Soe Moe, K.W., Cruden, D.M., Martin, C.D., Lewycky, D., Lach, P.R., 2009** — Mechanisms and kinematics of river valley landslides in Edmonton. *Annual Canadian Geotechnical Conference, GeoHalifax*.

**Stafford, D.M.J. et al., 2019** — Preliminary deformation detection of high-fill sections along the Inuvik-Tuktoyaktuk Highway using UAV photogrammetry. *Geo St. John's 2019*, CGS.

**Stark, T.D., Oommen, T., Ning, Z., 2021** — *Remote Sensing for Monitoring Embankments, Dams, and Slopes: Recent Advances*, ASCE GSP 322, 114 pp.

**Tedd, P., Powell, J.J., Charles, J.A., Uglow, I.M., 1990** — In situ measurement of earth pressures using push-in spade-shaped pressure cells — 10 years' experience. *Geotechnical Instrumentation in Practice*, Thomas Telford, London, 701–715.

**U.S. Geological Survey, 2008** — *Instrumentation Guidelines for the Advanced National Seismic System*. Open-File Report 2008–1262, 48 pp.

**Vaughan, P.R., 1969** — A Note on Sealing Piezometers in Boreholes. *Géotechnique* 19(3), 405–413.

**Walker, J. & Awange, J.L., 2020** — *Surveying for Civil and Mine Engineers*, Springer, 411 pp.

> **Acknowledgement (original chapter).** The chapter's author thanks the
> instrumentation suppliers who provided the figures and photographs for the
> original publication. Those figures are **not** reproduced here.
