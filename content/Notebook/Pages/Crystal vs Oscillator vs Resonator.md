---
draft: false
description:
socialDescription:
title: Crystal vs Oscillator vs Resonator
tags:
  - note/versus
  - note/electrical
date: 2025-05-18
modified: 2025-09-05
---

[[Quartz Crystal]]: When you need high precision, low jitter, or very stable clock (e.g. USB, radio, precision timers).
[[Crystal oscillator]]:  “Plug & play” clock source: no need to design an oscillator circuit or add caps. Ideal for microcontrollers, FPGAs, comms modules.
[[Ceramic resonator]]:  Low‑cost, moderate‑precision clocks (e.g. general‑purpose microcontrollers where ±1 % is acceptable).


|Feature|Quartz Crystal|Crystal Oscillator|Ceramic Resonator|
|---|---|---|---|
|Pins|2|3–4|3|
|External components|Two load caps + amplifier|None|External inverter only (caps built‑in)|
|Frequency tolerance|±10–30 ppm|±50–100 ppm|±0.5 %|
|Temperature stability|Excellent|Good|Fair|
|Aging|< 5 ppm/yr|< 10 ppm/yr|~10 ppm/yr|
|Cost|Low|Higher|Lowest|
|Typical jitter|Very low|Low–medium|Medium–high|
|Ease of use|Needs oscillator design|Drop‑in clock|Needs simple inverter|