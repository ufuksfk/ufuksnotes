---
draft: false
description:
socialDescription:
title: MLCC capacitor
tags:
  - wiki/component
  - wiki/electrical
date: 2025-05-18
modified: 2025-09-05
---
types of [[Capacitor]]

very cheap, easy to manufacture
non-polarized
values range from a few pF to about 100nF
working voltage from a few volts to more than 1kV
several forms of ceramic dielectric available
widely used
good performance at high freq
sound / vibration weird act. acts like microphone
it can crack when you bend board.

it is better to use bigger footprint capacitor near to usb connector because rush current can be significantly high so that capacite in smaller size can easily crack.

If you aim is to decouple switching noise, you need to consider loop inductance first. capacitance of the cap is  not a big deal, it should be small in size and as close to pad as possible. 100nF is a legacy code from THD era.

Bigger MLCC caps can burn with fire. While smaller size quickly smokes out.
	That's why it is best practice to put 0ohm or ferrite to DCDC input. Cheap fuse. It makes life easier If you have to divide that power rail from system.

What determine voltage rating?
* **Thinner layers** → more layers in same volume → **higher capacitance**, but **lower voltage**
- **Thicker layers** → fewer layers → lower capacitance, but **higher voltage rating**

**For the same X-Y footprint (e.g., 0402, 0603)**, an MLCC with **higher voltage rating typically has greater height (Z-dimension)**.