---
draft: true
description:
socialDescription:
title: X7R, X5R, C0G… A Concise Guide to Ceramic Capacitor Types
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
url: https://www.allaboutcircuits.com/technical-articles/x7r-x5r-c0g...-a-concise-guide-to-ceramic-capacitor-types/
last highlighted date: [[2025-04#23]]

[[MLCC capacitor]]
## Highlights
- If you search [[DigiKey]] for a 0.1 µF 0805 ceramic cap, why are there over 400 results for X7R and zero for C0G (aka NP0)?
- The three-character code with the letter-number-letter format is used for [capacitors](https://eepower.com/textbook/vol-i-foundations-power-design/chapter-2-analysis-ac-systems/capacitors-and-inductors) with Class 2 and Class 3 dielectrics. C0G is a Class 1 dielectric, so it’s not included (more on this later). X5R and X7R are in Class 2, and Y5V is in Class 3.
- ![](https://www.allaboutcircuits.com/uploads/articles/TB_captypes_1.JPG)
- C0G is a Class 1 dielectric and an all-around capacitor superstar: the capacitance is not significantly affected by temperature, applied voltage, or aging.
- It does, however, have one disadvantage that has become particularly relevant in this age of relentless miniaturization: it is not efficient with respect to volume. For example, if you go to an electronics distributor's website and search for a 0.1 µF C0G cap, the smallest in-stock part is a 1206. In contrast, you can find a 0.1 µF X7R cap in the 0306 package (illustrated in Figure 2), and with a voltage rating (10 V) high enough for 3.3 V or even 5 V circuitry.
- If you design audio devices, or if you simply prefer quiet PCBs, you have another reason to choose C0G over X7R or X5R: Class 2 caps exhibit piezoelectric behavior that can cause them to function as both microphones (that will convert sound into electrical noise) and buzzers (that will convert AC signals into audible noise). Class 1 capacitors don’t have this problem.
