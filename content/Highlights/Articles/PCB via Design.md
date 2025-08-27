---
draft: true
description:
socialDescription:
title: PCB via Design
tags:
  - highlight/articles
date: 2025-05-25
modified: 2025-08-21
---
url: https://www.protoexpress.com/kb/pcb-via-design/
last highlighted date: [[2025-05#25]]
published date: [[2021-12]]

[[Via (electronics)]]
## Highlights
- **Microvias:** According to IPC-T-50M, microvia is a blind structure with an ideal aspect ratio of 0.75:1. It is laser-drilled, with a diameter of less than 150μm. Its target length should not be more than 0.25mm measured from the capture land to the target land.
- [[Microvia]] are generally implemented in HDI PCBs. The depth of a microvia isn’t usually more than two layers since the process of copper plating, inside these vias, is a tedious task.
- ![](https://www.protoexpress.com/wp-content/uploads/2021/12/image2-3.png)
- ![](https://www.protoexpress.com/wp-content/uploads/2021/12/image3-1.png)
- Opt for [[staggerred via]] instead of stacked vias, as stacked vias need to be filled and planarized. This process is time-consuming and requires extra cost.
- Implement controlled depth for blind and buried vias.
- Keep the aspect ratio to a minimum for high-speed vias to avoid signal reflections. This provides better electrical performance and signal integrity, low noise and crosstalk, and reduced EMI/RFI.
- Use smaller vias especially in HDI boards to minimize the stray capacitance and inductance.
