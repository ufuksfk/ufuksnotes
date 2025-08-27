---
draft: true
description:
socialDescription:
title: Predicting Output-Capacitor Ripple in a CCM Boost PFC Circuit
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[e2e.ti.com]]
url: https://e2e.ti.com/blogs_/b/powerhouse/posts/predicting-output-capacitor-ripple-in-a-ccm-boost-pfc-circuit

last highlighted date: [[2023-10#19]]
[[(PFC) Power Factor Correction]] [[Capacitor]]
## Highlights
- Two main considerations determine how much capacitance you will need: the required holdup time and the allowable ripple voltage.
    - Note: bulk cap selection to PFC
- Both low- and high-frequency ripple currents are not functions of the amount of capacitance. Low-frequency current is a function of the output power; it is not a function of line voltage. High-frequency ripple is greatest at low line and is a function of line, boost inductance and output power.
    - Note: low freq and high freq ripple currents of the output bulk is depending on:
