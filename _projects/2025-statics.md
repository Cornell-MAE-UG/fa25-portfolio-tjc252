---
layout: project
title: Maximizing Lift of a Linear Actuator
description: Analysis
image: /assets/images/12loads.png
---

# Maximizing Lift of a Linear Actuator

<div style="background-color:#f8f9fa; border-left:4px solid #3c4267; padding:14px 18px; border-radius:4px; margin:1.5em 0; font-size:0.97em; line-height:1.7;">Designed a planar lifting mechanism in a 150 cm × 50 cm workspace using a rigid bar, three pin supports, and a catalog linear actuator. Optimized for maximum payload height while constraining beam deflection to under 2% of beam length.</div>

---

## Problem

I need to design a planar lifting mechanism in a 150 cm by 50 cm workspace. Using a rigid bar of chosen length, three pin supports (two fixed to the ground), and one linear actuator from a provided catalog, I needed to design a frame that lifted the maximum possible weight to the highest possible height, assuming all elements behaved as rigid bodies.

---

## Design Choice

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1.5em 0;">
<div style="flex:1; min-width:140px; background-color:#f8f9fa; border-left:4px solid #3c4267; padding:12px 16px; border-radius:4px;">
<div style="font-size:0.8em; color:#666; margin-bottom:4px;">Actuator Selected</div>
<div style="font-size:1.2em; font-weight:bold; color:#3c4267;">IMA44 RN05</div>
</div>
<div style="flex:1; min-width:140px; background-color:#f8f9fa; border-left:4px solid #3c4267; padding:12px 16px; border-radius:4px;">
<div style="font-size:0.8em; color:#666; margin-bottom:4px;">Peak Load Rating</div>
<div style="font-size:1.2em; font-weight:bold; color:#3c4267;">3,850 lbf</div>
</div>
<div style="flex:1; min-width:140px; background-color:#f8f9fa; border-left:4px solid #3c4267; padding:12px 16px; border-radius:4px;">
<div style="font-size:0.8em; color:#666; margin-bottom:4px;">Bar Length</div>
<div style="font-size:1.2em; font-weight:bold; color:#3c4267;">45 cm</div>
</div>
<div style="flex:1; min-width:140px; background-color:#f8f9fa; border-left:4px solid #3c4267; padding:12px 16px; border-radius:4px;">
<div style="font-size:0.8em; color:#666; margin-bottom:4px;">Payload Height Range</div>
<div style="font-size:1.2em; font-weight:bold; color:#3c4267;">9.4 – 39.7 cm</div>
</div>
</div>

Placing the actuator at 0.6L gave a good compromise between mechanical advantage and allowable stroke. With the base at (90, 0) and point A positioned to clear the workspace, the usable motion range was **12° to 62°**, satisfying the deflection constraint throughout.

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/problem4.png" alt="Problem setup and geometry" style="max-width:85%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Problem geometry and design parameters</em></p></div>

---

## Step 2 — Rigid-Bar Design

<div style="background-color:#f0f0f0; border-left:4px solid #aaa; padding:12px 16px; border-radius:4px; margin:1em 0; font-size:0.93em; color:#555; font-style:italic;">All elements treated as rigid bodies for this phase.</div>

- Defined the problem geometry, constraints, objectives, and design degrees of freedom
- Performed a full static analysis of the mechanism to size the actuator and locate the supports
- Chose an actuator that could provide the required force over the needed stroke
- Produced the final rigid-body design as free-body diagrams and hand calculations

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/part2.png" alt="Rigid bar static analysis" style="max-width:85%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em>Static analysis and free-body diagrams — rigid bar design</em></p></div>

---

## Step 3 — Flexible-Bar Design and Deflection

In the final step the bar was treated as a beam that bends under the combined weight and actuator force.

<table style="width:100%; border-collapse: collapse; font-size: 0.95em; margin: 1.5em 0;">
  <thead>
    <tr style="background-color: #3c4267; color: white; text-align: left;">
      <th style="padding: 10px 12px;">Task</th>
      <th style="padding: 10px 12px;">Approach</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #f8f9fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Deflection modeling</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Modeled bar as a beam under worst-case combined loading; calculated maximum vertical deflection</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Cross-section selection</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Selected material and cross-section to keep deflection below 2% of beam length with minimum weight</td>
    </tr>
    <tr style="background-color: #f8f9fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Dimension update</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Updated mechanism dimensions to avoid singular positions and maintain smooth motion over full actuator travel</td>
    </tr>
  </tbody>
</table>

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1.5em 0;"><figure style="flex:1; min-width:220px; margin:0; text-align:center;"><img src="/fa25-portfolio-tjc252/assets/images/part3a.png" alt="Beam deflection analysis" style="width:100%; height:auto;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Beam deflection analysis</em></figcaption></figure><figure style="flex:1; min-width:220px; margin:0; text-align:center;"><img src="/fa25-portfolio-tjc252/assets/images/part3bc.png" alt="Updated mechanism dimensions" style="width:100%; height:auto;"><figcaption style="margin-top:6px; font-size:0.9em;"><em>Updated mechanism dimensions and motion range</em></figcaption></figure></div>

---

<div style="background-color:#f8f9fa; border-left:4px solid #3c4267; padding:12px 16px; border-radius:4px; margin:1em 0; font-size:0.93em;"><strong>Methods used:</strong> Static analysis &nbsp;·&nbsp; Free-body diagrams &nbsp;·&nbsp; Beam deflection &nbsp;·&nbsp; Cross-section optimization &nbsp;·&nbsp; Actuator catalog selection</div>