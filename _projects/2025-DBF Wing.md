---
layout: project
title: 2025/26 CUDBF Wing CAD
description: Designed the wing from scratch
image: /assets/images/fullplanefinal.png

---

<img src="/fa25-portfolio-tjc252/assets/images/fullplanefinal.png" alt="Full plane CAD" style="max-width: 100%; height: auto;">

### Role

On the Cornell Design Build Fly team, I led the airfoil selection, computationally analyzed different wing design choices and then built the full wing CAD for our 2025 aircraft. Furthermore I also 

### Airfoil selection

To choose the wing airfoil, I used a weighted trade matrix to compare candidates on aerodynamic performance and practical build constraints. I weighted $C_{L,\max}$ and manufacturability the highest because $C_{L,\max}$ sets stall speed (especially important for M3 with banner drag), and manufacturability drives surface quality and how cleanly the wing integrates with internal components like the servos and spar. I gave $C_L/C_D$ a moderate weight since the overall aircraft configuration also affects that ratio. I weighted $C_{L0}$ and stall angle the lowest because they were similar across the candidate airfoils and mattered less given that we were not limited by takeoff distance.

From a larger pool, I narrowed the shortlist to four airfoils: FX 60-126, MH-114, NACA 2412, and USA-35B. I analyzed these at the expected Reynolds number of 300,000 in XFLR5 (Figure 4.4.1), and based on the comparisons, I identified the FX 60-126 as the strongest option.

<img src="/fa25-portfolio-tjc252/assets/images/fullairfoil.png" alt="MATLAB plotted graphs of the airfoil analysis done in xFLR5" style="max-width: 100%; height: auto;">

### Wing design and integration

I designed the aircraft wing as a rectangular planform high-wing with no dihedral, no taper, and aileron control surfaces. Since we did not have a takeoff requirement, I chose not to implement flaps or flaperons. I modeled the wing and ailerons as rib-and-stringer structures, with one servo in each wing half. For structural support, I designed the wing around a single square carbon fiber spar that runs through both halves.

To minimize control surface gaps, I used CA hinges and added balsa reinforcement blocks to increase hinge bond area. I also implemented 3D printed PLA leading edges on the ailerons to further close the gap. I used an asymmetric triangular balsa piece for the trailing edge to keep stiffness while still matching the airfoil geometry. I modeled the full wooden wing structure and servo mechanism in SOLIDWORKS (Figure 5.1.7).

<img src="/fa25-portfolio-tjc252/assets/images/full wing pictures.png" alt="Full wing CAD" style="max-width: 100%; height: auto;">

### Endplate Research

I evaluated endplates by running CFD in ANSYS Fluent across multiple geometries (Figure 5.1.8). I ultimately decided not to include endplates because the aerodynamic improvement was small relative to the weight increase, added manufacturing complexity, and build time.

<img src="/fa25-portfolio-tjc252/assets/images/endplate cfd results results.png" alt="Pressure contours of the wing with different endplates" style="max-width: 100%; height: auto;">

### Mathematical Performance

I used Equations (1) and (2) to evaluate turning performance (Fig. 4.4.6). The plot shows turn rate versus airspeed with families of curves for constant load factor and constant turn radius. As airspeed increases, the design becomes load-factor-limited due to structural constraints, so I used a maximum load factor of {% raw %}\(n = 2\){% endraw %} to represent a standard banked turn based on RC convention and our team’s prior experience. I included constant-radius curves to give geometric context for the maneuvering envelope.

$$
R=\frac{v^{2}}{g\sqrt{n^{2}-1}}
$$
*(1)*

$$
\omega=\frac{g\sqrt{n^{2}-1}}{v}
$$
*(2)*

I calculated ROC for each mission using Equation (3). Figure 4.4.7 summarizes the results, and the ROC values landed in the expected range based on prior DBF aircraft and our team research.

$$
\mathrm{ROC}=\frac{v\,(T-D)}{W}
$$
*(3)*

For drag, I built a full drag characterization of DF1 using a mix of empirical analytical methods and numerical simulations. I separated total drag into parasitic and induced components and used Equation (4) for the overall drag coefficien:

$$
\mathrm{C}_D = \mathrm{C}_{D0} + \frac{\mathrm{C}_L^{2}}{\pi e\,AR}
$$
*(4)*

<img src="/fa25-portfolio-tjc252/assets/images/turning_climb_graphs.png" alt="MATLAB plotted graphs of turning performance and climb rate" style="max-width: 100%; height: auto;">

### Wing manufacturing

To manufacture the wing and ailerons, I used a wooden rib-and-stringer approach assembled with wood glue and CA, then mounted everything on a square carbon fiber spar. I chose to laser cut the ribs and combs from 1/8 in balsa or basswood depending on what each piece needed to do: basswood for the more load-bearing parts and balsa for components that were primarily shaping the geometry. Before covering, the full wooden structure is shown. 

<img src="/fa25-portfolio-tjc252/assets/images/wingmidmanu.png" alt="Wing midway through manufacturing" style="max-width: 100%; height: auto;">

For the leading edge, I formed it from 1/32 in balsa sheet. I soaked the sheet in water so it could bend cleanly, then molded it to match the airfoil contour. For the trailing edge, I bonded 1/8 in balsa stringers into the rib notches using CA. This gave the wing a clean, continuous edge and provided a rigid skeleton that the MonoKote could pull tight over without collapsing or warping the structure.

For integration, I mounted the servos directly to a wing rib using 2-56 nylon fasteners. After covering the wing halves and ailerons with MonoKote, I attached the ailerons with CA hinges to keep the gap small and maintain consistent control feel.

<img src="/fa25-portfolio-tjc252/assets/images/planefly.png" alt="Iteration 2 flight test" style="max-width: 100%; height: auto;">

**Technologies used:** XFLR5, SOLIDWORKS, ANSYS Fluent, 3D printing, hardwood and balsa construction
