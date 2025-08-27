---
draft: true
description:
socialDescription:
title: Explain Like I’m a Designer ELIC PCB and HDI Routing
tags:
  - highlight/articles
date: 2025-06-21
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/explain-im-designer-elic-pcb-and-hdi-multilayer-designing
last highlighted date: [[2025-06#18]]

[[PCB stackup]]
## Highlights
- The most complex HDI routing and stackup design style in use today is called every layer interconnect (ELIC). This routing style follows a simple idea: extend microvias throughout the entire PCB stackup so that signals can route on high density interconnects between any set of layers in the PCB
- When using ELIC on an [HDI board](https://resources.altium.com/p/how-to-pack-more-complexity-into-a-smaller-footprint-using-hdi), each layer has its own copper-filled, [laser-drilled](https://resources.altium.com/p/how-ultrafast-uv-lasers-improve-hdi-pcb-design-layouts) microvias. ELIC uses only stacked copper-filled [microvias](https://resources.altium.com/p/working-altium-designers-multilayered-routing-rules) to make connections through each layer. This allows connections to be made between any two layers in the PCB once the layers are stacked.
- ![ELIC PCB stackup microsection](https://files.resources.altium.com/sites/default/files/styles/max_width_1300/public/inline-images/elic-microsection.png?VersionId=23qQCC6RL2EBjvRDHiz7ycpxTtziVPw2&itok=3Fz55lsG)
- This particular stackup goes against the [IPC warning on microvia reliability](https://resources.altium.com/p/ipc-warning-about-microvia-reliability-high-performance-products) as we have stacked microvias spanning across the entire PCB stackup. Not all fabricators that can guarantee yield for ELIC PCBs without latent defects from reflow. Be careful when selecting a manufacturer that can provide these guarantees and be sure to implement their DFM rules to ensure your board will pass quality and acceptance criteria.
- ELIC has found a home in PCBs used for GPUs and memory cards, but newer smartphones, tablets, and wearable devices can also be designed using ELIC. These applications tend to require components with high pin count and fine pitch. These boards also tend to use 10 or more layers. Using ELIC in these applications allows designers to route the required interconnects in boards with a small footprint.
- Inner signal layers in high density, high speed designs will have multiple ground/power planes that can help shield signal layers from each other and reduce crosstalk. This aids EMC compliance by shielding excess radiation.
