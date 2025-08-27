---
draft: true
description:
socialDescription:
title: Antiresonance of Multiple Parallel Decoupling Capacitors Use Same Value or Multiple Values
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[Electrical Engineering Stack Exchange]]
url: https://electronics.stackexchange.com/questions/320363/antiresonance-of-multiple-parallel-decoupling-capacitors-use-same-value-or-mult
last highlighted date: [[2025-05#02]]

[[Capacitor]] [[Decoupling capacitor]]
## Highlights
- It seems sensible to place a bulk capacitor (say 10-100uF), to act as an energy reservoir, and several smaller capacitors to deal with higher frequencies. The reason to place several small capacitors instead of just one is to deal with their Equivalent Series Inductance (ESL), which in practice, causes them to behave like an LC circuit.
- Yet, here is where best design practices and electronic myth seem to get mixed up and confusing to me. Most electronic engineers I have met like placing several decoupling capacitors of different values in parallel (with the smaller capacitors closer to the IC). The logic behind it is that the each capacitor takes care of a different noise frequency as depicted in Figure 1.
  [![Figure 1: Impedance over frequency of three different value capacitors in parallel (cyan) vs their individual contribution (brown, blue, red). Image taken from https://www.allaboutcircuits.com/technical-articles/clean-power-for-every-ic-part-2-choosing-and-using-your-bypass-capacitors/](https://i.sstatic.net/5zgze.jpg)](https://i.sstatic.net/5zgze.jpg)
- However, I have read in [Electromagnetic Compatibility Engineering](https://rads.stackoverflow.com/amzn/click/com/0470189304) by [Henry W. Ott] that placing capacitors of different values may cause a much greater antiresonance-peak which can be very harmful for our designs (see Figure 2). In fact, it amplifies any noise that falls into the anti-resonance frequency range,
- ![Figure 2: from Electromagnetic Compatibility Engineering, by Henry W. Ott, section 11.4.4](https://i.sstatic.net/DHSyV.png)
- Today you can find 10uF decoupling caps in 0603 package so there is absolutely no reason to do this multiple capacitor trick.
- You're doing pretty good on getting to the parallel resonance already. It depends on your application. If you're trying to suppress/bypass for example ethernet peaks, you should use parallel caps which have impedance dips in the fundamental frequency and some of the harmonics.
- ![enter image description here](https://i.sstatic.net/IE5nC.png)