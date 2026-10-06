---
lang: en
lang_alt: vi/reference-manuals/tailings-dam-safety/chapter-11-data-management/
---
# Chapter 11 — Data Acquisition, Management, and Databases

## 11.1 From reading to record

Raw sensor output is not information. The data chain — acquisition, validation,
storage, and retrieval — determines whether measurements become defensible
evidence of performance.

## 11.2 Reading frequency

Frequency is set by:

- **Parameter dynamics** (pore pressure and movement during a storm change fast;
  settlement slowly).
- **Life stage** (commissioning and peak filling need more; steady operation less).
- **Risk category** (higher consequence → more frequent, often automated).

A minimum frequency is documented in the plan; event-driven increases follow
storms, earthquakes, or anomalies.

## 11.3 Validation and quality control

Before data enters the record it should be checked for:

- **Plausibility** (within range, no wild jumps).
- **Continuity** (gaps explained, not hidden).
- **Calibration drift** (compared to manual checks and factory cal).
- **Environmental correlation** (e.g., temperature effects removed).

!!! warning "Gaps are data too"
    A missing reading is a finding. Investigate and document gaps rather than
    silently interpolating. A pattern of gaps in a critical instrument is itself
    an alarm.

## 11.4 Databases and retrieval

A structured database (not scattered spreadsheets) supports:

- Time-series plots per instrument and parameter.
- Cross-plots (e.g., movement vs. pore pressure).
- Audit trail and access control.
- Long-term continuity as staff and instruments turn over.

## 11.5 Preservation and handover

Monitoring records must outlast any individual or contract. Archive raw and
processed data, installation records, and review notes in a form that survives
**closure and ownership transfer**. The record is the facility's memory.

## 11.6 Key takeaways

- Data chain quality determines whether readings become evidence.
- Set frequency by parameter, life stage, and risk.
- Validate plausibility, continuity, and calibration; document gaps.
- Archive for the long term, through closure and ownership change.
