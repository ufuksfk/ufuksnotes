---
draft: true
description:
socialDescription:
title: Capacitance vs. Frequency Graph of ceramic capacitors
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[Electrical Engineering Stack Exchange]]
url: https://electronics.stackexchange.com/questions/327975/capacitance-vs-frequency-graph-of-ceramic-capacitors
last highlighted date: [[2025-05#02]]
[[Capacitor]]
## Highlights
- Every component has inductance (Equivalent Series Inductance or ESL), the value is determined by the area of the loop the current has to go through. It includes the mounting inductance on the PCB, vias, traces, etc. An example:
- ![enter image description here](https://i.sstatic.net/Zzp1Z.jpg)
- [![enter image description here](https://i.sstatic.net/zmMpK.gif)](https://i.sstatic.net/zmMpK.gif)
  The low-frequency part shows the expected 1jωC1jωC \frac{1}{j\omega C} . At high frequency, jωLjωL j\omega L dominates. Since they're all the same dimension, they all have the same HF impedance.
- smaller packages have lower ESL:
- ![enter image description here](https://i.sstatic.net/c1AvP.gif)
- So, the reason why you often see 10nF // 100nF is not that the 10nF cap is "faster", rather it is that you can get it in 0201 package, thus it has lower inductance. If both caps are 0805, then the 10nF is useless, and a single 1µF would work better.
- Parallelling low-ESR MLCCs of different values can get nasty. This is why for the simple stuff (like a logic gate or a micro) don't bother with 10n//100n, it will actually be worse. One single value is less risky, 100n or 1µ. Also power traces are inductive, that's another LC tank, ferrites ring with caps too... spice helps!