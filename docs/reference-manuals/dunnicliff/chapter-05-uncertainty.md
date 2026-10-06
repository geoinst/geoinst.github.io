---
lang: en
lang_alt: vi/reference-manuals/dunnicliff/chapter-05-uncertainty/
---
# Chapter 5 — Measurement Uncertainty & Data Acquisition Systems

## 5.1 All measurements are uncertain

No reading is exact. Understanding and managing **measurement uncertainty** is
what separates trustworthy monitoring from deceptive precision.

## 5.2 Key concepts

- **Accuracy** — closeness to the true value.
- **Precision / repeatability** — closeness of repeated readings to each other.
- **Hysteresis** — output depends on the direction of change (loading vs.
  unloading).
- **Noise** — random fluctuation masking the signal.
- **Error budget** — the sum of individual uncertainties (sensor, cable, readout,
  environment) that bounds the total uncertainty.

A small, precise but inaccurate instrument can be more misleading than a larger,
honest one.

## 5.3 Transducers: how instruments "speak"

Most modern instruments are **transducers** converting a physical quantity into
an electrical or pneumatic signal. Common types:

- **Vibrating-wire** — frequency output, robust, widely used.
- **Electrical (strain-gage, resistance, capacitance)** — versatile, sensitive to
  lead effects.
- **Pneumatic** — gas-pressure balance, no power needed.
- **Hydraulic** — liquid-column balance, long-established.

## 5.4 Data acquisition systems (ADAS)

A data acquisition system scans sensors, applies conversion, time-stamps, and
stores readings. For automated monitoring it includes telemetry and a database.
Selection considers channel count, scan rate, power, environmental hardening,
and data formats.

## 5.5 Managing uncertainty in practice

- Choose instruments whose accuracy matches the decision, not maximal spec.
- Establish and document the error budget.
- Calibrate and verify (Chapter 11).
- Report readings with their uncertainty, not as false-precision decimals.

!!! warning "Precision is not accuracy"
    A readout showing `12.3456 kPa` is not more true than `12.3 kPa`. Report to
    the resolution the instrument and installation actually support.

## 5.6 Key takeaways

- Every reading carries uncertainty; manage the error budget.
- Accuracy ≠ precision; both matter, neither alone suffices.
- Match instrument accuracy to the decision, not to the brochure.
- Automated systems need robust ADAS, telemetry, and data handling.
