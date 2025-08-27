---
draft: true
description:
socialDescription:
title: Selecting Inductors for BUCK DCDC Regulators
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[docs.nordicsemi.com]]
url: https://docs.nordicsemi.com/bundle/nwp_050/page/WP/nwp_050/buck_inductor_selection.html
last highlighted date: [[2025-05#01]]
[[Buck Converter]] [[Inductor]] [[(PMIC) Power Management IC]]
## Highlights
- The buck regulators of nPM1300 are designed to operate with
  inductors that have a nominal inductance of 2.2 µH with ± 20% tolerance. To ensure loop stability,
  do not use inductors with other nominal inductances. 
  The saturation current of the inductor should be greater than 400 mA. This saturation current
  requirement should be respected even if the load current range required in the application during
  design is lower than the maximum load current of the buck regulator. This is because the inductor
  peak current level is higher than the load current, especially when the buck regulator operates
  in hysteretic mode.
    - Note: good example of how to choose inductor for BUCK DC/DC
