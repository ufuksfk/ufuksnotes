---
draft: true
description:
socialDescription:
title: How to Use Class X and Class Y Safety Capacitors
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/how-use-class-x-and-class-y-safety-capacitors
last highlighted date: [[2025-04#08]]

[[Safety capacitor ( Class X, Class Y)]]
## Highlights
- These capacitors are not special or unique. Just like a decoupling capacitor, the term “safety” refers to the function and placement of the capacitor, not to a specific type of capacitor. My mission in this article is to make you an expert on the usage of these capacitors.
- In isolated power supplies, safety capacitors are placed primarily in two locations:
  • As a filtering element on the input line voltage
  • As a net connection between galvanically isolated grounds
- class X and class y capacitors are defined by their AC voltage ratings as specified in the IEC 60384-14 standard. [[IEC 60384]]
- Class [[Y capacitor]]s are used to address common-mode noise by using a common shunt point to earth. For example, when used on an AC input to a DC power supply, one Class Y capacitor is used on each of the line and neutral connections to Earth, as shown below. The same type of connection to Earth could be used after a bridge rectifier, although this is very uncommon.
- Class [[X capacitor]]s are used to filter differential-mode noise in the same way, but they are connected across line and neutral. These capacitors are also shown below.
- ![](https://lh7-us.googleusercontent.com/vObtr55ocH8_YmtA-hXjjr_pUd2hBj227C9RfYD6K3ureL0b-simEpnt1ZAtwlfVC7EIXsk5tZLbnDshi-uJiMubN58wbnKWItpOEqmxYf2JEctDBmLiqxzQVRfT3oFTKmBqbh2akEmGdjNirgtmdcw)
- ![](https://lh7-us.googleusercontent.com/_XPUj_HS4M1Dnjt-5XW0K4vbMniky81OneGf9BOY_YasYlUTp6jRyEWGLIj5TlwA4_8Xj3vUYoKWmtsWCd2-E-FK2yBLWJqobUp2tZdU4WZe7rWQ9NRxWWgAworsJ209bOk1dmLfuQ4p9slgb2gbs-4)
- Notice the location where PGND is assigned: it is after the bridge rectifier! This is very important because we are connecting two DC grounds with the 2200 pF capacitor. If we connected it to neutral, we would have high AC voltage attached to the 2200 pF capacitor, which could destroy the capacitor.
- Stop splitting ground into analog and digital planes. You will create more problems than you will solve.
- I should probably tell people to keep doing it only because they will need to hire someone like me to fix the resulting EMI problems when planes are split.
- That being said, there is a very specific instance of precision low-frequency measurements with low SNR values that sometimes works better with a split plane and a safety cap or ferrite bridging the two grounds. In that case, you can still use a capacitor or ferrite (or both) to control the return path and noise currents. ***If you don’t know how or why to do this, then don’t do it.***
