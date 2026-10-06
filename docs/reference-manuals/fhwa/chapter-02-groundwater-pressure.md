---
lang: en
lang_alt: vi/reference-manuals/fhwa/chapter-02-groundwater-pressure/
---
# Chapter 2 — Overview of Hardware for Groundwater Pressure

## 2.1 What a piezometer is

In this reference, a **piezometer** is a device sealed within the ground so that
it responds **only** to groundwater pressure around itself and not to pressures at
other elevations. Piezometers monitor **pore-water pressure in soil** and **joint
water pressure in rock**. (The term *pore-pressure cell* is sometimes used as a
synonym.) An **observation well** is a different instrument: it has no subsurface
seals and therefore creates a vertical connection between strata.

Piezometer applications fall into two broad categories:

1. **Mapping the pattern of water flow** — for example, monitoring subsurface flow
   during large-scale pumping tests to determine permeability in situ, or tracking
   long-term seepage in slopes.
2. **Providing an index of strength** — pore pressure allows effective stress to be
   estimated ($\sigma' = \sigma - u$), and thus strength to be assessed. Examples
   include the strength along a potential failure plane behind a cut slope, and
   pore-pressure control during staged construction over soft clay foundations.

The difference between soil and rock piezometers is not the instrument but the
**installation**: in soil, a short sand column (typically ~750 mm) is placed around
the piezometer; in rock, the sand column is much longer to ensure it intersects a
discontinuity.

## 2.2 Observation wells

An observation well is a perforated section of pipe attached to a riser, installed
in a sand- or gravel-filled borehole. A surface seal prevents runoff from entering,
and a vent in the cap lets water flow freely. The water level is found by sounding.

**Appropriate applications are very limited.** Because an observation well creates
a **vertical connection between strata**, it is valid only in continuously
permeable ground where groundwater pressure increases uniformly with depth — a
condition that can rarely be assumed. In current practice they are frequently
installed during site investigation "to define initial groundwater pressures," but
the readings are often misleading. **Observation wells should rarely be used** for
performance monitoring.

## 2.3 Open standpipe piezometers

The **open standpipe (Casagrande) piezometer** is a filter tip connected to a riser
pipe, with the annular space sealed above the filter so that only the target zone
is connected. It is reliable, has a long record of successful performance, and its
seal integrity can be checked after installation with a falling-head test. It can
be converted to a remote-reading instrument by inserting a pressure transducer.

Its great limitation is the **long hydrodynamic time lag** (Section 2.7). Other
limitations: it can be damaged by construction equipment or by vertical compression
of the surrounding soil; it can freeze if the piezometric level rises above the
frost line; extending the standpipe through an embankment interrupts fill
placement and causes inferior compaction; and the porous filter can plug with
repeated inflow and outflow.

## 2.4 Pneumatic piezometers

A **pneumatic piezometer** uses a flexible diaphragm balanced by gas pressure
supplied and returned through twin tubes. Advantages: short time lag, the
calibrated part of the system stays accessible at the readout, minimum interference
with construction, and no freezing problems. Limitations: readings are somewhat
operator-dependent, and accuracy is reduced when read under a flowing-gas
condition.

## 2.5 Vibrating-wire piezometers

A **vibrating-wire (VW) piezometer** measures the change in resonant frequency of a
tensioned wire as a diaphragm deflects under water pressure. Advantages: easy to
read, short time lag, minimum interference with construction, minimal lead-wire
effects, no freezing problems, and ready connection to a **datalogger** for
automated monitoring. Its principal limitation is that the **need for lightning
protection should be evaluated**.

## 2.6 Multipoint piezometers

A **multipoint piezometer** places several sensors in one borehole to give detailed
pressure-versus-depth measurements, with an unlimited number of measurement points
and a calibrated part of the system accessible at the surface. The trade-off is a
**complex installation procedure**, and typically only periodic manual readings.

![Figure: dunnicliff-piezometer-types](../../assets/figures/dunnicliff-piezometer-types.svg)

**Figure.** Common piezometer types compared: vibrating-wire, pneumatic, open standpipe, and twin-tube hydraulic (after FHWA-HI-98-034, Ch. 2).

## 2.7 Hydrodynamic time lag

The **hydrodynamic time lag** is the time for water to move through the filter and
equalize pressure with the surrounding ground. It is governed by the instrument's
**volume-change flexibility** relative to the permeability of the ground:

- A **standpipe** must admit a large volume of water to raise the column — so in
  low-permeability clay the lag can be **weeks to months**.
- A **diaphragm instrument** (pneumatic or VW) changes volume by only a tiny amount,
  so its lag is **seconds to minutes**.

This is why low-permeability ground demands a stiff-diaphragm instrument, and why a
standpipe is only appropriate in relatively permeable soil.

## 2.8 Recommended instruments and miscellaneous issues

- **Selection:** use the table of advantages and limitations to match the instrument
  to the ground and to the required response speed.
- **Filter type:** the porous filter must be chosen so it does not clog and does not
  itself add lag.
- **Granular bentonite seal above the piezometer**, then **grout above that seal**,
  to isolate the measurement zone.
- **Sounding hammer / probe:** used to locate the water level in standpipes and
  observation wells.

!!! warning "Diaphragm piezometers read head, not elevation"
    A diaphragm piezometer reading indicates the **head above the piezometer**; the
    piezometer's own elevation must be measured or estimated if a piezometric
    *elevation* is required. All diaphragm piezometers (except vented types) are
    sensitive to **barometric pressure** changes.

![Figure: dunnicliff-instrument-cross-section](../../assets/figures/dunnicliff-instrument-cross-section.svg)

**Figure.** Typical borehole installation cross-section showing the filter zone, seal, and grout backfill that isolate a piezometer (after FHWA-HI-98-034, Ch. 2).

## 2.9 Key takeaways

- A piezometer must be **sealed** to respond only to its own zone.
- **Observation wells create a vertical connection** and should rarely be used for
  monitoring.
- **Time lag** is the deciding factor: standpipes are slow, diaphragm instruments
  are fast.
- VW piezometers are the default for automated, long-term monitoring — but plan
  **lightning protection**.
- Always record the piezometer **elevation**, and watch **barometric** effects.
