---
draft: false
description:
socialDescription:
title: Crystal oscillator
tags:
  - wiki/component
  - wiki/electrical
date: 2025-05-18
modified: 2025-09-05
---
- **What it is**  
    A self‑contained 3‑ or 4‑pin package that **integrates** a quartz crystal **and** the oscillator circuitry (inverter, buffers, level‑shift).
- **Function**  
    Simply apply power (VCC & GND) and you get a buffered square‑wave (TTL/CMOS/CMOS‑LV) out.
- **Key specs**
    - **Frequency tolerance**: often ±50–100 ppm
    - **Stability**: a little worse than a bare crystal (e.g. ±100 ppm over temperature)
    - **Startup time**: specified (e.g. < 1 ms to valid clock)

from STM32 Crystal Guideline
![[Pasted image 20250501191449.png]]it can reduce drive strength of crystal. If you overdrive crystal, you will get harmonic and it can influence timing accuracy of the device. 
