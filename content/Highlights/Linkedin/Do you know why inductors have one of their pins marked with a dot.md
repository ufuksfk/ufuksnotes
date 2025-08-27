---
draft: true
description:
socialDescription:
title: Do you know why inductors have one of their pins marked with a dot
tags:
  - highlight/linkedin
date: 2025-07-15
modified: 2025-08-21
---
[[2025-07#15]]
https://www.linkedin.com/feed/update/urn:li:activity:7350735869571424256/
[[Inductor]]

![[Pasted image 20250715145612.png]]

The dot on the part is there for productiin reasons.  
For a (single) inductor, it should indicate the 'start' of the winding. That is, the winding that is shielded by subsequent winding and has the lowest surface area (capacitive and magnetic coupling).  
For coupled inductors and transformers, there should be only 1 dot, pin 1. The documentation should state which pins are the start of the winding. Preferably, pin 1 is (also) a start of the winding.  
Only the EE drawing the schematic knows which pin to where, including start of winding. For both the layout engineer and EMS, only pin 1 matters (IF it matters).


It start of winding. This pin indicates that it all the ret of windings physically placed above this entery point. Very important for DC/DC applications, where you connect the most noisy point to this pin, it ensures that it wiil less radiate EMI outsude.