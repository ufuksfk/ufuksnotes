---
draft: true
description:
socialDescription:
title: How to Pick Voltage Rating for Capacitors
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[Electrical Engineering Stack Exchange]]
url: https://electronics.stackexchange.com/questions/324643/how-to-pick-voltage-rating-for-capacitors/324776#324776
last highlighted date: [[2025-05#02]]
[[Capacitor]]

## Highlights
- Thus, a larger thicker cap (1206 vs 0603) will have thicker dielectric, a higher voltage rating, and capacitance will drop less with voltage.
  [![enter image description here](https://i.sstatic.net/k6jny.png)](https://i.sstatic.net/k6jny.png)
  This also depends on value. In a 100nF cap the dielectric will be much thicker than in a 1µF plate, so if both are the same size, the 100nF cap will show less voltage dependence.
- Depending on the dielectric, ceramic capacitors derate based on the DC voltage applied. The higher the voltage rating compared to the applied DC voltage, the less they derate. So you will have more effective capacitance with the 20V rated part than the 6.3V rated part.
  This does not apply to (polymer) tantalums, film caps, or electrolytics.