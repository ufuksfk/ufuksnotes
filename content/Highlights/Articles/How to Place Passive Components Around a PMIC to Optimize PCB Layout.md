---
draft: true
description:
socialDescription:
title: How to Place Passive Components Around a PMIC to Optimize PCB Layout
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[ti.com]]
url: https://www.ti.com/document-viewer/lit/html/SSZTCC7
last highlighted date: [[2025-05#03]]
[[(PMIC) Power Management IC]]
## Highlights
- First, place the components related to the reference block after the input capacitors. Second, place the inductors for the buck converters on the same layer as the PMIC after the reference-block components. Third, place the buck-converter output capacitors after the inductor. If that’s not possible, place these components right beneath the PMIC on the bottom layer, connected with several vias per component.
