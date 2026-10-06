---
lang: en
lang_alt: vi/thuat-ngu/
---

# 📖 Geotechnical Instrumentation & ADAS Glossary

> Comprehensive technical glossary and reference dictionary covering subsurface geotechnical instrumentation, sensor physics, automated data acquisition systems (ADAS/ADAQS), wireless telemetry, and field monitoring engineering. Grounded in international standards (ISO 18674, ASTM, BS 5930) and John Dunnicliff's foundational principles.

---

## 1. Subsurface Sensors & Measurement Devices

### Piezometers & Pore Water Pressure

* **Piezometer**: An instrument installed in soil, rock, or backfill to measure pore water pressure or groundwater elevation.
* **Vibrating Wire Piezometer (VWP)**: A diaphragm-based sensor where water pressure deflects a flexible diaphragm connected to a tensioned steel wire. Changes in diaphragm deflection alter wire tension and its natural resonant frequency ($f$). Highly resistant to electrical noise and long cable runs.
* **Standpipe Piezometer (Casagrande)**: An open-tube piezometer consisting of a porous ceramic or plastic tip connected to a riser pipe. Measures hydrostatic water level directly using an electric water level indicator (dip meter). Slower hydraulic response time in low-permeability clays.
* **Pneumatic Piezometer**: A diaphragm sensor operated by gas pressure. Gas (usually nitrogen) is pumped down a supply tube until it balances pore pressure and opens a valve, venting through a return tube. Zero fluid volume change, negligible time lag.
* **Drive-In / Push-In Piezometer**: A robust, pointed-tip piezometer pressed directly into soft clay or silt formations without pre-drilling a borehole.
* **High-Air-Entry (HAE) vs Low-Air-Entry (LAE) Filter**:
    * **HAE Ceramic**: Fine pore size (typically 1–2 µm) with high bubbling pressure, preventing air entry under negative pore water pressures (suction) in unsaturated soils.
    * **LAE Carborundum/Polyethylene**: Coarse pore size (typically 50 µm), designed for rapid saturation in standard saturated groundwater measurements.
* **Multi-Level Piezometer Array**: Multiple VWP sensors positioned at discrete elevations within a single borehole to capture vertical hydraulic gradients, perched aquifers, and seepage profiles.

### Inclinometers & Lateral Displacement

* **Inclinometer Casing**: Special grooved plastic (ABS) or aluminum tubing installed in a borehole, slurry wall, or embankment, with internal orthogonal keyways that guide probe orientation.
* **Traversing Probe Inclinometer**: A wheeled torpedo containing dual orthogonal servo-accelerometers or MEMS sensors, lowered into grooved casing on a graduated control cable to record tilt profiles at regular intervals (e.g., 0.5 m).
* **In-Place Inclinometer (IPI)**: A string of articulated tilt sensor pods permanently suspended inside grooved casing at critical depths to provide continuous, automated lateral displacement logging.
* **ShapeArray (SAA / Flexible 3D Array)**: A jointed string of miniature rigid segments interconnected by flexible joints, containing triaxial MEMS accelerometers that measure continuous 3D displacement profiles in real time.
* **Horizontal Inclinometer**: An inclinometer system utilizing horizontally installed grooved casing to measure vertical settlement and heave profiles beneath embankments, tanks, or landfills.
* **Spiral Twist Survey**: An auxiliary probe run used to measure rotational twist in inclinometer casing keyways over deep boreholes, correcting azimuth errors in lateral deflection calculations.

### Extensometers & Settlement Systems

* **Multipoint Borehole Extensometer (MPBX)**: An assembly of anchors fixed at varying depths inside a borehole, linked via rigid rods or fiberglass tendons inside protective sleeves to a reference head at the surface. Measures axial ground movement and zone deformation.
* **Magnetic Settlement Gauge**: An access pipe surrounded by external spider magnets anchored to the soil. A portable reed-switch probe lowered down the pipe sounds a buzzer when passing each magnetic target, yielding point-specific vertical settlement.
* **Liquid Level Settlement Cell**: A differential pressure sensor or overflow cell linked via liquid-filled tubing to an external reservoir, measuring vertical elevation changes of subterranean structures or foundation slabs.
* **Settlement Plate**: A rigid steel or timber plate placed on original ground prior to fill placement, connected to a vertical riser pipe extended as embankment height increases.
* **Tape Extensometer**: A portable high-precision steel measuring tape with an in-line micrometer tensioning head, used to measure convergence across tunnel walls and excavation struts.

### Structural & Load Monitoring

* **Load Cell (Center-Hole / Annular)**: An instrument placed beneath anchor nuts on tiebacks, rock bolts, or foundation struts to measure axial tensile or compressive load. Most commonly utilizes multiple vibrating wire strain gauges arranged in parallel.
* **Vibrating Wire Strain Gauge (VWSG)**: A sensor welded to steel structures or embedded directly in concrete (sister bar / embedment gauge) to record micro-strain ($\mu\varepsilon$) caused by structural loading or thermal expansion.
* **Earth Pressure Cell (Total Pressure Cell)**: Two circular or rectangular steel plates welded together with an incompressible hydraulic fluid between them, connected to a pressure transducer. Installed at the soil-structure interface or within embankment fill.
* **Tiltmeter**: An instrument anchored to retaining walls, historic structures, or bridge piers to detect angular rotation. Utilizes electrolytic bubbles or high-precision MEMS sensors.
* **Crackmeter / Jointmeter**: A displacement transducer anchored across concrete joints or rock fissures to monitor relative joint opening, closing, and shear movements.

---

## 2. Automated Data Acquisition Systems (ADAS) & Telemetry

### Signal Conditioning & Protocols

* **ADAS / ADAQS**: Automated Data Acquisition System — an autonomous setup comprising sensors, data loggers, power modules, and communications infrastructure for unattended geotechnical monitoring.
* **Pluck Frequency Excitation**: The standard method for vibrating wire sensors, in which an electromagnetic coil applies a rapid swept-frequency impulse to pluck the steel wire into mechanical resonance, followed by reading the induced sinusoidal signal.
* **Spectral Analysis / VSPECT**: Advanced signal conditioning technology that performs Fast Fourier Transforms (FFT) on the raw vibrating wire return signal, isolating the true fundamental resonant frequency from external electrical noise.
* **4–20 mA Current Loop**: An analog transmission standard where sensor signals are modulated as electric current. Highly immune to cable resistance over long distances.
* **RS-485 / Modbus RTU**: A balanced differential serial bus standard capable of multidrop networking up to 32+ digital sensors over distances up to 1,200 meters.
* **SDI-12**: A low-power, serial digital interface standard widely used in environmental and geotechnical sensors operating at 1200 baud.
* **CAN Bus / CANopen**: A robust vehicle-grade digital bus protocol adopted in high-speed and underground tunneling instrumentation.

### Wireless Networks & Field Hardware

* **Data Logger**: An electronic instrument that powers attached sensors, digitizes analog signals, processes calibration polynomials, and stores timestamped records in non-volatile flash memory.
* **Relay Multiplexer**: An expansion module utilizing solid-state or sealed reed relays to sequentially switch multiple sensor channels into a single data logger measurement port.
* **LoRaWAN (Long Range Wide Area Network)**: Low-power, long-range wireless protocol operating on unlicensed sub-GHz bands (868 MHz EU, 915 MHz US/Americas, 923 MHz AS). Excellent penetration in dense urban environments and deep pits.
* **Wireless Mesh Network**: A self-forming, self-healing network topology where sensor nodes act as relays to route data packets to a central gateway, providing operational resilience against line-of-sight obstructions.
* **Cellular IoT (NB-IoT & LTE-M)**: Low-power cellular communication standards built for battery-operated IoT sensors, transmitting small data packets directly to cloud servers via commercial telecom towers.
* **Satellite Telemetry (Iridium SBD)**: Low-earth-orbit satellite data transmission used for mission-critical remote dams and mining sites where terrestrial cellular networks do not reach.
* **Solar Power Module & MPPT**: Photovoltaic solar array combined with a Maximum Power Point Tracking (MPPT) charge controller and sealed AGM or LiFePO4 battery for autonomous field operation.

---

## 3. Sensor Physics & Mathematical Reductions

### Vibrating Wire Reductions

* **Natural Frequency Equation**: The fundamental resonant frequency $f$ of a clamped wire under tension $\sigma$:

    $$
    f = \frac{1}{2L} \sqrt{\frac{\sigma}{\rho}} = \frac{1}{2L} \sqrt{\frac{E \cdot \varepsilon}{\rho}}
    $$

    Where $L$ is wire length, $\rho$ is density, $E$ is Young's modulus, and $\varepsilon$ is wire strain.

* **Digits (Linear Period Units)**: A linearizing parameter directly proportional to wire strain:

    $$
    \text{Digits} = \frac{f^2}{1000}
    $$

* **Linear Calibration Equation**:

    $$
    P = G \cdot (R_0 - R)
    $$

    Where $G$ is the gauge factor (calibrated linear coefficient), $R_0$ is baseline reading in digits, and $R$ is current reading.

* **Polynomial Calibration Equation (Second-Order)**:

    $$
    P = A \cdot R^2 + B \cdot R + C
    $$

    Provides higher measurement precision over broad pressure ranges.

* **Thermal Compensation** ($K_T$):

    $$
    P_{corr} = P_{raw} + K_T \cdot (T - T_0)
    $$

    Corrects for differential thermal expansion between the vibrating wire and the stainless steel sensor body.

* **Barometric Compensation**:

    $$
    P_{net} = P_{measured} - (B - B_0)
    $$

    Essential for sealed piezometers to isolate genuine groundwater changes from ambient atmospheric barometric swings.

### Inclinometer Data Reduction

* **Deflection Increment** ($\delta_i$):

    $$
    \delta_i = L \cdot \sin(\theta_i) = C \cdot (A_0 - A_{180})
    $$

    Where $L$ is probe wheelbase (typically 500 mm), $\theta_i$ is tilt angle, and $A_0, A_{180}$ are conjugate runs.

* **Check Sum (Zero Offset Error)**:

    $$
    \text{Check Sum} = A_0 + A_{180}
    $$

    A constant value across all depths confirming instrument stability and absence of mechanical contamination in wheels.

* **Cumulative Displacement** ($D_k$):

    $$
    D_k = \sum_{i=1}^k \delta_i
    $$

    Summation of incremental displacements calculated from the stable bottom anchor upwards to the surface collar.

---

## 4. Engineering Risk & TARP Frameworks

* **TARP (Trigger Action Response Plan)**: A systematic emergency and risk management framework that establishes defined operational actions based on observed instrumentation thresholds:
    * **Level 0 (Green / Baseline)**: Normal behavior within predicted design limits. Standard monitoring frequency.
    * **Level 1 (Amber / Alert)**: Measurement exceeds statistical baseline or initial safety margin. Monitoring frequency doubled; engineering site inspection dispatched.
    * **Level 2 (Orange / Review)**: Significant trend acceleration or structural stress approaching design tolerance. Senior engineering review, verification of backup instruments, equipment standby.
    * **Level 3 (Red / Action Required)**: Critical threshold breached; imminent structural failure or uncontrollable seepage. Immediate work stoppage, site evacuation, and execution of emergency remedial protocols.
* **Velocity of Displacement ($v = \frac{d\delta}{dt}$)**: Rate of ground movement over time. An acceleration in displacement velocity is the primary precursor to catastrophic slope and excavation failures.
* **Phreatic Line (Seepage Line)**: The upper boundary of water seepage flow through an earth dam embankment, at which pore water pressure equals atmospheric pressure.
* **Piping (Internal Erosion)**: Progressive removal of soil particles by seepage flow through embankment dams or foundations, leading to internal conduits and dam breaching.

---

## 5. Field Installation & Grouting Best Practices

* **Fully Grouted Method (Mikkelsen / Contreras)**: Installation technique where piezometers are placed directly into a borehole and encapsulated completely in a cement-bentonite grout without a traditional sand filter pack or bentonite pellets. Enabled by the extremely low volume displacement of modern diaphragm sensors.
* **Grout Mix Proportions**: Specific ratio of water to Portland cement and sodium bentonite powder designed to match the permeability and modulus of the surrounding ground formation:
    * *Soft soil*: Water:Cement:Bentonite $\approx$ 2.5 : 1.0 : 0.3 to 0.4 by weight.
    * *Medium to stiff rock*: Water:Cement:Bentonite $\approx$ 1.5 : 1.0 : 0.1 by weight.
* **Bentonite Pellet Seal**: Highly compressed sodium bentonite tablets tamped above sand packs in traditional Casagrande installations, swelling upon hydration to form an impermeable hydraulic seal.
* **Telescoping Coupling**: Slip-joints placed along inclinometer or settlement casing strings to prevent axial compression and buckling when large vertical settlements occur.

---

## 6. Tailings Storage Facilities & Tailings Dam Safety

* **Tailings**: The finely ground waste solids left after extracting metals or minerals from ore, transported and deposited as a slurry.
* **Tailings Storage Facility (TSF)**: The complete impoundment system — embankment(s), deposited tailings, supernatant pond, decant, and reclaim works — that stores mine tailings.
* **Tailings Dam**: The engineered embankment that retains the tailings deposit; often raised incrementally over the mine life and frequently built from the tailings themselves.
* **Embankment Raise (Dam Raise)**: An incremental addition to the height of a tailings embankment, placed by the upstream, centerline, or downstream method.
* **Downstream Construction Method**: Each raise is placed downstream of the previous one, so most of the structure rests on foundation — generally the most robust method.
* **Centerline Construction Method**: Raises are placed on the original centerline; intermediate in risk.
* **Upstream Construction Method**: Each raise is placed on the upstream (deposited) side, so the embankment rests on loose, saturated tailings — the highest-risk method, prone to liquefaction.
* **Beach (Tailings Beach)**: The gently sloping surface of deposited tailings between the discharge point and the supernatant pond.
* **Beach Geometry**: The slope and length of the beach, which control where the phreatic surface sits and how much freeboard is retained.
* **Supernatant Pond**: The body of clarified water above the settled tailings, from which water is recovered or decanted.
* **Decant (Decant Tower / Decant System)**: The structure and piping used to remove supernatant water and control pond level and freeboard.
* **Freeboard**: The vertical distance between the pond surface and the lowest point of the embankment crest; a primary safeguard against overtopping.
* **Spigotting / Deposition**: Discharging the tailings slurry from the embankment crest to build the beach by hydraulic deposition.
* **Thickened / Paste / Filtered Tailings**: Dewatered tailings (progressively higher solids content) that reduce free water and lower liquefaction risk.
* **In-Pit / Paddock Storage**: Storing tailings in a mined-out pit or a ring-dyke paddock instead of a valley impoundment.
* **Liquefaction**: Loss of shear strength when a saturated, loose (contractive) soil is loaded or shaken and pore pressure rises toward near-zero effective stress.
* **Static Liquefaction**: Liquefaction triggered by a static load (a raise, rapid pond rise, or foundation weakness) rather than an earthquake — the dominant catastrophic mechanism in tailings failures.
* **Seismic Liquefaction**: Liquefaction triggered by cyclic earthquake shaking.
* **Pore-Pressure Ratio ($r_u$)**: The ratio of measured pore pressure to the initial vertical effective stress ($r_u = u / \sigma'_v$); rising values signal approaching liquefaction.
* **Excess Pore Pressure**: Pore pressure above the steady-state (hydrostatic) value, generated by loading, construction, or shaking.
* **Flow Failure / Run-out**: A liquefied mass that flows rapidly and travels long distances, causing extreme downstream damage.
* **Toe Drain**: A permeable zone or drain at the downstream toe that collects and controls seepage, keeping the phreatic surface low.
* **Turbid Seepage**: Seepage carrying fine soil particles (cloudy discharge) — a warning sign of internal erosion (piping).
* **Consequence Category**: A classification of a facility by the potential downstream impact of failure (often A/B/C), which sets the intensity of monitoring and review.
* **Closure (Mine Closure)**: The post-operational phase in which the facility is decommissioned and made safe, requiring continued surveillance until the long-term steady state is demonstrated.
* **InSAR / A-DInSAR (Satellite Radar Interferometry)**: A remote-sensing technique using repeat satellite radar passes to measure millimetre-scale ground displacement over a whole facility with no on-site instruments.

---

## 7. Dam Performance Monitoring (ASCE MOP-135 scope)

* **Dam Performance**: The observed behavior of a dam, its foundation, and appurtenant structures compared with expected behavior.
* **Expected vs. Measured Behavior**: The comparison at the heart of monitoring; a large, unexplained, or trending difference is an anomaly.
* **Performance Signal**: The difference between measured and expected behavior used to judge whether the dam is performing acceptably.
* **Potential Failure Mode**: A credible way in which a dam could fail (e.g., overtopping, internal erosion, slope instability, foundation seepage); the basis for choosing instruments.
* **Uplift**: Upward water pressure acting on the base of a concrete dam or within a foundation, reducing stability.
* **Appurtenant Structures**: Auxiliary works such as spillways, outlet works, and decants that support the main dam.
* **Crest Settlement / Displacement**: Vertical or horizontal movement of the dam crest, a key deformation indicator.
* **Surveillance Plan**: The documented program stating what is monitored (visually and by instrument), how often, and the response to each anomaly.
* **Independent Review**: Periodic review of monitoring data and the program by a party independent of the operating team, to catch normalized trends.

---

## 8. Monitoring Program Planning & Reliability (Dunnicliff)

* **Geotechnical Instrumentation**: The measurement of soil, rock, foundation, and structural behavior to confirm performance and detect change.
* **Systematic Planning Approach**: Dunnicliff's structured process (the "hub") that defines the geotechnical questions first, then selects parameters, instruments, locations, and frequency.
* **Geotechnical Question**: A specific question the monitoring must answer (e.g., "will the wall exceed allowable movement?"), which dictates what is measured and the decision supported.
* **The Chain of 25 Links**: Dunnicliff's metaphor that monitoring success is a chain from defining the project need to a reading that informs a decision; break any link and the chain fails.
* **Recipe for Reliability**: The set of ingredients (selection, procurement, installation, calibration, reading, maintenance, data handling, people) that make monitoring trustworthy.
* **Observational Method**: A design approach in which the design is refined during construction based on monitored performance.
* **Transducer**: A device that converts a physical quantity (pressure, displacement, load) into an electrical or pneumatic signal.
* **Accuracy vs. Precision**: Accuracy is closeness to the true value; precision (repeatability) is closeness of repeated readings to each other. Neither alone guarantees a good measurement.
* **Hysteresis**: The dependence of an instrument's output on the direction of change (loading vs. unloading).
* **Error Budget**: The combined effect of all individual uncertainties (sensor, cable, readout, environment) that bounds the total measurement uncertainty.
* **Calibration Factor / Zero / Span**: The slope of the input–output relationship (calibration factor), the reading at zero input, and the full-scale range (span).
* **Baseline Reading**: The reference reading(s) taken after installation and settlement, against which all future change is judged.
* **Piezometric Head**: The equivalent water-surface elevation corresponding to a measured pore pressure.
* **Hydraulic Time Lag**: The delay of a piezometer's response to a change in pore pressure, governed by the permeability and geometry of the surrounding ground and filter.
* **Saturation / De-airing**: The procedure of removing air from a piezometer's filter and connecting tube so it responds correctly to pore pressure; a critical, often-neglected installation step.
* **Convergence**: The shortening (closure) of the distance between points in a tunnel or excavation, indicating ground movement.
* **Telltale**: A simple device that indicates relative movement across a joint or section.
* **Sister Bar**: A vibrating-wire strain gauge attached parallel to a rebar so that it measures the rebar's strain when embedded in concrete.
* **Overcoring**: A stress-relief technique in which a borehole instrument is isolated by overcoring to back-calculate the in-situ rock stress state.
* **Flat Jack**: A thin hydraulic jack inserted in a slot in rock to measure stress relief and estimate in-situ stress.
* **Borehole Pressure Cell (BPC)**: A device grouted into a borehole to monitor changes in rock stress around an opening.
* **Contact Stress Cell**: A pressure cell placed flush against a soil–structure interface to measure contact stress.

## 9. FHWA Highway Instrumentation (FHWA-HI-98-034 scope)

* **Golden Rule (instrumentation)**: Every instrument must be selected and placed to answer a specific geotechnical question — if there is no question, there should be no instrumentation.
* **Chain of 31 Links**: The 21 planning links plus 10 execution links that must all hold for a monitoring program to succeed; one weak link can break it.
* **Embedment Earth Pressure Cell**: A flat, fluid-filled cell embedded in soil to measure the total stress normal to its face.
* **Aspect Ratio (cell)**: The diameter-to-thickness ratio of an earth pressure cell; a high ratio reduces measurement error.
* **Soil/Cell Stiffness Ratio**: The ratio that governs how much an earth pressure cell redistributes local stress, and thus its measurement error.
* **Observation Well**: An open pipe with no subsurface seal; it creates a vertical connection between strata and is rarely suitable for performance monitoring.
* **Open Standpipe (Casagrande) Piezometer**: A filter-tipped riser pipe; reliable but with a long hydrodynamic time lag.
* **Pneumatic Piezometer**: A diaphragm balanced by gas pressure through twin tubes; short lag, no freezing, but operator-dependent.
* **Vibrating-Wire (VW) Piezometer**: A stiff-diaphragm instrument read by the change in wire frequency; short lag and datalogger-ready.
* **Multipoint Piezometer**: A single borehole containing several sensors to profile pressure with depth.
* **Settlement Platform**: A surface plate (often with a riser) recording fill settlement as an embankment is built.
* **Subsurface Settlement Point**: An anchor at depth (driven/grouted or Borros) recording settlement of a buried layer.
* **Liquid-Level Gage**: A liquid-filled tube and cell that measures settlement or heave from the change in pressure or liquid level.
* **Series Extensometer**: A stack of anchors in one borehole that resolves deformation into increments between adjacent anchors.
* **Horizontal Inclinometer**: An inclinometer traversing a horizontal casing to give a settlement profile.
* **In-Place (Fixed) Inclinometer**: A string of sensors left in casing for continuous, automated monitoring.
* **Shear-Plane Indicator**: A device that detects the depth at which inclinometer casing shears.
* **Acoustic Emission (AE) Monitoring**: Detecting the high-frequency sound from grain slip and breakage as early warning of developing instability.
* **Demec Gage**: A mechanical surface strain gage measuring the change in distance between two reference discs.
* **Calibrated Hydraulic Jack**: A center-hole jack used to apply and measure load in tensioning; it must be calibrated because fluid-pressure readings carry friction error.
* **Contact Earth Pressure Cell**: A cell measuring stress or load at a soil–structure interface, at a pile toe, or at a shaft base.
* **Load Transfer (deep foundations)**: The distribution of axial load between shaft friction and end bearing, resolved from strain gages, sister bars, and telltales.
* **Ground Improvement**: In-situ modification of ground properties — by grouting, densification, or drainage — to make it suitable for construction.
* **Acceptance Test (pre-/post-installation)**: A test confirming an instrument meets specification before installation and survived installation afterwards.
* **Installation Record Sheet**: The as-built record of position, depth, seal, and the calibration values in force — the permanent record that makes data interpretable.
* **Cause-and-Effect Plot**: A plot of measured change against an influencing factor (load, rainfall, fill height) to reveal relationships.
* **Implementation (final link)**: Acting on the interpreted data — the step that makes monitoring worthwhile.

---

*See also: [Thuật ngữ Anh – Việt (Vietnamese Glossary)](../vi/thuat-ngu/index.md) · [Compliance Matrix (Decree 114 / TCVN 9398)](../compliance/decree-114-tcvn-9398.md) · [Interactive Sandbox](../visualizer.md)*
