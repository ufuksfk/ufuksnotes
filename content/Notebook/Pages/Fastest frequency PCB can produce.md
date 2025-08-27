---
draft: true
description:
socialDescription:
title: Fastest frequency PCB can produce
tags:
  - note/electrical
date: 2025-05-18
modified: 2025-08-21
---
With a microcontroller operating at 160 MHz and minimal digital communication on the PCB, what could cause an EMI issue at 300 MHz, which isn't a harmonic of the core frequency? What determines the highest frequency a PCB can emit?

1. Signal rise and fall times [[High Speed Signals]]
2. PCB Layout and routing. Acts as unintended antennas
3. Impedance discontunuities [[Signal Integrity]]
4. PDN Integrity. Inadequate decoupling or [[bypass capacitor]]
5. Poor grounding, ground loops [[Proper grounding at PCB Design]]