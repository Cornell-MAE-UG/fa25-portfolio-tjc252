---
layout: default
permalink: /O6_ClientReport/
fontsize: 11pt
geometry: margin=1in
papersize: letter
pagestyle: empty
header-includes:
  - \pagenumbering{gobble}
---

# BuzzKill Jaw Bucket: Client Report

<div style="background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px; margin:1em 0;"><strong>Team Buzzkill:</strong> Ethan Moger (ejm349), Bennett Wehibe (bdw56), Adair Bluman (ahb234), Trevor Crouse (tjc252), Allen Liu (al2593)</div>

---

## Context and Problem Statement

We took on the challenge of controlling the egg masses of spotted lanternflies (SLF) as it was more efficient than targeting SLF in its adult stage. Individual egg masses contain 30–50 eggs, can be laid on organic or inorganic surfaces, and can still hatch if scraped off the surface (1, 5). Current egg mass control strategies fail to ensure destruction or provide a reliable way to quantify egg mass management.

Our challenge was to develop a mechanical system that ensures destruction of egg masses across various surfaces and enables growers to numerically analyze the system's success. Our main constraints were making the device user-friendly, lightweight, easy to manufacture, and effective against large numbers of egg masses, which we analyzed by creating numerical testing protocols for each design driver. By combatting the SLF invasion via egg masses, we are addressing the issue at its source in a manner that is far more efficient than attempting to kill individual adult SLFs.

---

## Final Prototype and Application

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/labeled_eggst.png" alt="Final Prototype with Labeled Components" style="max-width:90%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em><strong>Figure 1: Final CAD Prototype with Labeled Components</strong></em></p></div>

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/sliding_head_eggst.png" alt="Removable Basket Detail View" style="max-width:75%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em><strong>Figure 2: Removable Basket Detail</strong></em></p></div>

Our final prototype consists of a device designed to easily remove SLF egg masses. The prototype weighs 3.6 kg and measures 1.5 m in length. Materials include PVC pipe, springs, string, and a hinge — all sourced from McMaster-Carr or fabricated in the Taylor Design Studio (TDS) and Rapid Prototyping Lab (RPL).

### Key Features

<table style="width:100%; border-collapse: collapse; font-size: 0.95em; margin: 1.5em 0;">
  <thead>
    <tr style="background-color: #3a3f58; color: white; text-align: left;">
      <th style="padding: 10px 12px;">Feature</th>
      <th style="padding: 10px 12px;">Function</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; font-weight:600;">Scraping Edge (Jaw)</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Optimized to match the adhesion of egg masses, allowing for more complete removal in a single pass</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; font-weight:600;">Ergonomic Handle System</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Adjustable handle gives users better control over force and angle, reducing fatigue and improving consistency</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; font-weight:600;">Collection Bucket</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">25 in³ (410 cm³) capacity — estimated to hold 100 egg masses at once</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; font-weight:600;">Internal Divider</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Prevents already-collected egg masses from falling out when collecting more</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; font-weight:600;">Removable Basket</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Holds egg masses past the divider; pulls out for easy disposal</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; font-weight:600;">Pivoting Head</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Allows removal from a variety of heights while keeping the bucket-jaw assembly level</td>
    </tr>
  </tbody>
</table>

### Operating Procedure

The user operates the prototype with a cross-body orientation. First, the head angle is set based on egg mass height. The shoulder stock is placed at the shoulder, and the handle is adjusted for the opposite hand. The pull handle is drawn back and set on the pull handle lock, holding the jaw open. With the bucket positioned, the pull handle is released off the lock, snapping the jaw closed and scraping the egg mass off. The divider is then opened to let the egg mass fall into the basket and re-closed. The process repeats for each egg mass collected, and when the bucket is filled the basket is pulled out for disposal.

---

## Conclusion and Recommendation

The intended goal of the prototype was to efficiently collect egg masses while remaining comfortable for the user across a range of heights. We achieved an average of 2.65 seconds per egg mass — incredibly efficient compared to current credit-card scraping solutions. The design performed favorably on the Rapid Upper Limb Assessment (RULA), scoring a 3.9 (a score below 4 indicates an ergonomic design (2)). The scraping jaw generated 12.5 N of force, decreasing by 8% to 11.5 N after 100 cycles.

These tests indicate that the design meets our two main objectives — efficiency and comfort — though there are areas for improvement. We recommend implementing electronic motors to open and close the jaw, pivot the head, and operate the divider. These adjustments would eliminate spring wear-induced force loss and allow full operation from a single position.

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1em 0;">
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">Total Project Spend</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">$211.27</div><div style="font-size:0.8em; color:#666;">39.6% under budget</div></div>
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">Final Prototype Cost</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">$104.62</div><div style="font-size:0.8em; color:#666;">29.9% of budget</div></div>
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">3D-Printed Parts</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">$29.30</div><div style="font-size:0.8em; color:#666;">Reducible at scale</div></div>
</div>

The design is not only efficient against our success criteria, but would also be affordable at scale. We conclude that the prototype is worth pursuing further as a successful proof of concept. For an industry-grade product, we recommend implementing electronic motors for bucket angle, jaw, and divider control, and using a malleable material for the tooth so it can contour to the scraping surface.

---

## Testing and Results

### Test One: Egg Mass Removal Efficiency

**Testing:** Time required and effectiveness of removing a batch of simulated egg masses.

**How to Perform:** Placed 20 Play-Doh egg masses (~1 in × 1 in × 0.5 in) at varying heights and timed full collection.

**Results:**

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1em 0;">
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">Total Time</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">53 s</div></div>
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">Avg. per Egg Mass</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">2.65 s</div></div>
  <div style="flex:1; min-width:150px; background-color:#3a3f58; border-left:4px solid #2a2f4a; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#ccc; margin-bottom:4px;">Removal Rate</div><div style="font-size:1.4em; font-weight:bold; color:white;">100%</div></div>
</div>

**Conclusion:** Egg mass removal efficiency is one of our success criteria and is vital to foster effective integration within farms. The device is efficient in egg mass removal.

### Test Two: Jaw Opening Range

**Testing:** Maximum jaw opening relative to average SLF egg mass length.

**How to Perform:** Used a dial caliper to measure opening distance with the pull handle clipped to the pull-handle lock.

**Results:**

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1em 0;">
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">Max Opening</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">87 mm</div></div>
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">Avg. SLF Egg Mass</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">~50 mm</div></div>
  <div style="flex:1; min-width:150px; background-color:#3a3f58; border-left:4px solid #2a2f4a; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#ccc; margin-bottom:4px;">Headroom</div><div style="font-size:1.4em; font-weight:bold; color:white;">+74%</div></div>
</div>

**Conclusion:** Device is sufficiently large to remove an average egg mass in one scrape.

### Test Three: Jaw Clamping Force and Durability

**Testing:** Scraping force at the jaw teeth and durability over 100 cycles.

**How to Perform:** Measured force using a spring scale at the jaw teeth, then cycled the actuating system 100 times and re-measured.

**Results:**

<table style="width:100%; border-collapse: collapse; font-size: 0.95em; margin: 1.5em 0;">
  <thead>
    <tr style="background-color: #3a3f58; color: white; text-align: left;">
      <th style="padding: 10px 12px;">Metric</th>
      <th style="padding: 10px 12px;">Initial</th>
      <th style="padding: 10px 12px;">After 100 Cycles</th>
      <th style="padding: 10px 12px;">Change</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Clamping Force</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">12.5 N</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">11.5 N</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">−8.0%</td>
    </tr>
  </tbody>
</table>

**Conclusion:** Clamping force is sufficient for scraping, and the device exceeds our 10 N target both before and after cycling. However, the &gt;5% force reduction after 100 uses exceeds our durability tolerance — an electric motor is recommended for the next iteration to eliminate spring-wear loss.

### Test Four: Ergonomic Assessment (RULA)

**Testing:** Musculoskeletal disorder (MSD) risk and overall user comfort across operating heights and angles.

**How to Perform:** RULA XL testing via CUergo (4), incorporating device weight, length, and percentage of operation time in each body position. Average grip strength data (6) and pruning shear force benchmarks (7) informed force targets.

**Results:**

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1em 0;">
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">RULA Score</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">3.9</div><div style="font-size:0.8em; color:#666;">Target: &lt;4</div></div>
  <div style="flex:1; min-width:150px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#444; margin-bottom:4px;">Device Weight</div><div style="font-size:1.4em; font-weight:bold; color:#3a3f58;">&lt;8 lbs</div><div style="font-size:0.8em; color:#666;">Target: &lt;15 lbs</div></div>
  <div style="flex:1; min-width:150px; background-color:#3a3f58; border-left:4px solid #2a2f4a; padding:12px 16px; border-radius:4px;"><div style="font-size:0.8em; color:#ccc; margin-bottom:4px;">Status</div><div style="font-size:1.4em; font-weight:bold; color:white;">PASS</div></div>
</div>

**Conclusion:** With a RULA score of 3.9 (below the threshold of 4), the design is ergonomic and comfortable for users across the expected operating envelope.

---

## Prototype and Testing Details

To construct the final prototype, we cut the PVC pipe to size and drilled ¼ in holes at the desired locations to bolt the 3D-printed components to the pipe and thread the string through the pipe to connect the pull handle and jaw scraper. We created seven 3D-printed PLA components: latches, jaw, pivoting head attachment, handle, pull handle lock, shoulder stock, and bucket. Components attach by sliding onto the pipe and fastening with M6 and AN4 bolts. The divider, basket, and string catch were constructed from cut balsa wood, sanded, and glued together. The latches — which hold the basket and divider shut when desired — were attached using M6 bolts. The jaw assembly uses M6 bolts to attach the hinge, with the springs zip-tied to tabs inside the jaw.

<div style="text-align:center; margin:1.5em 0;"><img src="/fa25-portfolio-tjc252/assets/images/eggst_exploded.png" alt="Exploded CAD View of Final Prototype" style="max-width:90%; height:auto;"><p style="margin-top:6px; font-size:0.9em;"><em><strong>Figure 3: Exploded CAD View of Final Prototype</strong></em></p></div>

### Pipe Length Sizing

To determine PVC pipe length, we performed a torque balance using the average peak full-flexion shoulder torque for right-handed males of 19.92 ft-lb (3). Estimating the bucket plus 100 collected egg masses at ~2.5 lb gives a maximum length of roughly 8 ft. Accounting for PVC flex, we elected for a 3.5 ft pipe and a 5 ft total design length.

<div style="background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px; margin:1em 0;"><strong>Testing Methodology Summary:</strong> Play-Doh simulated egg masses were used at ~1 in × 1 in × 0.5 in. The 50 mm jaw opening requirement was based on fitting around and scraping an average egg mass in one motion, measured via dial caliper. The clamp force test was motivated by observations that egg masses can be removed with a plastic card (low force required) and was measured with a spring scale at the jaw teeth. RULA XL testing was selected because the device is used at varying heights, angles, and body positions.</div>

---

## Appendix

### Table 1: Final Prototype Parts List

<table style="width:100%; border-collapse: collapse; font-size: 0.95em; margin: 1.5em 0;">
  <thead>
    <tr style="background-color: #3a3f58; color: white; text-align: left;">
      <th style="padding: 10px 12px;">Part</th>
      <th style="padding: 10px 12px;">Specs</th>
      <th style="padding: 10px 12px;">McMaster Code</th>
      <th style="padding: 10px 12px;">Fabrication Details</th>
      <th style="padding: 10px 12px; text-align: right;">Price [$]</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Bucket</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">165×140×220mm bounding box; PLA; 410 cm³ inner volume</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">17.20</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Jaw</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">140×75×10mm bounding box; PLA; tooth at end for scraping</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">1.60</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Divider</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">⅛ in balsa wood; 3.18×142×134mm</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Cut to size and sanded in TDS</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">Free</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Basket</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">¼ in balsa wood; 45×142×134mm</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Cut to size and sanded in TDS</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">Free</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Pivot Attachment</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">PLA; attaches to tube and bucket; allows pivoting</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">5.80</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Handle Holder</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">PLA; holds pull handle in open position</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">0.90</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Latches (×2)</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">PLA; hold basket and divider closed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">0.15</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Clevis Pin</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Carbon steel, 3/16" diameter, 2-13/16" usable length</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">98306A120</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">12.10</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Cotter Pin</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Spring steel, fits 3/16"–1/4" pin diameter, 3/64" wire</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">90492A220</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">4.12</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Extension Jaw Springs</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Steel, 1.5" long, 0.24" OD, 0.022" wire, 0.7 lbf/in</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">5108N214</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">16.92</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Nylon Tube</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">1/16" wall, 1.25" OD, 1.125" ID, 5 ft length</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">8628K74</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Cut to 3.5 ft long in TDS</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">25.88</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Handle</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">152×42×180mm bounding box; PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">2.30</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Pull Handle</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Open-ended, two-arm, black anodized aluminum, 10-24 thread</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">11625A31</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">5.82</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">String</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">585 mm length</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">Free</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Shoulder Stock</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">127×40×40mm bounding box; PLA; M6 bolt; padded</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">1.35</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Hinge</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Polycarbonate, 2.5×2.125×0.2 in; four M6 bolts</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">1635A24</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">6.75</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">M6 Bolts and Nuts</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Nine total: 6 @ 16mm, 3 @ 50mm</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Sourced from TDS</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">Free</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Handle Grip / Stock Padding</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">2 ft, Buna-N-Foam, 1.25" OD</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">9754K643</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Cut and hot-glued to pipe and shoulder stock</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">3.73</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">AN-Spec Bolts and Locknuts</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">2× each: AN4-30, ¼"-28 thread</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Sourced from ELL</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">Free</td>
    </tr>
    <tr style="background-color: #3a3f58; color: white; font-weight: bold;">
      <td style="padding: 10px 12px;" colspan="4">Total</td>
      <td style="padding: 10px 12px; text-align: right;">104.62</td>
    </tr>
  </tbody>
</table>

### Table 2: Bill of Materials for Remaining Items (Earlier Iterations)

<table style="width:100%; border-collapse: collapse; font-size: 0.95em; margin: 1.5em 0;">
  <thead>
    <tr style="background-color: #3a3f58; color: white; text-align: left;">
      <th style="padding: 10px 12px;">Part</th>
      <th style="padding: 10px 12px;">Specs</th>
      <th style="padding: 10px 12px;">McMaster Code</th>
      <th style="padding: 10px 12px;">Fabrication Details</th>
      <th style="padding: 10px 12px; text-align: right;">Price [$]</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">PVC Pipe</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3 ft, 1.125" OD, 0.625" ID; chemical-resistant oversized round PVC</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">8749K77</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Sanded in TDS to correct diameter</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">43.23</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Two Extension Springs</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">302 SS, corrosion-resistant, 2" long, 0.180" OD, 0.022" wire</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">9065K575</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">10.76</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Pack of 3 Extension Springs</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">302 SS, corrosion-resistant, 2" long, 0.5" OD, 0.055" wire</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">9065K343</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">No fabrication needed</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">10.11</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Bucket v1</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">215×200×168.5mm bounding box; PLA; 27 in³ inner volume</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">20.05</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Jaw v1</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">200×75×10mm bounding box; PLA; tooth attached</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">4.40</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Handle v1</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">152×42×180mm bounding box; PLA; trigger slides in internal rails</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">8.85</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Trigger v1</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">15×36×130mm bounding box; PLA; string attached for jaw actuation</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">0.80</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Shoulder Stock v1</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">127×50×38mm bounding box; PLA; M6 bolt; padded</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">4.60</td>
    </tr>
    <tr style="background-color: #f7f8fa;">
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Handle v2</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">152×42×180mm bounding box; PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">2.25</td>
    </tr>
    <tr>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">Jaw v2</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">140×75×10mm bounding box; PLA; tooth at end for scraping</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">N/A</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6;">3D printed in RPL using PLA</td>
      <td style="padding: 9px 12px; border-bottom: 1px solid #dee2e6; text-align: right;">1.60</td>
    </tr>
    <tr style="background-color: #3a3f58; color: white; font-weight: bold;">
      <td style="padding: 10px 12px;" colspan="4">Total</td>
      <td style="padding: 10px 12px; text-align: right;">106.65</td>
    </tr>
  </tbody>
</table>

<div style="background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:12px 16px; border-radius:4px; margin:1em 0;"><strong>Combined Project Total:</strong> $104.62 (final prototype) + $106.65 (earlier iterations) = <strong>$211.27</strong> — 39.6% under the project budget.</div>

---

## Group Absences Reflection

<div style="display:flex; gap:16px; flex-wrap:wrap; margin:1em 0;">
  <div style="flex:1; min-width:280px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:14px 18px; border-radius:4px;">
    <div style="font-weight:600; color:#3a3f58; margin-bottom:6px;">Allen — 04/06</div>
    <div style="font-size:0.92em; line-height:1.55;">The team confirmed Allen's progress in his role before the absence and used office hours to begin assembling the final prototype ahead of the lab section. This let us verify all components were on hand and let individual members focus on specific subassemblies without Allen present.</div>
  </div>
  <div style="flex:1; min-width:280px; background-color:#f7f8fa; border-left:4px solid #3a3f58; padding:14px 18px; border-radius:4px;">
    <div style="font-weight:600; color:#3a3f58; margin-bottom:6px;">Trevor — 04/20</div>
    <div style="font-size:0.92em; line-height:1.55;">The team met during the week before the presentation to rewrite and rehearse the elevator pitch with adjustments covering Trevor's planned part. We informed him of the progress made on his return, providing a smooth transition.</div>
  </div>
</div>

---

## References

<div style="font-size:0.95em; line-height:1.7;">
<p>1. Keller, J., Rost, J., Hoover, K., Urban, J., Leach, H., Porras, M., Walsh, B., Bosold, M., Calvin, D. "Dispersion Patterns and Sample Size Estimates for Egg Masses of Spotted Lanternfly (Hemiptera: Fulgoridae)." <em>Environmental Entomology</em>, vol. 49, no. 6, Dec. 2020, pp. 1462–1472. <a href="https://doi.org/10.1093/ee/nvaa107">https://doi.org/10.1093/ee/nvaa107</a></p>
<p>2. Ergonomics Plus. <em>A Step-by-Step Guide: Rapid Upper Limb Assessment (RULA).</em> <a href="https://ergo-plus.com/wp-content/uploads/RULA-A-Step-by-Step-Guide1.pdf">https://ergo-plus.com/wp-content/uploads/RULA-A-Step-by-Step-Guide1.pdf</a>. Accessed 23 Mar. 2026.</p>
<p>3. Soderberg, G. J., and Blaschak, M. J. "Shoulder Internal and External Rotation Peak Torque Production Through a Velocity Spectrum in Differing Positions." <em>Journal of Orthopaedic & Sports Physical Therapy</em>, vol. 8, no. 11, May 1987, pp. 518–24. <a href="https://doi.org/10.2519/jospt.1987.8.11.518">https://doi.org/10.2519/jospt.1987.8.11.518</a></p>
<p>4. Hedge, Alan. <em>CUergo: RULA.</em> Cornell University, <a href="https://ergo.human.cornell.edu/ahRULA.html">https://ergo.human.cornell.edu/ahRULA.html</a>. Accessed 23 Mar. 2026.</p>
<p>5. Liu, Houping. "Oviposition Substrate Selection, Egg Mass Characteristics, Host Preference, and Life History of the Spotted Lanternfly (Hemiptera: Fulgoridae) in North America." <em>Environmental Entomology</em>, vol. 48, no. 6, Dec. 2019, pp. 1452–1468. <a href="https://doi.org/10.1093/ee/nvz123">https://doi.org/10.1093/ee/nvz123</a></p>
<p>6. Perna, F. M., Coa, K., Troiano, R. P., Lawman, H. G., Wang, C. Y., Li, Y., Moser, R. P., Ciccolo, J. T., Comstock, B. A., Kraemer, W. J. "Muscular Grip Strength Estimates of the U.S. Population from the National Health and Nutrition Examination Survey 2011–2012." <em>J Strength Cond Res</em>, vol. 30, no. 3, Mar. 2016, pp. 867–874. <a href="https://doi.org/10.1519/JSC.0000000000001104">https://doi.org/10.1519/JSC.0000000000001104</a></p>
<p>7. Selvi, K. Ç., Kabaş, Ö., Karataş, M. "Force Requirements of Different Manual Pruning Shears When Cutting Abelia (Abelia Grandiflora) Branches." 7th TAE, 17–20 September 2019, Prague, Czech Republic. <a href="https://2019.tae-conference.cz/proceeding/TAE2019-085-Kemal-Ca%C4%9Fatay-Selvi.pdf">Conference Proceedings</a></p>
</div>
