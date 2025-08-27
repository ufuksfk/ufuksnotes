---
draft: true
description:
socialDescription:
title: Pi.MX8 Project - Board Layout Part 2
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/pimx8-project-chapter-four
last highlighted date: [[2025-06#14]]
published date: [[2024-03-21]]

## Highlights
- Connecting the decoupling capacitors was part of the breakout routing in the previous article. Let's review that first to see if we need to add any additional VIAs or traces on the top or bottom layer. The fact that we are using filled and capped VIAs really plays into our hands when it comes to routing the decoupling capacitors.
- The DRAM IC has a pin pitch of 0.65mm in the Y-Axis. This pin pitch allows us to place the decoupling capacitors directly between the GND and VDD/VDDQ pads. This arrangement allows for the lowest loop inductance possible. We can now evenly distribute the decoupling capacitors among the power pins.
- Coloring the command/address/control signal differently from the DQ groups helps us to identify a good routing strategy.
- Strictly speaking, we are not changing the reference layer, but we are introducing a second one by switching to L2. As soon as we place a trace with a time-varying voltage over a ground plane, a current will flow regardless of whether there is a second reference plane present. To provide a return path for those currents as well we are using return path VIAs close to the layer transitions on the top layer
