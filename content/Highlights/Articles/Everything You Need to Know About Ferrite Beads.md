---
draft: true
description:
socialDescription:
title: Everything You Need to Know About Ferrite Beads
tags:
  - highlight/articles
date: 2025-05-25
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/everything-you-need-to-know-about-ferrite-beads?utm_source=youtube&utm_medium=social&utm_campaign=yt-sponsor&utm_content=altium-academy
last highlighted date: [[2025-05#11]]
published date: [[2020-04]]

[[Ferrite bead]]
## Highlights
- To add to the confusion, in the application notes of some ICs, the component vendors will recommend using ferrite beads as a means of eliminating EMI.
- The attractiveness of this component is that it has a relatively high inductance in a small form factor. Typically, these components are not specified by the amount of inductance they have, but rather by their impedance at a particular frequency.
- The frequencies involved in radiated EMI range from 30MHz to 1GHZ for most products.  When the IC attempted to draw power at high frequencies from the power supply, it was prevented from doing so by the impedance of the ferrite bead.  As a result, there were no high frequencies on the IC package to cause an EMI problem
- Notice that in Figure 4, the capacitor is called a “[[bypass capacitor]]” with quotes around it. The reason for the quotes is to call attention to the fact that this capacitor is not bypassing noise, rather it is serving as a source of high frequency charge so that the ASIC can again switch rapidly. A much better name for these capacitors is “coulomb buckets” as they are functioning as local storage devices
- At Speeding Edge, our experience has been that the use of ferrite beads has been the result of a knee- jerk reaction, a band-aid or a case of holding onto bad practices rather than doing good engineering.  As Lee Ritchey, President of Speeding Edge notes, “In the 40+ years of designing high-speed computer systems and networking products, I have never used a ferrite bead in the power lead of a device whether it is a PLL or an analog circuit—all of which have functioned to their specifications and passed appropriate EMI and ESD tests. Instead, I have determined what the ‘ripple’ requirements of a circuit are and designed the power delivery system to meet those requirements.”
