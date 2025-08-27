---
draft: true
description:
socialDescription:
title: Performance Evaluation of CC++, MicroPython, Rust and TinyGo Programming Languages on ESP32 Microcontroller
  on ESP32 Microcontroller
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Ignas Plauska]]
url: https://www.mdpi.com/2079-9292/12/1/143

last highlighted date: [[2024-03#26]]

## Highlights
- TinyGo-based algorithms have a very important advantage over C and other programming languages, since they always have the same execution time, i.e., their standard deviation of all execution times is zero. This is explained by the fact that TinyGo programs are deployed directly to the hardware without any operating system; therefore, nothing interferes with the execution process. This means that currently TinyGo technology is the best choice for the implementation of hard real-time systems on the ESP32 platform, where time jitter is a problem.
    - Note: TinyGo advantage in ESP32 programming: Real-time
