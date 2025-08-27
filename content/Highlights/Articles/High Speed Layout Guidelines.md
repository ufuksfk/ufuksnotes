---
draft: true
description:
socialDescription:
title: High Speed Layout Guidelines
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[Texas Instruments]]
url: https://www.ti.com/lit/an/scaa082a/scaa082a.pdf?ts=1749711670861&ref_url=https%253A%252F%252Fwww.google.com%252F
last highlighted date: [[2025-06#12]]

[[High Speed Signals]]
## Highlights
- For example, the harmonics of a 100-MHz clock signal are not negligible,especially the third and fifth. In this case, consideration also should be made with frequencies up to 500MHz. With the CDCE906 from Texas Instruments, the user can set different rise and fall times to reducethe amplitude of the harmonics. However, take care to ensure these times do not violate the slew ratespecifications of the driven devices.
- If the lengths of traces are in the range of the signal's wavelength, then the user has to consider theeffects of transmission lines
- Another property of a transmission line is the characteristic impedance, Z0. The microstrip in Figure 4 hasfor the given attributes a characteristic impedance Z0 = 105 Ω, and the stripline Z0 = 55 Ω. If there are anyimpedance changes in the signal chain (source – trace – vias – connectors – sink, and so forth),reflections occur. These reflections cause over- and undershoots.
- A receiver often has a high-impedance input. To avoid these over- and undershoots, the reflections mustbe reduced. Therefore, a proper termination is required. The most common termination techniques follow:• Series termination• Parallel termination• Thevenin termination• AC termination
- With a complete power plane as close as possible to the ground plane, it is possible to createcapacitive coupling between them to get low impedance at high frequencies. This reduces the amounton small decoupling capacitors at the power pins of the devices. The closer the planes, the lessimpedance is present
- Power planes should only reference their own ground plane. They should not overlap with anotherground plane. This leads to capacitive coupling between the power plane and a not-referenced groundplane. Noise can couple into the other system
- Do not connect bypass capacitors between a power plane and an unrelated ground plane. Again,noise can be coupled from one supply system into the other. This mistake can occur in the circuitdesign section
- Decoupling capacitors between the power pin and ground pin of the device ensure low AC impedance toreduce noise and to store energy. To reach low impedance over a wide frequency range, severalcapacitors must be used
- A right angle in a trace can cause more radiation. The capacitance increases in the region of the corner,and the characteristic impedance changes. This impedance change causes reflections
- The designer has to make sure that thereturn current can flow ideally underneath (beside) the signal trace. A good way to realize this is to addsome ground vias around the signal via. This is a similar structure to a coaxial line
