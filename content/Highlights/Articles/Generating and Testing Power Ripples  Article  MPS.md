---
draft: true
description:
socialDescription:
title: Generating and Testing Power Ripples  Article  MPS
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Monolithic Power]]
url: https://www.monolithicpower.com/generating-and-testing-power-ripples

last highlighted date: [[2023-10#19]]
[[Ripple (electrical)]]
## Highlights
- There are multiple types of power ripples, described in greater detail below.
- ### Switching Cycle Ripples
- ![[Pasted image 20250313084145.png]]
- Consider a [[Buck Converter]]. This switching device turns on and off at a certain frequency. Switch ripples are generated while the device switches, meaning these ripples are generated within the switching cycle. Typically, switching ripples range between tens of kHz to several MHz
    - Note: switching cycle ripples from switching element
- Due to the influence of parasitic inductors and capacitors in the circuit, the actual switching power supply produces high-frequency switching noise in the switching tube as the power supply switches on and off (see Figure 2). The switching noise frequency exceeds the switching frequency; the switching noise magnitude relates to the parasitic parameters and PCB layout.
    - Note: switching noise are related to parasitic parameters of the pcb
- ![[Pasted image 20250313084107.png]]
- Figure 6 shows a high-impedance 10x probe where the input impedance is 9MΩ, the input impedance inside the oscilloscope is 1MΩ, and the total input impedance is 10MΩ. For 10x probes, the signal has 10x attenuation via impedance matching, and the higher attenuation ratio reduces the signal-to-noise ratio. Because the ripple is a small signal, it is better suited a 1x probe without impedance matching because the signal is not distorted.
    - Note: to measure small signal, it is better to use 1x without impedance matching
