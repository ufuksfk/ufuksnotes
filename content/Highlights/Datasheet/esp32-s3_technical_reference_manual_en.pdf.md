---
draft: true
description:
socialDescription:
title: esp32-s3_technical_reference_manual_en.pdf
tags:
  - highlight/datasheet
date: 2025-03-05
modified: 2025-08-21
---
author: [[Espressif]]
url: https://www.espressif.com/sites/default/files/documentation/esp32-s3_technical_reference_manual_en.pdf

last highlighted date: [[2024-04#03]]

## Highlights
- The Clock Glitch Detection module on ESP32-S3 monitors input clock signals from XTAL_CLK
    - Note: cybersecurity
- hetouch sensors can also be configured to be moisture tolerant, and support Water Rejection capabilities.A proximity sensing mode is also supported
    - Note: modes of touch sensors
- An additional touch sensor (T0) that does not have a channel is provided for noise detectionpurposes
- The touch sensors are controlled by a Touch Finite State Machine (Touch FSM). The Touch FSM can betriggered by software or a dedicated hardware timer to conduct a measurement (i.e., take a sample) on aparticular touch pin.
    - Note: touch fsm?
- Up to three channels can be configured with proximity mode
    - Note: up to 3?
- To determine whether a touch pin has been touched, the following touch-detection methods aresupported:– Polling of touch sensor samples via software.– Built-in hardware algorithm
    - Note: there is 2 algorithm
- Water Rejection (detect if the sensor array surface is covered in water and trigger a shut down).
    - Note: how to use it
