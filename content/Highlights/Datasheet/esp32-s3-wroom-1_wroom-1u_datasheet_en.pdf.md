---
draft: true
description:
socialDescription:
title: esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf
tags:
  - highlight/datasheet
date: 2025-03-05
modified: 2025-08-21
---
author: [[Espressif]]
url: https://www.espressif.com/sites/default/files/documentation/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf

last highlighted date: [[2024-04#02]]

## Highlights
- Power supply voltage 3.0 3.3 3.6
    - Note: it means it can't operate directly with lipo
- RP U Internal weak pull-up resistor — 45 — kΩRP D Internal weak pull-down resistor — 45 — kΩ
    - Note: internal pull-up and pull-down
- CHIP_PU is set to low level. The chip is shut down.
    - Note: this pin is responsible for shutdown chip
