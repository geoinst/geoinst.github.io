---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-06-acceptable-design/
---

# Chapter 6 — When is a Rock Engineering Design Acceptable?

## 6.1 The Fallacy of a Single Factor of Safety

In classical structural steel or reinforced concrete design, a deterministic Factor of Safety ($FS$) between $1.5$ and $2.0$ guarantees safety because material properties are manufactured under strict quality standards with small coefficients of variation ($COV < 10\%$).

In geotechnical and rock engineering, however:
- Rock mass properties exhibit vast spatial scatter ($COV$ of intact strength often $20 - 40\%$; joint persistence and GSI often $15 - 35\%$).
- An engineered slope with a calculated deterministic $FS = 1.3$ based on mean parameters can have a **Probability of Failure ($P_f$) exceeding $20\%$** if the standard deviation of joint friction or pore pressure is high.
- Conversely, a slope with $FS = 1.15$ where geotechnical uncertainty is minimal may have $P_f < 1\%$.

**A single deterministic Factor of Safety is meaningless without specifying the associated uncertainty and consequences of failure.**

---

## 6.2 Deterministic Factor of Safety ($FS$) vs. Probability of Failure ($P_f$)

```
             RESISTANCE R (Capacity)
                 \       /
                  \     /
                   \   /
                    \ /
                     X  <--- OVERLAP REGION: Probability of Failure Pf
                    / \
                   /   \
                  /     \
                 /       \
             LOAD S (Demand)
```

1. **Deterministic Margin of Safety**:
   
$$FS = \frac{\text{Mean Capacity } \bar{R}}{\text{Mean Demand } \bar{S}} = \frac{\sum \text{Resisting Forces}}{\sum \text{Driving Forces}}$$

2. **Reliability Index ($\beta$)**:
   Assuming capacity $R$ and demand $S$ are normally distributed variables:
   
$$\beta = \frac{\bar{R} - \bar{S}}{\sqrt{\sigma_R^2 + \sigma_S^2}}$$

   The Probability of Failure is directly related through the standard normal cumulative distribution:
   
$$P_f = \Phi(-\beta)$$

3. **Monte Carlo Simulation**:
   Instead of calculating a single $FS$, input parameters ($c', \phi', \text{GSI}, r_u$) are sampled from statistical probability distributions (Normal, Lognormal, Beta) over $10,000$ iterations:
   
$$P_f = \frac{\text{Number of iterations with } FS < 1.0}{\text{Total number of Monte Carlo runs}}$$

---

## 6.3 Acceptable Risk Criteria Across Industries

Dr. Hoek established target criteria balancing economic investment against consequence of failure:

| Facility Type | Consequence Category | Minimum Deterministic $FS$ (Static) | Maximum Acceptable $P_f$ |
|---------------|----------------------|-------------------------------------|--------------------------|
| **Temporary Mine Open Pit Benches** | Low (localized bench spill, no personnel exposure) | $1.1 - 1.2$ | $15\% - 30\%$ |
| **Main Mine Haulage Ramps / Highwalls** | Moderate (haulage disruption, economic loss) | $1.3$ | $5\% - 10\%$ |
| **Permanent Civil Highway Slopes** | High (public traffic, disruption to commerce) | $1.5$ | $1\%$ |
| **Dam Abutments & Hydro Caverns** | Extreme (potential catastrophic dam breach or loss of life) | $1.5 - 2.0$ | $< 0.1\%$ |

---

## 6.4 The Role of Trigger Action Response Plans (TARP)

Because rock engineering accepts residual uncertainty, operations must link real-time monitoring to explicit **TARP** action matrices:

- **Level 1 (Green — Normal Operation)**: Deformation rate $< 1.0\text{ mm/day}$; pore pressure below design phreatic line. Normal mining/tunneling continues.
- **Level 2 (Amber — Advisory / Heightened Vigilance)**: Velocity increases to $2 - 5\text{ mm/day}$ or accelerating trend detected. Double sensor polling frequency; install supplementary cablebolts; inspect tension cracks.
- **Level 3 (Red — Immediate Evacuation)**: Inverse velocity analysis ($1/v \to 0$) indicates onset of tertiary creep failure. Sound alarms; extract all personnel and equipment; isolate area.

---

## 6.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Factor of Safety (FS) | Hệ số an toàn (FS) | Ratio of total resisting forces to driving forces |
| Probability of failure ($P_f$) | Xác suất phá hoại ($P_f$) | Statistical likelihood that demand exceeds capacity |
| Reliability index ($\beta$) | Chỉ số độ tin cậy ($\beta$) | Number of standard deviations separating mean margin from failure |
| Monte Carlo simulation | Mô phỏng Monte Carlo | Computational method evaluating probabilistic distributions |
| Trigger Action Response Plan (TARP) | Kế hoạch ứng phó ngưỡng kích hoạt (TARP) | Documented matrix linking sensor thresholds to operational responses |
