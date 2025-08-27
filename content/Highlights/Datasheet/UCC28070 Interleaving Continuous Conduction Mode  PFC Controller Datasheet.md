---
draft: true
description:
socialDescription:
title: UCC28070 Interleaving Continuous Conduction Mode  PFC Controller Datasheet
tags:
  - highlight/datasheet
date: 2025-03-05
modified: 2025-08-21
---
author: [[ti.com]]
url: https://www.ti.com/lit/ds/symlink/ucc28070.pdf

last highlighted date: [[2023-10#17]]

## Highlights
- Soft-Start and External Fault Interface. Connect a capacitor to GND on this pin to set the soft-start slew ratebased on an internally-fixed, 10-μA current source. The regulation reference voltage for VSENSE is clamped toVSS until VSS exceeds 3 V. Upon recovery from certain fault conditions, a 1-mA current source is present at theSS pin until the SS voltage equals the VSENSE voltage. Pulling the SS pin below 0.6 V immediately disablesboth GDA and GDB outputs.
    - Note: fault detection functionality
- RSYN RSYNTH resistance 15 750 kΩRRDM RDM resistance 30 330 kΩ
    - Note: Rsynth = Current syntesis down-slope programming. Connect it to VREF disables it.
      Rdm = Dither magnitude for frequency
- The UCC28070 power factor corrector IC controls two CCM (Continuous Conduction Mode) Boost PFC powerstages operating 180° out of phase with each other. This interleaving action reduces the input and output ripplecurrents so that less EMI filtering is needed and allows operation at higher power levels than a non-interleavedsolution.
    - Note: overview of UCC28070
- One of the main benefits from the 180° interleaving of phases is significant reductions in the high-frequencyripple components of both the input current and the current into the output capacitor of the PFC preregulator.Compared to that of a single-phase PFC stage of equal power, the reduced ripple on the input current eases theburden of filtering conducted-EMI noise and helps reduce the EMI filter and CIN sizes. Additionally, reduced high-frequency ripple current into the PFC output capacitor, COUT, helps to reduce its size and cost. Furthermore, withreduced ripple and average current in each phase, the boost inductor size can be smaller than in a single-phasedesign
    - Note: interleaving means smaller boost inductor, reduced emi ...
- A resistor-divider network from VREF to GND can easily program the peak current limit voltage on PKLMT,provided the total current out of VREF is less than 2 mA to avoid drooping of the 6-V VREF voltage. TIrecommends a load of less than 0.5 mA, but if the resistance on PKLMT is very high, TI recommends a smallfilter capacitor on PKLMT to avoid operational problems in high-noise environments.
    - Note: Peak current limitation with PKLMT
- Detailed Design Procedure
    - Note: how to design components step by step. There is also a calculation excel for it.
      https://www.ti.com/tool/download/SLUC114
- The bridge rectifier must be rated to carry the full line current. The voltage rating of the bridge should be at least600 V. The bridge rectifier also carries the full inrush current as the bulk capacitor COUT charges when line isconnected.
    - Note: bridge rectifier selection
- Current Loop Feedback Configuration(Sizing of the Current Transformer Turns Ratio and Sense Resistor (RS)
    - Note: how to arrange current sense circuit
- Similar to other power management devices, whenlaying out the PCB it is important to use star grounding techniques and to keep filter and high frequency bypasscapacitors as close to device pins and ground as possible. To minimize the possibility of interference caused bymagnetic coupling from the boost inductor, the device should be located at least 1 inch away from the boostinductor. TI recommends the device not be placed underneath magnetic elements [[How to design a PCB]]
    - Note: layout guidelines

last highlighted date: [[2024-09#20]]
## Highlights
- The UCC28070 power factor corrector IC controls two CCM (Continuous Conduction Mode) Boost PFC power
  stages operating 180° out of phase with each other. This interleaving action reduces the input and output ripple
  currents so that less EMI filtering is needed and allows operation at higher power levels than a non-interleaved
  solution.
- the boost inductor size can be smaller than in a single-phase
  design