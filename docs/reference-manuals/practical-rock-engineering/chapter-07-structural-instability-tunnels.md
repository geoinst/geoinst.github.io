---
lang: en
lang_alt: vi/reference-manuals/practical-rock-engineering/chapter-07-structural-instability-tunnels/
---

# Chapter 7 — Structurally Controlled Instability in Tunnels

## 7.1 Kinematic Release of Polyhedral Wedges

In shallow to intermediate depth tunnels driven through blocky, jointed rock masses, failure is rarely driven by crushing of intact rock. Instead, **gravity-induced fallouts of polyhedral rock wedges** bounded by intersecting discontinuities represent the dominant hazard.

For a wedge to detach and fall or slide into a tunnel void, two conditions must be met:
1. **Kinematic Feasibility**: The geometry of intersecting joint planes must form a closed tetrahedral or pentahedral wedge whose apex points away from the excavation void, and whose sliding direction daylighting into the opening is physically unobstructed.
2. **Limit Equilibrium Instability**: Driving forces (wedge gravity weight $W$ and joint water cleft pressures $U$) must exceed resisting forces (joint cohesion $c_j$, friction $\sigma_n' \tan\phi_j$, and installed rockbolt capacities $T$).

---

## 7.2 Stereographic Projection & Kinematic Analysis

Stereonets (equal-angle Wulff or equal-area Schmidt projections) plot 3D orientation data (Dip $\psi$ and Dip Direction $\alpha$) onto a 2D plane:

- **Great Circles**: Represent planes of discontinuities and tunnel excavation faces.
- **Poles**: Normal vectors perpendicular to discontinuity planes.
- **Intersections ($\vec{I}_{12}$)**: The plunge ($\beta$) and trend ($\theta$) of the line of intersection formed by two joint planes:

$$\vec{I}_{12} = \vec{n}_1 \times \vec{n}_2$$

### Sliding Modes:
- **Direct Falling (Roof Dropouts)**: The wedge apex lies vertically above the crown; all bounding planes dip steeper than their friction angles.
- **Single-Plane Sliding**: The intersection line daylights, but the wedge slides along the steeper of the two joint planes while detaching from the second.
- **Double-Plane Sliding**: The wedge slides along the line of intersection $\vec{I}_{12}$, with contact maintained on both joint faces simultaneously.

```
       Crown of Tunnel
     +-----------------+
      \     WEDGE     /
       \   (Weight W)/
        \    /\     /
         \  /  \   /   Joint Plane 2
          \/    \ /   (Dip psi_2)
 Joint Plane 1   v
 (Dip psi_1)   SLIDE VECTOR (Line of Intersection)
```

---

## 7.3 Limit Equilibrium Calculation: The UNWEDGE Method

For a wedge sliding along the line of intersection of Plane 1 and Plane 2 with plunge $\beta$:

### Driving Force ($F_{\text{drive}}$):

$$F_{\text{drive}} = W \sin\beta$$

### Normal Forces on Joint Faces ($N_1, N_2$):
Resolved by wedge equilibrium perpendicular to the intersection line:

$$N_1 + N_2 = W \cos\beta \cdot f(\text{wedge wedge geometry})$$

### Resisting Force ($F_{\text{resist}}$):

$$F_{\text{resist}} = (c_1 A_1 + N_1' \tan\phi_1) + (c_2 A_2 + N_2' \tan\phi_2) + \sum T_b \cos\theta_b$$

Where $A_1, A_2$ are face areas, $N'$ are effective normal forces reduced by pore cleft water pressures, and $T_b$ is the tensile capacity of intersecting rockbolts oriented at angle $\theta_b$ to the sliding vector.

$$FS = \frac{F_{\text{resist}}}{F_{\text{drive}}}$$

---

## 7.4 Support Design for Roof and Sidewall Wedges

1. **Dead-Weight Support Rule**: Pattern rockbolts must anchor the maximum anticipated wedge volume back into stable rock beyond the failure envelope with an anchor embedment length $\ge 1.5 - 2.0\text{ m}$.
2. **Bolt Spacing**: Bolt spacing $s$ must be smaller than the minimum dimensions of the expected wedge face to prevent small blocks falling out between bolts:
   
$$s \le \frac{1}{2} \text{Wedge Dimension}$$

3. **Shotcrete Integration**: Mesh-reinforced or steel fiber reinforced shotcrete (SFRS) provides immediate surface containment, preventing small keyblocks from ravelling and unravelling larger wedges.

---

## 7.5 Canonical Terminology

| English Term | Canonical Vietnamese Translation | Definition |
|--------------|-----------------------------------|------------|
| Kinematic analysis | Phân tích động học | Geometric assessment determining whether a rock wedge can physically detach |
| Stereographic projection | Phép chiếu lập thể cực | 2D graphical representation of 3D plane and line orientations |
| Line of intersection | Đường giao tuyến | Vector formed by the intersection of two discontinuity planes |
| Wedge failure | Phá hoại trượt nêm | Detachment of a polyhedral rock block bounded by intersecting joints |
| Keyblock | Khối nêm khóa | Critical surface block whose removal destabilizes adjacent rock masses |
