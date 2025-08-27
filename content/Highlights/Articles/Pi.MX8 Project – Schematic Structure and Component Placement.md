---
draft: true
description:
socialDescription:
title: Pi.MX8 Project – Schematic Structure and Component Placement
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/pimx8-project-chapter-two
last highlighted date: [[2025-06#13]]
published date: [[2024-02-05]]

## Highlights
- The iMX8 SoC is divided into several parts which are placed on multiple sheets. On the top-level sheet, the large symbol in the center of the page represents the SoC
- Another limitation we should consider for component placement is the fact that certain components may be susceptible to mechanical stress. Depending on the mounting situation of a PCB inside an enclosure, certain areas of a board can experience significant mechanical stress. Typical examples of such scenarios are mounting holes or heatsinks that apply an external mounting pressure to a PCB.
- But, why is this important for the Pi.MX8 module? There are components on the module that are sensitive to external mechanical stress. These components are large ceramic capacitors.
- These capacitors can easily crack if they are subject to mechanical stress. Often the capacitors fail with a short circuit causing a catastrophic failure of the whole system. For this reason, large ceramic capacitors should not be placed close to mounting holes or V-cut board edges.
