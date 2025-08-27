---
draft: true
description:
socialDescription:
title: The Best Stack-Up Possible With a Four-Layer PCB
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Electrical Engineering Stack Exchange]]
url: https://electronics.stackexchange.com/questions/41470/the-best-stack-up-possible-with-a-four-layer-pcb

last highlighted date: [[2023-02#03]]

## Highlights
- Sig-GND-PWR-Sig will work just fine in many applications. However, I would not recommend it as a default choice.
  What I personally use as default stack-up is this one:
  1. Sig + Routed and/or Poured Power
  2. GND
  3. GND
  4. Sig + Routed and/or Poured Power
  I'm assuming a standard build-up with relatively thin prepregs under the outer layers and a relatively thick core between the inner layers (which would also be the preferred build-up for Sig-GND-PWR-Sig by the way).
  Some aspects about this stack-up:
  • In many cases, circuits on a four-layer PCB will not have very demanding requirements for the power distribution network (PDN). So chances are you don't need a dedicated power plane.
  • Every single trace (Signal and Power) has a close-by reference plane, which reduces cross-talk and radiation (less spreading of fields).
  • Since both reference planes are on the same DC potential, you can place return vias next to signal vias providing a reasonably well defined return path even when changing layers (again, less field spreading).
  • Traces are accessible for debugging/rework.
  • It is missing the "Faraday cage" shielding feature of GND-Sig-Sig-GND. But traces over close-by reference planes are already very bad antennas. The additional shielding of GND-Sig-Sig-GND should be negligible in many applications.
  Of course, GND-Sig-Sig-GND is still one of the better four-layer stack-ups.
  Depending on the application, many stack-ups will work just fine. There simply isn't a "best" or "worst" stack-up. But there are certainly stack-ups that are "better" to default to. At the very least it doesn't hurt to be aware of the different up- and downsides of different configurations.
  Regarding one of your questions:
  > Multiple ground planes lower the ground (reference plane) impedance of the board and reduce the common-mode radiation. (I don't really understand this one.)
  I guess, this is about **cable** radiation. Multiple ground planes lower the impedance (inductance) and thus lower voltage noise on the planes. That voltage noise can couple onto cables that are attached to your board an cause common-mode currents on these cables. Common-mode currents on cables are a major source for radiated emission failures.
    - Note: good explanation about 4 layer stackup
- Sig-GND-PWR-Sig will work just fine in many applications. However, I would not recommend it as a default choice.
  What I personally use as default stack-up is this one:
  1. Sig + Routed and/or Poured Power
  2. GND
  3. GND
  4. Sig + Routed and/or Poured Power
  I'm assuming a standard build-up with relatively thin prepregs under the outer layers and a relatively thick core between the inner layers (which would also be the preferred build-up for Sig-GND-PWR-Sig by the way).
  Some aspects about this stack-up:
  • In many cases, circuits on a four-layer PCB will not have very demanding requirements for the power distribution network (PDN). So chances are you don't need a dedicated power plane.
  • Every single trace (Signal and Power) has a close-by reference plane, which reduces cross-talk and radiation (less spreading of fields).
  • Since both reference planes are on the same DC potential, you can place return vias next to signal vias providing a reasonably well defined return path even when changing layers (again, less field spreading).
  • Traces are accessible for debugging/rework.
  • It is missing the "Faraday cage" shielding feature of GND-Sig-Sig-GND. But traces over close-by reference planes are already very bad antennas. The additional shielding of GND-Sig-Sig-GND should be negligible in many applications.
  Of course, GND-Sig-Sig-GND is still one of the better four-layer stack-ups.
  Depending on the application, many stack-ups will work just fine. There simply isn't a "best" or "worst" stack-up. But there are certainly stack-ups that are "better" to default to. At the very least it doesn't hurt to be aware of the different up- and downsides of different configurations.
  Regarding one of your questions:
  > Multiple ground planes lower the ground (reference plane) impedance of the board and reduce the common-mode radiation. (I don't really understand this one.)
  I guess, this is about **cable** radiation. Multiple ground planes lower the impedance (inductance) and thus lower voltage noise on the planes. That voltage noise can couple onto cables that are attached to your board an cause common-mode currents on these cables. Common-mode currents on cables are a major source for radiated emission failures.
    - Note: good explanation about 4 layer stackup
- Sig/gnd/pwr/sig stackup has two problems: smallest of which is that by using this stackup, pwr's return path is very far away.
