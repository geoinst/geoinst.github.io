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

*See also: [Thuật ngữ Anh – Việt (Vietnamese Glossary)](../vi/thuat-ngu/index.md) · [Compliance Matrix (Decree 114 / TCVN 9398)](../compliance/decree-114-tcvn-9398.md) · [Interactive Sandbox](../visualizer.md)*
