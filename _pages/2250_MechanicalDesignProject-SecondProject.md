---
layout: default
permalink: /O5_FunctionalPrototype/
fontsize: 11pt
geometry: margin=1in
papersize: letter
pagestyle: empty
header-includes:
  - \pagenumbering{gobble}
---

# BuzzKill Jaw Bucket

**Team:** BuzzKill

**Clients:** Cornell CALS Extension / E&J Gallo Winery / National Grape

## Parts List

**Table 1: Parts List**

| Part | Specs | McMaster Code | Fabrication Details | Price [$] |
|------|-------|---------------|---------------------|-----------|
| Bucket | 215×200×168.5mm bounding box; PLA; 27 in³ inner volume | N/A | 3D printed in RPL using PLA | 20.05 |
| Jaw | 200×75×10mm bounding box; PLA; tooth at end for scraping | N/A | 3D printed in RPL using PLA | 4.40 |
| Extension Jaw Springs | Stainless Steel, 2" rest length, 0.94 lbf/in spring constant | 9065K575 | No fabrication needed | 10.76 |
| PVC Pipe | ¼" wall, chemical resistant, 1.125in OD, 3ft length | 8749K77 | Drill press holes for string routing | 43.23 |
| Handle | 152×42×180mm bounding box; PLA; trigger slides in internal rails | N/A | 3D printed in RPL using PLA | 8.85 |
| Trigger | 15×36×130mm bounding box; PLA; string tied to it for jaw actuation | N/A | 3D printed in RPL using PLA | 0.80 |
| String | 585mm length | N/A | No fabrication needed | Free |
| Shoulder Stock | 127×50×38mm bounding box; PLA; attaches via M6 bolt; padded | N/A | 3D printed in RPL using PLA | 4.60 |
| Hinge | Polycarbonate, 2.5×2.125×0.2in; four M6 bolts | 1635A24 | No fabrication needed | 6.75 |
| M6 Bolt and Nuts | Seven total: 4 @ 16mm, 3 @ 50mm | N/A | Sourced from TDS | Free |
| Handle Grip/Stock Padding | 2ft, Buna-N-Foam, 1.25" OD | 9754K643 | Cut and hot glued to pipe and shoulder stock | 3.73 |
| **Total** | | | | **103.17** |

## Design Intent and Functionality

We used the calculations and design estimates from our proof of concept and the feedback we received to refine our design and build our functional prototype.

Our bucket and jaw assembly, made out of lightweight 3D-printed plastic, is designed to hold 100 egg masses. For our first prototype, we decided to use PLA because it is cost-effective and the RPL can print it quickly. We designed the bucket to have an angled opening and curved bottom so it works at different angles. The springs attach to the inside of the bucket and jaw, and the assembly moves with the help of the hinge and string on top.

<div style="display: flex; gap: 20px; flex-wrap: wrap; margin: 1em 0;">
  <figure style="flex: 1; min-width: 200px; text-align: center;">
    <img src="/fa25-portfolio-tjc252/assets/images/bucket_closed.jpg" alt="Bucket and Jaw Side View Closed" style="max-width: 100%; height: auto;">
    <figcaption><strong>Figure 1: Bucket and Jaw Side View Closed</strong></figcaption>
  </figure>
  <figure style="flex: 1; min-width: 200px; text-align: center;">
    <img src="/fa25-portfolio-tjc252/assets/images/bucket_open.jpg" alt="Bucket and Jaw Side View Open" style="max-width: 100%; height: auto;">
    <figcaption><strong>Figure 2: Bucket and Jaw Side View Open</strong></figcaption>
  </figure>
</div>

After feedback on our mock-up prototype, we designed a 3D-printed shoulder stock attachment to the other end of the PVC pipe and attached padding to further reduce user discomfort. The handle-trigger assembly is made up of two pieces of 3D-printed plastic. The handle is slid onto and screwed in place to the PVC pipe. The string that operates the jaw is attached to the trigger, which slides along guide rails on the inside of the handle. The user squeezes the trigger to open the jaw, then releases to scrape off an egg mass.

<div style="text-align: center; margin: 1em 0;">
  <img src="/fa25-portfolio-tjc252/assets/images/full_cad.jpg" alt="Entire CAD Prototype" style="max-width: 100%; height: auto;">
  <p><em>Figure 10: Entire CAD Prototype</em></p>
</div>

## Assembly Process

After 3D printing the parts and ordering the rest from McMaster or sourcing from the Taylor Design Studio, we began assembly. Due to larger-than-expected tolerances from the RPL, we sanded down the PVC pipe diameter to fit into our component slots. We then drilled ¼" holes at the required locations to bolt components and route string. Red arrows denote functional/mechanical motion; blue arrows denote assembly steps.

<div style="text-align: center; margin: 1em 0;">
  <img src="/fa25-portfolio-tjc252/assets/images/final_prototype.jpg" alt="Final Assembled Prototype in Operating Position" style="max-width: 100%; height: auto;">
  <p><em>Figure 18: Final Assembled Prototype in Operating Position</em></p>
</div>

## Design Testing

### Test One: Bucket and Jaw Assembly
**Testing:** Scraping/hinging force and durability over 100 cycles

**Results:**

| Metric | Initial | After 100 Cycles |
|--------|---------|-----------------|
| Output force (fully open) | 12.5 N | 11.5 N |
| Jaw opening gap | 1.05 in | 1.15 in |

**Conclusion:** Opening gap increased by 0.1 in and force dropped by 1 N over 100 cycles. The springs used are too long and wear-prone; shorter, more durable springs will be selected for the next iteration.

---

### Test Two: Handle/Trigger Assembly
**Testing:** Ergonomics (RULA) and actuation force

**Results:**

| Position | RULA Score |
|----------|-----------|
| Low | 3 |
| Middle | 4 |
| High | 4 |
| **Total (time-weighted)** | **3.9** |

- Actuation force when misaligned: >40 lbf

**Conclusion:** We met our target of RULA < 5, indicating low MSD risk. The handle and trigger will be redesigned for the next iteration — the current rail system frequently jams under large squeezing forces.

---

### Test Three: Jaw-Trigger-String Connection
**Testing:** Jaw opening distance vs. egg mass size

**Results:**
- Rest length opening: 1.05 in
- Maximum trigger-actuated opening: 1.95 in
- Average SLF egg mass length: ~1.5 in (3)

**Conclusion:** The jaw opening is sufficient in theory, but the trigger cannot pull the jaw to its maximum height due to human hand range-of-motion limits. The trigger mechanism will be redesigned to amplify hand motion for the next prototype.

## Success Criteria

| Criterion | Target | Priority |
|-----------|--------|----------|
| Removal effectiveness | <10% of egg mass area remaining after one pass | High |
| Durability | Jaw force and opening within ±5% after 100 cycles | Mid |
| Clamping force | ≥10 N at jaw teeth | Low |
| Ergonomics | RULA score <5; weight <15 lbs | High |

**Exhibit-Day Demonstration:** Visitors will use the device to remove Play-Doh "egg masses" from bark, metal, or plastic surfaces and measure remaining material — directly demonstrating removal effectiveness and surface compatibility.

## References

1. Hedge, Alan. CUergo: RULA. Cornell University, https://ergo.human.cornell.edu/ahRULA.html. Accessed 23 Mar. 2026.

2. Ergonomics Plus: A Step-by-Step Guide: Rapid Upper Limb Assessment (RULA), https://ergo-plus.com/wp-content/uploads/RULA-A-Step-by-Step-Guide1.pdf. Accessed 23 Mar. 2026.

3. University of Rhode Island Biocontrol Lab. Biocontrol of Insects: Spotted Lanternfly: Identification and Life Cycle, https://web.uri.edu/biocontrol/projects/slf-identification-and-life-cycle/. Accessed 23 Mar. 2026.