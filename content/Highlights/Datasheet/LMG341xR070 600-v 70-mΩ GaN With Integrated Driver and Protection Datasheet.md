---
draft: true
description:
socialDescription:
title: LMG341xR070 600-v 70-mΩ GaN With Integrated Driver and Protection Datasheet
tags:
  - highlight/datasheet
date: 2025-03-05
modified: 2025-08-21
---
author: [[Texas Instruments]]
url: https://www.ti.com/lit/ds/symlink/lmg3411r070.pdf

last highlighted date: [[2023-10#10]]

## Highlights
- LMG341xR070s can be paralleled directly in soft-switching applications. As for hard-switching applications, smalldecoupling inductors should be utilized to parallel the two half-bridge LMG341xR070s. This type of setupprevents current and thermal unbalances among the parallel devices due to any propagation delay and gate-source threshold voltage mismatches, and other factors.
    - Note: how to parallel with soft and hard switching
- Use a four-layer board and place the return power path on an inner layer to minimize power-loop inductance
- The power loop, comprising the two devices in the half bridge and the high-voltage bus capacitance, undergoeslarge di/dt during switching events. By minimizing the inductance of this loop, ringing and electro-magneticinterference (EMI) can be reduced, as well as reducing voltage stress on the devices.
- By using an inner layer and not the bottom layer, the vertical dimensionof the loop is reduced, thus minimizing inductance
    - Note: route over next layer to reduce total distance
- The LMG341xR070's SOURCE pin is also signal ground reference. The signal GND plane should be connectedto SOURCE with low impedance kelvin connection. In addition, the return path for the passives associated to thedriver (e.g. bypass capacitance) must be connected to the GND plane. In Figure 19, local signal GND planes arelocated on the second copper layer to act as the return for the local circuitry. The local signal GND planes areisolated from the high-current SOURCE plane except the kelvin connection at the source pin through enough lowimpedance vias.
    - Note: How to connect signal ground?
- The PCB capacitance at the switch node can be minimized by following these guidelines:• Minimize overlap between the switch-node plane and other power and ground planes• Thin the GND return path under the high-side device somewhat while still maintaining a low-inductance path• Choose high-side isolator ICs and bootstrap diodes with low capacitance• Locate the power inductor as close to the power stage as possible• Power inductors should be constructed with a single-layer winding to minimize intra-winding capacitance• If a single-layer inductor is not possible, consider placing a small inductor between the primary inductor andthe power stage to effectively shield the power stage from the additional capacitance• If a back-side heat-sink is used, restrict the switch-node copper coverage on the bottom copper layer to theminimum area necessary to extract the needed heat
    - Note: how to minimize switching node capacitance.
      there is a trade-off for heat-sink copper size. heat dissipation vs low capacitance.
