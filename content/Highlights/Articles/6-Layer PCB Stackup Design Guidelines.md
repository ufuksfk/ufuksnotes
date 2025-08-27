---
draft: true
description:
socialDescription:
title: 6-Layer PCB Stackup Design Guidelines
tags:
  - highlight/articles
date: 2025-05-25
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/6-layer-pcb-design-guidelines-pcb-design
last highlighted date: [[2025-05#21]]
published date: [[2022-05]]

[[PCB stackup]]
## Highlights
- The most basic version of a 6-layer stackup will take the same approach as a SIG/PWR/GND/SIG stackup in a 4-layer board and just puts signal on two additional in the center of a stackup. In reality, a SIG/PWR/SIG/SIG/GND/SIG is the worst 6-layer PCB stackup from an EMC perspective, and it’s probably only appropriate for a board running at DC.
- If applied to 6-layer PCBs, you would expect the following two arrangements: one where the outer layers are core and thin prepreg, and another where two thicker cores are used in the inner layers and a thin prepreg forms the very center of the 6-layer PCB stackup.
- I would argue that the 3-core version (or equivalently 1 thick central core with thin outer layers) is the superior option in most cases. There are several reasons for this:
  • It places the power rails on L3 very close to ground on L2; this increases PDN plane capacitance and reduces [spreading inductance](https://resources.altium.com/p/what-spreading-inductance)
  • It places the signal on L4 close to ground on L5 and farther from any [power rail splits on L3](https://resources.altium.com/p/should-you-route-signals-your-pcb-power-plane); this reduces chances of radiated emissions from PCB edge
  • Related to the previous point, the impedance of any signals on L4 will have smaller deviations near power rail splits on L3
- 
