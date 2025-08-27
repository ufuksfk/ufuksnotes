---
draft: true
description:
socialDescription:
title: esp32-s3_datasheet_en.pdf
tags:
  - highlight/datasheet
date: 2025-03-05
modified: 2025-08-21
---
author: [[Espressif]]
url: https://www.espressif.com/sites/default/files/documentation/esp32-s3_datasheet_en.pdf

last highlighted date: [[2024-04#02]]

## Highlights
- The functional block diagram of the SoC is shown below.
    - Note: first check this page
- CoreMark® score:– 1 core at 240 MHz: 613.86 CoreMark; 2.56CoreMark/MHz
    - Note: https://www.eembc.org/coremark/
- – ULP-RISC-V coprocessor– ULP-FSM coprocessor
    - Note: They are 2 ULP coprocessor?
- Cryptographic hardware acceleration:– AES-128/256 (FIPS PUB 197)– Hash (FIPS PUB 180-4)– RSA– Random Number Generator (RNG)– HMAC– Digital signature
    - Note: learn more about that part
- In Table 2-3 IO MUX and GPIO Pin Functions and Table 2-4 RTC and Analog Pin Functions some pin functions arehighlighted . The non-highlighted GPIO or RTC_GPIO pins are recommended for use first. If more pins areneeded, the highlighted GPIOs or RTC_GPIOs should be chosen carefully to avoid conflicts with important pinfunctions.
    - Note: how to choose pinout
- VDD3P3_RTC Input RTC and part of Digital power domains
    - Note: we need to use this to have RTC on while shutdown all other peripherals
- Only RTC is powered on. Wireless connection data is stored in RTC memory.
- VDD3P3_RTC 2 Recommended input voltage 3.0 3.3 3.6 V
    - Note: But RTC voltage has 3.6V absolute maximum
