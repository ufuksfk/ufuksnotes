---
draft: true
description:
socialDescription:
title: Why we should add series resistor to MOSFET gate
tags:
  - note/electrical
date: 2025-05-18
modified: 2025-08-21
---
If we directly drive mosfet gate via microcontroller, it means  we are driving capacitive load via low impedance source. It is directly correlated to [[(EMC) Electromagnetic Compatibility]]
We should consider using series resistor for these reasons:
1. Limit inrush current into gate capacitance
2. Control dV/dt to control switching speed
	1. Very fast switch means overshoot/ringing, EMI issues.
3. Dampen gate ringing [[Signal Integrity]]
	1. gate drive loops contain parasitic LC, which can oscillate at high freq.