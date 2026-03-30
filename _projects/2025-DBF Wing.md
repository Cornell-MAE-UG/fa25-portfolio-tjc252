---
layout: project
title: 2025/26 CUDBF Wing CAD
description: Designed the wing from scratch
image: /assets/images/fullplanefinal.png
---

# 2025/26 CUDBF Wing CAD

<div style="background-color:#f8f9fa; border-left:4px solid #3c4267; padding:14px 18px; border-radius:4px; margin:1.5em 0; font-size:0.97em; line-height:1.7;">On the Cornell Design Build Fly team, I led the airfoil selection, computationally analyzed different wing design choices, and built the full wing CAD for our 2025 aircraft.</div>

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/fullplanefinal.png" alt="Full plane CAD" style="max-width:100%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Full Plane CAD</em></p></div>

---

## Airfoil Selection

To choose the wing airfoil, I used a weighted trade matrix to compare candidates on aerodynamic performance and practical build constraints. I weighted $C_{L,\max}$ and manufacturability the highest because $C_{L,\max}$ sets stall speed (especially important for M3 with banner drag), and manufacturability drives surface quality and how cleanly the wing integrates with internal components like the servos and spar. I gave $C_L/C_D$ a moderate weight since the overall aircraft configuration also affects that ratio. I weighted $C_{L0}$ and stall angle the lowest because they were similar across the candidate airfoils and mattered less given that we were not limited by takeoff distance.

From a larger pool, I narrowed the shortlist to four airfoils: FX 60-126, MH-114, NACA 2412, and USA-35B. I analyzed these at the expected Reynolds number of 300,000 in XFLR5, and based on the comparisons, I identified the **FX 60-126** as the strongest option.

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/fullairfoil.png" alt="MATLAB plotted graphs of the airfoil analysis done in xFLR5" style="max-width:100%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Figure 4.4.1: Airfoil analysis in XFLR5</em></p></div>

---

## Wing Design and Integration

I designed the aircraft wing as a rectangular planform high-wing with no dihedral, no taper, and aileron control surfaces. Since we did not have a takeoff requirement, I chose not to implement flaps or flaperons. I modeled the wing and ailerons as rib-and-stringer structures, with one servo in each wing half. For structural support, I designed the wing around a single square carbon fiber spar that runs through both halves.

To minimize control surface gaps, I used CA hinges and added balsa reinforcement blocks to increase hinge bond area. I also implemented 3D printed PLA leading edges on the ailerons to further close the gap. I used an asymmetric triangular balsa piece for the trailing edge to keep stiffness while still matching the airfoil geometry.

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/full wing pictures.png" alt="Full wing CAD" style="max-width:100%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Figure 5.1.7: Full wing CAD in SOLIDWORKS</em></p></div>

---

## Endplate Research

I evaluated endplates by running CFD in ANSYS Fluent across multiple geometries. I ultimately decided **not** to include endplates because the aerodynamic improvement was small relative to the weight increase, added manufacturing complexity, and build time.

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/endplate cfd results results.png" alt="Pressure contours of the wing with different endplates" style="max-width:100%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Figure 5.1.8: Pressure contours across endplate geometries in ANSYS Fluent</em></p></div>

---

## Mathematical Performance

I used the following equations to evaluate turning performance and rate of climb (ROC):

**Turn radius and turn rate:**

$$R=\frac{v^{2}}{g\sqrt{n^{2}-1}}$$

$$\omega=\frac{g\sqrt{n^{2}-1}}{v}$$

I used a maximum load factor of $n = 2$ to represent a standard banked turn based on RC convention and our team's prior experience.

**Rate of climb:**

$$\mathrm{ROC}=\frac{v\,(T-D)}{W}$$

**Drag characterization:**

$$\mathrm{C}_D = \mathrm{C}_{D0} + \frac{\mathrm{C}_L^{2}}{\pi e\,AR}$$

I built a full drag characterization of DF1 using a mix of empirical analytical methods and numerical simulations, separating total drag into parasitic and induced components.

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/turning_climb_graphs.png" alt="MATLAB plotted graphs of turning performance and climb rate" style="max-width:100%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Figures 4.4.6–4.4.7: Turning performance and climb rate</em></p></div>

---

## Wing Manufacturing

To manufacture the wing and ailerons, I used a wooden rib-and-stringer approach assembled with wood glue and CA, then mounted everything on a square carbon fiber spar. I laser cut the ribs and combs from 1/8 in balsa or basswood — basswood for load-bearing parts and balsa for geometry-shaping components.

For the leading edge, I formed it from 1/32 in balsa sheet soaked in water to bend cleanly to the airfoil contour. For the trailing edge, I bonded 1/8 in balsa stringers into the rib notches using CA. I mounted the servos directly to a wing rib using 2-56 nylon fasteners, and after covering both wing halves and ailerons with MonoKote, I attached the ailerons with CA hinges.

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1.5em 0;"><figure style="flex:1; min-width:220px; margin:0; text-align:center;"><img src="/fa25-portfolio-tjc252/assets/images/wingmidmanu.png" alt="Wing midway through manufacturing" style="width:100%; height:260px; object-fit:contain;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Wing midway through manufacturing</em></figcaption></figure><figure style="flex:1; min-width:220px; margin:0; text-align:center;"><img src="/fa25-portfolio-tjc252/assets/images/planefly.png" alt="Iteration 2 flight test" style="width:100%; height:260px; object-fit:contain;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Iteration 2 flight test</em></figcaption></figure></div>

---

<div style="background-color:#f8f9fa; border-left:4px solid #3c4267; padding:12px 16px; border-radius:4px; margin:1em 0; font-size:0.93em;"><strong>Technologies used:</strong> XFLR5 &nbsp;·&nbsp; SOLIDWORKS &nbsp;·&nbsp; ANSYS Fluent &nbsp;·&nbsp; 3D printing &nbsp;·&nbsp; Hardwood and balsa construction</div>