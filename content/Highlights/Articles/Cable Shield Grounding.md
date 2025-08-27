---
draft: true
description:
socialDescription:
title: Cable Shield Grounding
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[sigcon.com]]
url: https://sigcon.com/Pubs/news/2_2.htm

last highlighted date: [[2024-06#29]]

## Highlights
- On the matter of how to ground the shields (hardwire to ground, or through a capacitor), and ground currents melting shields, I would like to offer my experience with the care and feeding of ground loops in the shield protecting low- level signals: use a resistor, not a capacitor.
- Specifically, the voltage offset between chassis (green wire) grounds rarely exceeds ten volts
- f one puts a hundred-ohm one-watt carbon resistor in series with the shield at either end, with the other end directly grounded to the chassis, the ground current will be limited to 0.1 amp, well within the abilities of the shield to carry
- Joe, I am going to disagree with your suggestion that a shield with a resistor at one end acts as an effective EMI shield. In high-speed digital applications, it doesn't.
- In high-speed digital applications, a low impedance connection between the shield and the equipment chassis *at both ends* is required in order for the shield to do its job.
- In low-speed applications involving high-impedance circuitry, where most of the near-field energy surrounding the conductors is in the electric field mode (as opposed to the magnetic field mode), shields need only be grounded at one end. In this case the shield acts as a Faraday cage surrounding the conductors, prevent the egress (or ingress) of electric fields.
- In high-speed applications involving low-impedance circuitry, most of the near-field energy surrounding the conductors is in the magnetic field mode, and for that problem, only a magnetic shield will work. That’s what the double-grounded shield provides. Grounding both ends of the shield permits high-frequency currents to circulate in the shield, which will counteract the currents flowing in the signal conductors. These counteracting currents create magnetic fields that cancel the magnetic fields emanating from the signal conductors, providing a magnetic shielding effect.
