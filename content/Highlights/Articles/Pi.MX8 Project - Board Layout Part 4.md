---
draft: true
description:
socialDescription:
title: Pi.MX8 Project - Board Layout Part 4
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/pimx8-project-chapter-six
last highlighted date: [[2025-06#14]]
published date: [[2024-07-23]]

## Highlights
- Looking at the layerstack we can see that we have two dedicated power plane layers available. These layers are separated from the adjacent ground layers by a thin prepreg. This stacking increases the low inductance plane capacitance and can help to decrease the PDN impedance at high frequencies.
- The final step of the power plane routing is to set up an AC and DC PDN analysis and check if the results are within the impedance value boundaries set by the hardware design guide of the SoC.
- The AC simulation must include the decoupling capacitors with an accurate equivalent model, the buck regulator output characteristics and the geometry of the layout. We won’t go over the simulation setup in this article but need to keep it in mind as a mandatory verification step.
- ![LPDDR4-4000 PCB delay tuning requirements](https://files.resources.altium.com/sites/default/files/styles/max_width_1300/public/inline-images/Image%209.png?VersionId=896j7tXBfCB.fsowA6oklwTzMvAQB7kw&itok=VjN1vfLS)
