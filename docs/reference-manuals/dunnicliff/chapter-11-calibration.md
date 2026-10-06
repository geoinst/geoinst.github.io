---
lang: en
lang_alt: vi/reference-manuals/dunnicliff/chapter-11-calibration/
---
# Chapter 11 — Calibration & Maintenance

## 11.1 Calibration: the reference point

A sensor's reading is meaningless without a known relationship between its output
and the physical quantity. **Calibration** establishes and maintains that
relationship.

## 11.2 Factory and field calibration

- **Factory calibration** provides the as-delivered conversion and a certificate
  of traceability.
- **Field calibration / verification** confirms the instrument still performs
  after transport, installation, and exposure — because field conditions shift
  the relationship.

Periodic re-calibration (or at least verification against a reference) catches
drift before it corrupts the record.

## 11.3 Maintenance schedules

A maintenance plan addresses:

- **Readout units and dataloggers** — function, clock, power.
- **Cables and connectors** — continuity, water ingress, rodent damage.
- **Sensor zero and span** — checked against manual or reference readings.
- **Environmental protection** — UV, corrosion, freezing.

## 11.4 Cold-weather guidelines

Freezing is a major cause of data loss:

- Bury or heat cables and sensors where needed.
- Use antifreeze or heated enclosures for standpipes and readouts.
- Document a seasonal plan, including safe shutdown and fallback to manual reads.

## 11.5 Documentation

Every calibration and maintenance action is recorded: date, method, result,
person, and any change to conversion factors. This preserves the data's
defensibility over the instrument's life.

!!! warning "Drift is silent"
    An uncalibrated sensor rarely fails loudly; it drifts quietly, corrupting
    trends until someone notices a physically impossible reading. Schedule
    verification; don't wait for the impossible number.

![Figure: dunnicliff-calibration](../../assets/figures/dunnicliff-calibration.svg)

**Figure.** Calibration. The input-output relationship (slope = calibration factor), with zero, span, and hysteresis (Dunnicliff, Ch. 7 and 16).

## 11.6 Key takeaways

- Calibration ties output to physical quantity; verify it in the field.
- Maintain on a schedule: readouts, cables, zero, environment.
- Plan explicitly for freezing and seasonal effects.
- Record every calibration and maintenance action.
