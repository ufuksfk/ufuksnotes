---
draft: true
description:
socialDescription:
title: The STPMIC1 PCB Layout Guidelines - Application Note
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[STMicroelectronics]]
url: https://www.st.com/resource/en/application_note/an5431-the-stpmic1-pcb-layout-guidlines-stmicroelectronics.pdf
last highlighted date: [[2025-05#01]]
[[(PMIC) Power Management IC]]

## Highlights
- General recommendations• Always consider and determine where and how the return currents flow• As in all switching DC/DC converter configurations, the minimum length of critical traces is a key-factor aswell as the use of ground and power planes• Reduce the use of vias along the critical current paths• Route analog signals in the analog section of the board only• Do not route analog signals (voltage feedback signal) over ground plane gaps• In case ground or power plane must be split (mechanical and or electrical reasons), do not place any traceacross the gap on an adjacent layer• Never underestimate the importance of decoupling capacitors. Decoupling is the process of placing acapacitor as close as possible to the STPMIC1 to provide the transient switching current. In a DC/DCconverter, it is the process of placing an L-C network near the STPMIC1 to minimize the trace inductancescausing overvoltage spikes. If they exceed the value of AMR, the device may be damaged• A high capacity value of the decoupling capacitors is important for low-frequency decoupling effectiveness,but it is less important at high frequencies, where the most important rule is to reduce the stray inductance inseries with the decoupling capacitors
    - Note: good reccomendatios for pmic layout
- All passive components should be placed as close as possible to the STPMIC1 pins, but when this devicepacks many regulators in a small area, this can be difficult. A criterion for the passive componentsplacement is to manage their distance from the STPMIC1 by following these priorities, the highest being theshortest distance:1. Input capacitors of each Buck converter and output capacitor of the Boost converter2. Input capacitors for each LDO and device power supply (VIN, INTLDO...)3. Inductors for each DC/DC converter4. Output capacitors of each Buck converter and input capacitor of the Boost converter5. Output capacitors for each LDO regulators
