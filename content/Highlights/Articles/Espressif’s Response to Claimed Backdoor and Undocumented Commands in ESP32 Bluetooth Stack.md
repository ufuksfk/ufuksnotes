---
draft: true
description:
socialDescription:
title: Espressif’s Response to Claimed Backdoor and Undocumented Commands in ESP32 Bluetooth Stack
tags:
  - highlight/articles
date: 2025-03-13
modified: 2025-08-21
---
[[Espressif]]
url: https://www.espressif.com/en/news/Response_ESP32_Bluetooth
last highlighted date: [[2025-03#12]]
published date: [[2025-03#10]]

[[Bluetooth]]
## Highlights
- Recently, some media have reported on a press release initially calling out ESP32 chips for having a “backdoor”. Espressif would like to take this opportunity to clarify this matter for our users and partners.
- The functionality found are debug commands included for testing purposes. These debug commands are part of Espressif’s implementation of the HCI (Host Controller Interface) protocol used in Bluetooth technology. This protocol is used internally in a product to communicate between Bluetooth layers.
- **Internal Debug Commands:** These commands are meant for use by developers and are not accessible remotely. Having such private commands is not an uncommon practice.
- **No Remote Access:** They cannot be triggered by Bluetooth, radio signals, or over the Internet, meaning they do not pose a risk of remote compromise of ESP32 devices.
- **Security Impact:** While these debug commands exist, they cannot, by themselves, pose a security risk to ESP32 chips. Espressif will still provide a software fix to remove these undocumented commands.
- **Scope:** If ESP32 is used in a standalone application and not connected to a host chip that runs a BLE host, the aforementioned HCI commands are not exposed and there is no security threat
- **Affected Chipsets:** These commands are present in the ESP32 chips only and are not present in any of the ESP32-C, ESP32-S, and ESP32-H series of chips.
