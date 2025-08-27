---
draft: true
description:
socialDescription:
title: "👻 How (Not) to Use Ferrite Beads - EMI Buster #59"
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Joost Brilman]]

last highlighted date: [[2024-10#17]]

## Highlights
- Ferrite beads are passive components, but they're often misunderstood as acting like active ones.
- Some experts advise to NEVER use them.
    - Note: ferrite
- A bead works to reduce High Frequency interference in two ways:
  1. Dissipating the unwanted HF energy to heat (R)
  2. Isolation of the HF source through a high impedance connection (L + R)
- Typical bead impedance looks like this:
- ![](https://embed.filekitcdn.com/e/k5wvNU14RgMLyBEFpeu16b/tiS1dcJJ7tfvXLGV9SLM86)
- At higher frequencies (typically around 100+ MHz), the impedance is mainly resistive, the inductive properties rapidly fade away.
- The resistive peak where ferrites perform best, depends heavily on current bias.
- That is to say, datasheet impedance curves are valid for no or very little current (often not specified at all). 
  When a DC current is applied, core saturation occurs and the resistive peak shifts to higher frequencies.
- Using ferrites to reduce 1 MHz switching harmonics of a power converter is therefore a bad idea:
  • The resistive region of ferrite beads usually peaks around 100 MHz or higher. (little attenuation in the first 80 (!) harmonics ...)
  • The resistive damping regions shifts to even higher frequencies when a DC load current is applied.
