---
draft: true
description:
socialDescription:
title: Signal Noise Issues With MMC & SD Memory Cards
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
]]
url: https://ibex.tech/open-source/signal-noise-issues-with-mmc-sd-memory-cards-clocked-devices-in-general

last highlighted date: [[2023-01#24]]
[[Signal Integrity]]
## Highlights
- What happens when you send a signal with a fast rising and falling edge down a wire or PCB track, if the impedance of the gate driving the wire or track isn’t exactly the same as the one receiving the it, is it that some of the pulse bounces (literally) back to the driving gate.
- This bouncing becomes worse as the speed of signal rise and fall times increases.
- If you can’t use a power plane then at least ensure you provide good ground trace routing. Many PCB designers spend ages optimising the routing of signals on their PCB’s and largely ignore the ground routing, forgetting that the routing of ground signals is 50% of the total path a signal takes.
- The downside of this is that the pair of resistors draw current so you could instead replace the resistor to GND with a small (couple of hundred pico farad) capacitor.
- One example is ‘[[Signal Integrity Issues and Printed Circuit Board Design]]’ by Douglas Brooks.
- SD card SPI busses (and many other general signals) will generally perform well with a 100ohm track Impedance (this is what we have used in many designs). Some examples with a GND plane under the tracks:
