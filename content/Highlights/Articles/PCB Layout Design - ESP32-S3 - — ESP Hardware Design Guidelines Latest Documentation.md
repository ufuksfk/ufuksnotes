---
draft: true
description:
socialDescription:
title: PCB Layout Design - ESP32-S3 - — ESP Hardware Design Guidelines Latest Documentation
  \ Documentation"
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[docs.espressif.com]]
url: https://docs.espressif.com/projects/esp-hardware-design-guidelines/en/latest/esp32s3/pcb-layout-design.html

last highlighted date: [[2024-03#13]]
about [[(PCB) Printed Circuit Board]] [[How to design a PCB]]
## Highlights
- If the PCB antenna cannot be placed outside the board, please ensure a clearance of at least 15 mm around the antenna area (no copper, routing, or components on it), and place the feed point of the antenna closest to the board
    - Note: how to cutout under antenna
- The drill diameter on other power traces should be no smaller than the width of the power traces.
- The ground pad at the bottom of the chip should be connected to the ground plane through at least nine ground vias.
- The width of the main power traces should be no less than 25 mil. The width of VDD3P3 power traces should be no less than 20 mil. The recommended width of other power traces is 10 mil.
    - Note: power traces
- The UART trace should be surrounded by ground copper and ground vias stitching.
- Make sure there is a complete reference ground plane and surround the [[USB]] traces with ground copper.
    - Note: usb trace
- The trace length for SDIO_CMD and SDIO_DATA0 ~ SDIO_DATA3 should be 3 mil longer or shorter than the trace length for SDIO_CLK. If necessary, use serpentine routing.
- It is better to surround the SDIO_CLK trace with ground copper.
- The trace width (W) can not be larger than 0.18 mm (7 mil).
- Generally, the peak-to-peak value of the ripple should be <80 mV when ESP32-S3 sends MCS7@11n packets, and <120 mV when ESP32-S3 sends 11 MHz@11b packets.
- Add a 10 μF filter capacitor to the branch of the power trace (the branch powering the chip’s analog power pin). The 10 μF capacitor should be as close to the analog power pin as possible for small and stable voltage ripples.
    - Note: The voltage ripple is not large, but the TX performance of RF is rather poor
- Good TX performance indicates proper RF impedance matching. Poor RX sensitivity may result from external coupling to the antenna. For instance, the crystal signal harmonics could couple to the antenna. If the TX and RX traces of UART cross over with RF trace, they will affect the RX performance, as well. If there are many high-frequency interference sources on the board, signal integrity should be considered.
    - Note: TX performance is not bad, but the RX sensitivity is low.
