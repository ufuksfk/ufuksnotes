---
draft: true
description:
socialDescription:
title: Power Planes as Return Reference Planes in PCB Design Challenges and Solutions in Multilayer Stackups
tags:
  - highlight/articles
date: 2025-06-25
modified: 2025-08-21
---
author: [[Dario Fresu]]
url: https://www.fresuelectronics.com/post/emc-design-for-multilayer-pcb-be-aware-of-using-power-planes-as-return-reference-planes
last highlighted date: [[2025-06#24]]

[[PCB stackup]]

## Highlights
- In this stackup, the power plane on Layer 5 is separated from the ground planes on Layers 2 and 7 by multiple signal layers and dielectric layers. This configuration is common in designs where cost or layer count constraints limit the number of ground planes or dictate plane placement. However, it amplifies the challenges of using power planes as reference planes, as the increased interplane distance reduces capacitance and increases impedance.
    - Note: Layer 1: Signal
      Layer 2: Ground
      Layer 3: Signal
      Layer 4: Signal
      Layer 5: Power
      Layer 6: Signal
      Layer 7: Ground
      Layer 8: Signal
- This stackup places power and ground planes adjacent to each other (Layers 2–3 and 6–7), maximizing interplane capacitance and minimizing impedance. A thinner dielectric (e.g., 4 mils) between these planes further increases capacitance, reducing the voltage drop caused by displacement current.
    - Note: Layer 1: Signal
      Layer 2: Ground
      Layer 3: Power
      Layer 4: Signal
      Layer 5: Signal
      Layer 6: Power
      Layer 7: Ground
      Layer 8: Signal
