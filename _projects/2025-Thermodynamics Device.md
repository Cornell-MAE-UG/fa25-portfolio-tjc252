---
layout: project
title: De-icing Thermodynamic System Analysis
description: Analysis
image: /assets/images/350.png
permalink: /projects/2025-Thermodynamics/
---


<div style="background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:14px 18px; border-radius:4px; margin:1.5em 0; font-size:0.97em; line-height:1.7;">Selected a real-world thermodynamic system, modeled it using control volume analysis, and evaluated how performance changes under a modified operating condition.</div>

---

## Problem

I need to select a real-world instance of a thermodynamic system, explain how it works in detail, and then discuss how its performance would change under a change in design or operating conditions.

---

## Aircraft Selection

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1.5em 0;"><figure style="flex:1; min-width:200px; margin:0; text-align:center;"><img src="/trevor_crouse/assets/images/figure1.png" alt="Beechcraft King Air 350" style="width:100%; height:220px; object-fit:contain;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Figure 1: Beechcraft King Air 350</em></figcaption></figure><figure style="flex:1; min-width:200px; margin:0; text-align:center;"><img src="/trevor_crouse/assets/images/figure2.png" alt="King Air 350 interior" style="width:100%; height:220px; object-fit:contain;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Figure 2: King Air 350 profile</em></figcaption></figure></div>

The Beechcraft King Air 350 is a twin-prop, low-wing, T-tail aircraft capable of carrying up to 11 passengers over 2,077 miles at 359 mph. I modeled its **pneumatic de-icing system**, focusing on the left wing from engine to wingtip using Goodrich De-Icers components.

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1.5em 0;"><figure style="flex:1; min-width:200px; margin:0; text-align:center;"><img src="/trevor_crouse/assets/images/figure3.png" alt="De-icer components" style="width:100%; height:220px; object-fit:contain;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Figure 3: Collins Aerospace Goodrich De-Icer components</em></figcaption></figure><figure style="flex:1; min-width:200px; margin:0; text-align:center;"><img src="/trevor_crouse/assets/images/figure4.png" alt="System layout" style="width:100%; height:220px; object-fit:contain;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Figure 4: System layout</em></figcaption></figure></div>

---

## Modelling the System

<div style="text-align:center; margin:1.5em 0;"><img src="/trevor_crouse/assets/images/figure5.png" alt="Control volume diagram" style="max-width:85%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Figure 5: Control volume schematic of the de-icing system</em></p></div>

Flow exits the engine compressor and is tapped off at a bleed port, entering the de-icing system at state 1 with high pressure and temperature. The bleed air then passes through a **flow control valve** modeled as a throttling device — pressure drops, entropy increases, with negligible shaft work and heat transfer.

Downstream, the air enters the **wing de-ice boot**, modeled as a small inflation chamber along the leading edge. During inflation, mass enters and pressure rises as the boot volume expands. After inflation, air is routed to an **exhaust line** — another throttling device — which collapses the boot back to the wing surface, breaking off accumulated ice.

<div style="background-color:#f0f0f0; border-left:4px solid #aaa; padding:12px 16px; border-radius:4px; margin:1em 0; font-size:0.93em; color:#555;">Throughout this system, no shaft work crosses the control volume boundaries (engine compressor work stays inside the engine), and heat transfer is negligible due to the small duct size and fast process. Energy is carried entirely by the enthalpy of the flowing air.</div>

---

## Assumptions

<table style="width:100%; border-collapse: collapse; font-size: 0.95em; margin: 1.5em 0;">
  <thead>
    <tr style="background-color: #3a3f58; color: white; text-align: left;">
      <th style="padding: 10px 12px;">Component</th>
      <th style="padding: 10px 12px;">Assumptions</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Compressor bleed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Not modeled; only outlet bleed properties at state 1 are used. No work or heat crosses this boundary.</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Throttling valve</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Steady state, adiabatic, no shaft work, negligible kinetic and potential energy changes, single inlet and outlet.</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Boot (tank)</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Transient control mass, negligible heat transfer and shaft work, boundary work from boot expansion neglected.</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Exhaust</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Steady state throttling from boot pressure to exhaust pressure, adiabatic, no shaft work.</td>
    </tr>
  </tbody>
</table>

<div style="text-align:center; margin:1.5em 0;"><img src="/trevor_crouse/assets/images/figure6.png" alt="Assumptions diagram" style="max-width:75%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Figure 6: Annotated control volume with assumptions</em></p></div>

---

## Equations of the System

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1.5em 0;"><figure style="flex:1; min-width:180px; margin:0; text-align:center;"><img src="/trevor_crouse/assets/images/figure7.png" alt="Mass balance" style="width:100%; height:auto;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Figure 7: Mass balance</em></figcaption></figure><figure style="flex:1; min-width:180px; margin:0; text-align:center;"><img src="/trevor_crouse/assets/images/figure8.png" alt="Energy balance" style="width:100%; height:auto;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Figure 8: Energy balance</em></figcaption></figure><figure style="flex:1; min-width:180px; margin:0; text-align:center;"><img src="/trevor_crouse/assets/images/figure9.png" alt="Entropy production" style="width:100%; height:auto;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Figure 9: Entropy production</em></figcaption></figure></div>

---

## Effect of Changing Valve Setting

In normal operation, the flow control valve is sized so that the de-ice boot inflates to a target pressure $P_{\text{boot-nom}}$ within a short interval. I consider a redesign where the valve has a **larger effective flow area**.

For the same upstream bleed pressure $P_1$, a larger opening increases mass flow into the boot. From the mass balance:

$$\dot{m}_2 = \frac{dm_{\text{boot}}}{dt}$$

A larger $\dot{m}_2$ means the boot reaches target pressure faster. The energy balance:

$$\frac{d(m_{\text{boot}}\, u_{\text{boot}})}{dt} = \dot{m}_2 h_2$$

shows that internal energy also rises more rapidly, giving a higher peak boot pressure.

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1.5em 0;">
<div style="flex:1; min-width:180px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;">
<div style="font-size:0.8em; color:#666; margin-bottom:4px;">Benefit</div>
<div style="font-size:0.95em; color:#3a3f58; font-weight:bold;">Faster inflation → better ice removal in severe icing</div>
</div>
<div style="flex:1; min-width:180px; background-color:#f7f8fa; border-left:4px solid #aaa; padding:12px 16px; border-radius:4px;">
<div style="font-size:0.8em; color:#666; margin-bottom:4px;">Cost</div>
<div style="font-size:0.95em; color:#555; font-weight:bold;">More bleed air → higher fuel consumption + boot wear risk</div>
</div>
</div>

My model highlights this trade-off: increasing valve flow area improves anti-icing performance but at the cost of more entropy generation and greater engine bleed losses. In a full design study, the valve schedule would be optimized to balance rapid ice removal against engine performance and boot durability.

---

## References

<div style="font-size:0.95em; line-height:1.7;">
<p>1. <a href="https://moonjet.aero/blog/twin-engine-turboprop-planes-you-might-have-missed/">moonjet.aero — Twin Engine Turboprop Planes</a></p>
<p>2. <a href="https://www.goodrichdeicing.com/images/uploads/documents/Beechcraft.pdf">Goodrich De-Icers — Beechcraft Component Reference</a></p>
<p>3. <a href="https://www.facebook.com/Anika.Insana/posts/how-aircraft-de-icing-systems-work-%EF%B8%8F%EF%B8%8Fever-wondered-how-airplanes-stay-ice-free-i/623976260248911/">How Aircraft De-Icing Systems Work</a></p>
</div>