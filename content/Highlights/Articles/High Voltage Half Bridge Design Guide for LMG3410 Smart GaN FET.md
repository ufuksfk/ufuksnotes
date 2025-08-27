---
draft: true
description:
socialDescription:
title: High Voltage Half Bridge Design Guide for LMG3410 Smart GaN FET
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author [[Texas Instruments]]
url: https://www.ti.com/lit/an/snoa946a/snoa946a.pdf?ts=1695718032326

last highlighted date: [[2023-09#27]]

## Highlights
- With typical slewrates around 30 V/ns to 100 V/ns at operating voltages around 380 V to 480 V, printed circuit board (PCB)layout optimization is even more essential since parasitic inductances and capacitances from poor layoutscan drastically reduce performance or even prevent operation
- The LMG3410x devices have a user-controllable slew rate from 30 V/nsto 100 V/ns. While this helps reduce the power loss during each switching transition, it also increases thevoltage and current slew rates. As Equation 1 shows, by increasing the current slew rate the voltageinduced across any parasitic inductor is increased, increasing voltage overshoot on the power device.
