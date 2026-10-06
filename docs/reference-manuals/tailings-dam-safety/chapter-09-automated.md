---
lang: en
lang_alt: vi/reference-manuals/tailings-dam-safety/chapter-09-automated/
---
# Chapter 9 — Automated, Remote, and Real-Time Systems

## 9.1 Why automate

Tailings facilities operate continuously and can fail between manual readings.
Automated systems provide **continuous, unattended** data and can raise alarms
when no one is on site — essential for higher-consequence facilities.

## 9.2 Components of an automated system

- **Sensors** — VW piezometers, in-place inclinometers, prisms, level sensors.
- **Dataloggers** — scan sensors, apply conversion, time-stamp, and buffer data.
- **Telemetry** — cellular, satellite, radio, or fiber to move data off-site.
- **Central database and dashboard** — where data is validated, plotted, and
  reviewed ([Chapter 11](chapter-11-data-management.md)).
- **Alarm engine** — compares readings to trigger/action levels and notifies
  responders ([Chapter 13](chapter-13-decisions.md)).

## 9.3 Satellite radar (InSAR)

Interferometric Synthetic Aperture Radar (InSAR / A-DInSAR) from satellites
measures ground displacement over the entire facility and surroundings at
millimeter precision, with no on-site instruments. It is ideal for:

- Detecting **regional or unexpected** movement.
- Covering remote or large facilities economically.
- Providing an independent check on point instruments.

Its limitations — revisit intervals of days, sensitivity mainly to vertical and
look-direction movement, vegetation effects — mean it **complements**, not
replaces, ground instruments.

## 9.4 Real-time alerting and thresholds

Automated systems are only useful if they **alert**. Design:

- Clear trigger and action levels per parameter.
- Redundant communication paths (a single failed cell modem is a blind spot).
- Escalation paths and on-call responsibility.
- Regular testing of the alarm path (don't discover it's broken during an event).

!!! warning "Automation needs maintenance"
    Automated systems fail silently if neglected: dead batteries, fouled sensors,
    broken cables, expired SIM cards. A maintenance plan ([Chapter 10](chapter-10-iom.md))
    and periodic end-to-end alarm tests are mandatory.

## 9.5 Independence and resilience

For high-consequence facilities, regulators increasingly expect **independent**
monitoring — systems and data paths not dependent on the operating control system
— so that a site-wide outage does not also blind surveillance.

## 9.6 Key takeaways

- Automation gives continuous, unattended coverage and alarms.
- InSAR adds whole-facility mm-precision with no on-site sensors.
- Design real trigger levels, redundant paths, and tested escalation.
- Independent, maintained systems are expected for high-consequence facilities.
