---
draft: true
description:
socialDescription:
title: Touch Sensor - ESP32-S3 - — ESP-IDF Programming Guide V5.2.1 Documentation
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[docs.espressif.com]]
url: https://docs.espressif.com/projects/esp-idf/en/stable/esp32s3/api-reference/peripherals/touch_pad.html

last highlighted date: [[2024-04#03]]
[[How to design a PCB]]
## Highlights
- The touch pad sensing process is under the control of a hardware-implemented finite-state machine (FSM) which is initiated by software or a dedicated hardware timer.
- The touch sensor records the period of time (i.e., the number of clock cycles) over a fixed charge/discharge cycles (specified by touch_pad_set_charge_discharge_times()). The count result is the raw data that read from touch_pad_read_raw_data(). After finishing one measurement, the touch sensor sleeps until the next measurement start, this interval between two measurements can be set by touch_pad_set_measurement_interval().
    - Tags: [[esp32]] 
    - Note: how esp32s3 measure touch sensor
- to sense smaller capacity changes, it is possible to narrow down the reference voltage range within which the touch pads are charged/discharged. The high and low reference voltages are set using the function touch_pad_set_voltage().
- Besides the ability to discern smaller capacity changes, a positive side effect is reduction of power consumption for low power applications. A likely negative effect is an increase in measurement noise. If the dynamic range of obtained readings is still satisfactory, then further reduction of power consumption might be done by reducing the measurement time with touch_pad_set_charge_discharge_times().
    - Note: how to reduce power consumption
