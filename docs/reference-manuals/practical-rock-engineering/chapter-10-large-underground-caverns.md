---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-10-large-underground-caverns/
---

# Chapter 10 — Design of Large Underground Caverns

## 10.1 Geometry & Excavation Sequence in Underground Caverns

Large underground caverns (hydroelectric powerhouses, transformer halls, underground mine crusher chambers, and defense installations) feature span dimensions exceeding $20 - 35\text{ m}$ and wall heights reaching $40 - 60\text{ m}$.

At these dimensions, single-pass excavation is impossible. Caverns must be developed through multi-stage sequential heading and benching:

```
Step 1: Top Heading Pilot Tunnel (Advance with crown rockbolts & shotcrete)
Step 2: Crown Slashings (Enlarge crown to full span width; install cablebolts)
Step 3: Bench 1 Excavation (Central bench down 3-5 m; sidewall pattern support)
Step 4: Bench 2 to N (Sequential benching downwards, maintaining sidewall support)
Step 5: Invert Excavation & Drainage Gallery Connection
```

---

## 10.2 Cavern Axis Orientation Relative to In-Situ Stresses & Joint Sets

Cavern orientation is the single most important design decision:

1. **Alignment with Major Horizontal Stress ($\sigma_H$)**:
   - The longitudinal axis of the cavern should be aligned parallel (or within $15^\circ - 20^\circ$) to the direction of the maximum horizontal principal stress ($\sigma_H$).
   - This minimizes the high compressive stresses acting across the cavern sidewalls, preventing massive sidewall buckling and deep shear zones.
2. **Alignment Relative to Dominant Joint Sets**:
   - The cavern axis must avoid striking parallel to steeply dipping persistent joint sets or faults.
   - If a fault strikes parallel to a long high sidewall, huge multi-thousand-tonne wedge blocks are formed that require uneconomically heavy cable anchor reinforcement.

---

## 10.3 Pre-Stressed Cablebolt Design for Caverns

Standard rockbolts ($3 - 5\text{ m}$ length) are insufficient to reinforce the deep plastic yield zones ($6 - 15\text{ m}$ depth) surrounding large caverns. High-capacity pre-stressed cablebolts ($15 - 25\text{ m}$ length, $500 - 1,000\text{ kN}$ capacity) are mandatory:

### Cable Anchor Components:
- **Tendon**: Multiple 7-wire high-tensile steel strands ($15.2\text{ mm}$ diameter, ultimate capacity $260\text{ kN}$ per strand).
- **Bond Length (Anchor Zone)**: Resin or cement grouted fixed length ($5 - 8\text{ m}$) anchored into virgin, elastic rock beyond the yield zone.
- **Free Length**: Sheathed or unbonded length allowing elastic elongation during tensioning.
- **Anchor Head & Bearing Plate**: Large steel bearing plate distribution stress across reinforced shotcrete pads.

$$\text{Design Working Load } T_{\text{work}} \le 0.60 - 0.70 T_{\text{ult}}$$

---

## 10.4 3D Instrumentation Arrays in Large Caverns

Monitoring during cavern benching provides the feedback loop validating numerical models (boundary element and finite element analyses):

| Instrument | Location & Array | Primary Monitoring Objective |
|------------|------------------|------------------------------|
| **Multi-Point Borehole Extensometers (MPBX)** | Radial fans from crown and high sidewalls ($10, 20, 30\text{ m}$ depth) | Measures depth of rock dilation and verifies that cable anchor bond lengths remain anchored in stationary rock |
| **Borehole Stressmeters (Vibrating Wire)** | Biaxial cells installed in sidewall rock pillars | Measures stress concentrations between adjacent powerhouse and transformer caverns |
| **Load Cells on Cablebolts** | Under bearing plate anchor heads | Continuously tracks whether rock dilation is overloading cable tendons toward tensile rupture |
| **Convergence Targets (Optical RTS)** | Grid points across cavern crown and sidewalls | Measures 3D inward closure vectors during successive lower bench blasts |

---

## 10.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Underground cavern | Buồng ngầm quy mô lớn | Large underground excavation with high span and wall height |
| Pre-stressed cablebolt | Cáp neo dự ứng lực | Long high-capacity steel strand anchor pre-tensioned against rock |
| Free length | Đoạn tự do của neo | Unbonded section of an anchor that elongates elastically |
| Bond length | Đoạn neo bầu / Chiều dài đoạn ngàm | Grout-anchored fixed section transferring load to the rock mass |
| Sequential benching | Đào hạ tầng giật cấp | Top-down excavation method removing rock in progressive horizontal benches |
