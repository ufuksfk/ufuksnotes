---
draft: true
description:
socialDescription:
title: Microsoft Word - AN1025 Clock Termination & Design Guidelines.DOC
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[dpoole]]
url: https://www.ctscorp.com/wp-content/uploads/2015/10/AN1025.pdf

last highlighted date: [[2024-09#20]]

## Highlights
- In general, most clock sources have low impedance outputs.
- The value of R can be larger than the impedance difference in order to create a slightly over damped
  condition and still eliminate reflections from the clock source.
- The major draw back for a Series termination is:
   Increases rise and fall times of the signal at the load; this may not be acceptable in some high-
  speed applications
   Not able to drive multiple loads
    - Tags: [[advice]] [[clock]] [[electronics]] 
    - Note: it is important
- Employing good design practices during the printed circuit board layout process will minimize the signal
  degradations previously discussed. Some common guidelines for PCB designs are:
   Physically locate the clock source as close to the load as possible
   Limit trace lengths for clock signals
   Do not route clock signals close to the board edge
   Try to avoid using vias in clock signal routings. Vias change the trace impedance causing
  reflection.
   Do not route signal traces on the power and ground layer
