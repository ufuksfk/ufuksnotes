---
draft: true
description:
socialDescription:
title: Ground level difference between isolated grounds
tags:
  - note/electrical
date: 2025-05-18
modified: 2025-08-21
---
When you have **two isolated ground domains**, any **potential difference** (even small) between them can lead to:
- **Noise coupling**
- **Leakage currents**
- **EMI issues**
- Even **regulatory test failures** (especially for medical safety and EMC)

Techniques to minimize ground level difference:
1. Use a Common-choke or capacitive bridge (Y-caps)
	1. Add Y-caps (safety-rated, typically 1-10nF) between the 2 grounds
	2. They dont break isolation but help equalize AC potential. i.e. High freq common mode noise
	3. [[IEC 60601]] allows this within leakage current limits
2. Connect via high resistance resistor
	1. Not a typical application in medtech
	2. Only use if isolation isn't safety critical
3. Keep isolation barrier compact and controlled
	1. Minimize parasitic caps between planes by reducing overlapping copper areas and avoiding long parallel traces between domains
4. Using an isolated DC/DC Power modules
	1. Make sure both domains are powered by properly isolated supplies with low parasitic coupling
	2. Use modules with high common-mode rejection
5. Proper layout practices
	1. Keep return currents local within each domain
	2. Use creepage and clearance distance to standards
	3. avoid mixed vias or signal traces crossing isolation barrier.