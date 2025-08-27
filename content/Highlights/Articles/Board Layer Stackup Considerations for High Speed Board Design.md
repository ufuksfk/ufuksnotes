---
draft: true
description:
socialDescription:
title: Board Layer Stackup Considerations for High Speed Board Design
tags:
  - highlight/articles
date: 2025-05-25
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/board-layer-stackup-considerations-for-high-speed-board-design
last highlighted date: [[2025-05#21]]

[[PCB stackup]]
## Highlights
- For moderate layer count boards, there are few simple guidelines that can help suppress EMI and ensure power integrity:
  • It's okay to divide up a power plane into multiple rails as long as signals are not referenced to that plane layer
  • If there are multiple power planes, do not stack the power planes on adjacent layers; separate them with a GND plane
  • Put fast signals on internal layers between two GND planes; do not reference these to power planes with any splits
  • Only use the surface layers for fast microstrips, some power routing if needed, and [some GND pour if needed](https://resources.altium.com/p/copper-pour-and-stitching-do-you-need-them-pcb-layout)
