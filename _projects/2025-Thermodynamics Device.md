---
layout: project
title: De-icing Thermodynamic System Analysis
description: Analysis
image: /assets/images/350.png

---


### Problem

 I need to select a real-world instance of a thermodynamic system, explain how it works indetail, and then discuss how its performance would change under a change in design or operating conditions.

### Initial Design Choice

Take a Beechcraft King Air 350, which is a twin prop, low wing, T-tail aircraft. It can carry up to 11 passengers up to 2077 miles at 359 mph. Figures 1 and 2 show what the aircraft looks like.

<img src="/fa25-portfolio-tjc252/assets/images/figure1.png" alt="Thermo" style="max-width: 50%; height: auto;">
<img src="/fa25-portfolio-tjc252/assets/images/figure2.png" alt="Thermo" style="max-width: 50%; height: auto;">
I will model this aircraft's de-icing system. Information on the components can be found in figure 3 from Collins Aerospace inside of their Goodrich De-Icers. Specifically I am going the pick the left wing from the engine to wingtip.

<img src="/fa25-portfolio-tjc252/assets/images/figure3.png" alt="Thermo" style="max-width: 50%; height: auto;">

<img src="/fa25-portfolio-tjc252/assets/images/figure4.png" alt="Thermo" style="max-width: 50%; height: auto;">

### Modelling System

<img src="/fa25-portfolio-tjc252/assets/images/figure5.png" alt="Thermo" style="max-width: 100%; height: auto;">

As seen in Figure 5, flow exits the engine compressor and is tapped off at a bleed port. At this point the air has high pressure and temperature from the compressor and enters my de-icing system at state 1. The bleed air then passes through a flow control valve that I model as a throttling device. Across this valve there is a pressure drop and an increase in entropy, but negligible shaft work and negligible heat transfer. I assume steady state through the valve.

Downstream of the valve, the air enters the wing de-ice boot, which I model as a small inflation chamber or tank along the leading edge. During inflation, mass enters the chamber and the pressure inside rises while the boot volume expands slightly. In this control mass the amount of air and its internal energy increase temporarily as the boot inflates.

After the inflation phase, the system switches to the exhaust phase. Air is routed from the boot into an exhaust or vacuum line that dumps to a lower pressure region. This removes pressure from the boot so that it collapses back toward the wing surface. In practice, this inflation and exhaust cycle breaks ice off the leading edge and prevents further ice buildup. In my model, I treat the exhaust hardware as another throttling device with a pressure drop, negligible heat transfer, no shaft work, and entropy generation due to irreversibilities in the flow.

Throughout this system there is no shaft work crossing the boundaries of my control volumes, because the engine compressor work stays inside the engine. There is also negligible heat transfer to the surroundings because the ducts and lines are small and the process is fast. Energy is carried in and out entirely by the enthalpy of the flowing air.

### Assumptions for this Control Volume

<img src="/fa25-portfolio-tjc252/assets/images/figure6.png" alt="Thermo" style="max-width: 100%; height: auto;">

Compressor bleed: I do not model the compressor itself. I only take the outlet bleed air properties at state 1 (pressure P1, temperature T1, enthalpy h1). No work or heat crosses this system boundary.

Throttling device: steady state, adiabatic, no shaft work, negligible kinetic and potential energy changes, single inlet and outlet.

Tank: control mass that inflates. Transient process with accumulation of mass and internal energy, negligible heat transfer and shaft work, small changes in kinetic and potential energy. I neglect boundary work associated with boot expansion.

Exhaust: steady state throttling from boot pressure to an exhaust or vacuum pressure, adiabatic, no shaft work, negligible kinetic and potential energy changes.

### Equations of the System
<img src="/fa25-portfolio-tjc252/assets/images/figure7.png" alt="Thermo" style="max-width: 100%; height: auto;">

<img src="/fa25-portfolio-tjc252/assets/images/figure8.png" alt="Thermo" style="max-width: 100%; height: auto;">

<img src="/fa25-portfolio-tjc252/assets/images/figure9.png" alt="Thermo" style="max-width: 100%; height: auto;">

Figures 7, 8, and 9 show mass balance, energy balance, and entropy production.

### Effect of Changing Valve Setting

In normal operation, the flow control valve is sized and scheduled so that the de-ice boot inflates to a target pressure Pboot-nom within a short time interval. I consider a change where the valve is redesigned or operated with a larger effective flow area. For the same upstream compressor bleed pressure P1​, a larger valve opening increases the mass flow rate m2​ into the boot chamber.

From the mass balance for the boot, m2=dmboot/dt a larger m2 means that the mass inside the boot rises more quickly, so the pressure reaches the target value in a shorter inflation time. The energy balance for the boot, d(mboot*uboot)/dt also shows that a larger mass flow rate leads to a faster increase in the internal energy stored in the boot air. In practice, this gives a more rapid and possibly higher peak boot pressure.

The performance impact is two-sided. A faster inflation rate improves the system’s ability to break off ice, especially in severe icing where rapid boot cycling is important. However, the higher mass flow rate of bleed air slightly reduces the mass flow through the engine core and increases engine fuel consumption. A higher peak pressure also increases mechanical stresses in the boot material. If the pressure overshoots the design value, the boot can wear prematurely or even fail.

My model highlights this trade-off. Increasing the valve flow area improves anti-icing performance but at the cost of more entropy generation and more engine bleed losses. In a full design study, the valve schedule would be optimized to balance rapid ice removal against engine performance and boot durability.

### Sources Used

- https://moonjet.aero/blog/twin-engine-turboprop-planes-you-might-have-missed/
- https://www.goodrichdeicing.com/images/uploads/documents/Beechcraft.pdf
- https://www.facebook.com/Anika.Insana/posts/how-aircraft-de-icing-systems-work-%EF%B8%8F%EF%B8%8Fever-wondered-how-airplanes-stay-ice-free-i/623976260248911/
