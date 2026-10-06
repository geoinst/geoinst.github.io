---
lang: en
lang_alt: vi/reference-manuals/monitoring-dam-performance/chapter-11-data-management.md/
---
# Chapter 11 — Data Acquisition, Management, and Databases

## 11.1 Data only matters if you can find it later

The goal of data management is simple: every reading is captured, validated,
stored, and retrievable for decades, with enough context to be interpreted by
someone who was not there. Data loss is permanent; a reading not saved might as
well not have been taken.

## 11.2 Acquisition frequency

Frequency follows the rate of change and the program plan
([Chapter 4](chapter-04-planning.md)):

- **Steady state** — monthly to quarterly for slow variables.
- **Construction / first filling** — daily to weekly.
- **After events** — intensively, or continuously via automation
  ([Chapter 9](chapter-09-automated.md)).

## 11.3 Validation

Raw readings are not data until checked. Validation includes:

- **Range checks** — is the value physically possible?
- **Reasonableness** — does it match the trend and season?
- **Cross-checks** — do correlated instruments agree?
- **Manual vs. automated** agreement for spot readings.

Bad data must be flagged, not silently dropped.

## 11.4 Storage and databases

A monitoring database should record, for every reading:

- Instrument identity and location.
- Timestamp and reader.
- Value, units, and uncertainty.
- Environmental context (reservoir level, temperature, rainfall).

Prefer open, portable formats and a system with a clear migration path. Proprietary
"black boxes" that cannot export are a long-term risk.

## 11.5 The baseline as a managed asset

The early-operation baseline ([Chapter 2](chapter-02-failure-modes.md)) is a
managed asset. Store it explicitly so that future "normal" can be compared with
today's "normal" as the dam ages.

## 11.6 Integration with the wider program

Good data management links readings to the monitoring plan (why each instrument
exists) and to inspection findings (so an instrument anomaly and a field
observation can be viewed together).

## 11.7 Key takeaways

- Capture, validate, and store every reading with full context.
- Set frequency by rate of change, not convenience.
- Flag bad data; never silently delete it.
- Use portable, exportable systems; treat the baseline as a long-term asset.
