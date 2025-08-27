---
draft: true
description:
socialDescription:
title: Appendix A 100+ PCB Design Guidelines to Minimize Signal Integrity Problems
tags:
  - highlight/articles
date: 2025-06-21
modified: 2025-08-21
---
author: [[Eric Bogatin]]
url: https://www.theeecosystem.com/_files/ugd/3fb2d5_2213fc9ec8e442aabca5eb9a5900af77.pdf
last highlighted date: [[2025-06#17]]

[[PCB Design Notes]] [[Signal Integrity]]
## Highlights
- Never use a rise time shorter than you need to, consistent with meeting timing budgets.
- If different voltage planes are used as signal references, there should be tight coupling between the different voltage planes by keeping as thin a dielectric thickness between the layers as you can afford.
- Terminate both ends of the bus in a multi-drop buss.
    - Note: what does it mean?
- For data rates above about 2 Gbps, only point to point routing will work.
- Keep the TD of stubs less than 20% the rise time of the fastest signals.
- Place the series terminating resistors as close to the package pads as possible.
- Don’t worry about corners unless 10 fF of capacitance is important.
    - Note: :)
- Route signal traces around return path discontinuities rather than across them.
- When rise times are less than 150 psec, do everything possible to minimize the loop inductance of the terminating SMT resistors, or consider using integrated or embedded resistors
- Vias generally look capacitive. Minimizing the capture pads and increasing the antipad clearance diameter will help make the via look transparent.
- If the spacing between the traces in a differential pair has to change, adjust the line width to keep a constant differential impedance.
- It is ok to change the coupling in a differential pair as long as the differential impedance is maintained.
- In general, route differential pair traces with as tight a coupling as practical for highest interconnect density and lowest cost.
- Broadside coupled differential pairs are rarely better than edge coupled. To use broadside coupled, you need a very compelling reason.
    - Note: broadside means route in different layers. Example L2, L3 signals with L1 L4 reference
- If losses are important, do everything possible to minimize all capacitive discontinuities.
- If losses are important, engineer the signal vias to look like 100 Ohms differential impedance, which usually means do everything possible to decrease the barrel size, decrease the capture pad size and increase the antipad clearance holes.
- If losses are important, use as low a dissipation factor laminate as you can afford.
- If you have to cross a gap in the return path, only use differential pairs. Never cross a gap with single ended signals routed close together.
- For surface traces, keep the coupled lengths as short as possible and use as much solder mask as practical to minimize far end cross talk.
- Use the lowest dielectric constant laminate you can afford so the dielectric spacing to the return planes can be kept to a minimum for the same target characteristic impedance.
- Guard traces can often make cross talk larger in surface traces unless the traces are very short.
- If you do use a guard trace in stripline, make it as wide as will fit and use vias to short it to the return path and spaced at least 3 vias per rise time.
- All no-connect leads or pins should be assigned as ground return connections
- If a signal changes reference planes, the reference planes should be as closely spaces as you can afford. If you use a decoupling capacitor to minimize the impedance of the return path, its capacitance value is immaterial. Select it and design it in for lowest loop inductance.
- Allocate power and ground planes on adjacent layers with as thin a dielectric as you can afford.
- Get the lowest impedance between the planes by using as high a dielectric constant between the planes as you can afford consistent with the thinnest dielectric possible.
- Route the same currents far apart and opposite currents close together
    - Note: interesting
- Route the power and ground planes as close as possible to the surface where the decoupling capacitors are mounted.
- Use multiple vias to the same power or ground pad but keep the vias as far apart as possible.
    - Note: interesting
- Place as much decoupling capacitance as you can afford on the chip itself.
    - Note: so not 100n
- Keep all traces at least 5 line widths from the edge of the board
- Place the highest speed/highest current components as far from the I/O connections as possible.
- Know the resonant frequency of all packages and change the package geometry if there is an overlap with a clock harmonic.
    - Note: good!
- Never use a pigtail connection between the cable shield and the chassis.
- Keep apertures small diameter, significantly smaller than a wavelength of the lowest frequency radiation that might leak. More smaller holes are better than fewer large holes.
