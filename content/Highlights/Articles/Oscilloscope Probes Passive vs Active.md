---
draft: true
description:
socialDescription:
title: Oscilloscope Probes Passive vs Active
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[keysight.com]]
url: https://docs.keysight.com/kkbopen/oscilloscope-probes-passive-vs-active-608540396.html
[[Oscilloscope]]
last highlighted date: [[2024-04#09]]

## Highlights
- Passive probes are great for making general purpose measurements. They have a wide dynamic range and bandwidth as high as 500 MHz when connected to the 1MOhm input of the oscilloscope. They work well if you’re working in the DC and low-frequency range. They can also be sufficient for making quick quantitative measurements, such as if a clock is running or if the source is on- simple “yes or no” questions where a high degree of accuracy isn’t required.
    - Note: passive probe
- The probe’s input impedance is a function of frequency. It stays pretty flat from DC up to a certain frequency but as frequency continues to go up, the probe’s input impedance goes down, as the capacitance of the probe starts to come into play. The more capacitance, the lower the impedance. As the frequency goes up above the crossing point of ~10kHz, this is where we can really see a difference in performance between an active and passive probe.
    - Note: active is 1pf, passive is 10pf
