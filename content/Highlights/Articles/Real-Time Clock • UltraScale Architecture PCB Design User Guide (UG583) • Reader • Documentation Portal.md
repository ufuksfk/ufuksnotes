---
draft: true
description:
socialDescription:
title: Real-Time Clock • UltraScale Architecture PCB Design User Guide (UG583) • Reader • Documentation Portal
  \ \u2022 Reader \u2022 Documentation Portal"
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Developer Site]]
url: https://docs.xilinx.com/r/en-US/ug583-ultrascale-pcb-design/Real-Time-Clock

last highlighted date: [[2023-01#24]]

## Highlights
- SD/SDIO • A 30 Ω series resistor should be placed on the CLK, CMD, and DATA lines, as close to the MIO pins as possible. • Ensure SD signals have a total delay of less than 1.3 ns (including package delays) to ensure manual tuning can find the valid input delay. • A level shifter might be required depending on the particular voltages used on the Zynq UltraScale+ MPSoC and SD chip. • Asynchronous signals CDn and WPn have no timing relationship to CLK. • The CDn and WPn lines should both be pulled up with their own 4.7 k Ω resistors to the MIO I/O voltage. When using Micro-SD, WPn and CDn can be no connects. • A 10 k Ω pull-up resistor should be added to DAT3 on the SD card side of the level shifter. Note: An external pull-up resistor is not required if one is already present on the level shifter device. • When using the SDIO 0/1 power control signal, use an external 1 k Ω to 10 k Ω pull-down resistor to get a 1 ms reset pulse according to the SD card 3.01 specification. • For level shifters without a direction pin, the MPSoC "DIR" pin can be left floating or pulled-down with a 100 k Ω resistor. The DIR pin should not be used for any other purpose. • For level shifters with 0.4 mm pitch, an adapter can be used, such as from Aries Electronics.
