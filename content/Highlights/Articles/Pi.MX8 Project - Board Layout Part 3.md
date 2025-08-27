---
draft: true
description:
socialDescription:
title: Pi.MX8 Project - Board Layout Part 3
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/pimx8-project-chapter-five
last highlighted date: [[2025-06#14]]
published date: [[2024-06-21]]

## Highlights
- Next, we can route the other high-speed interfaces such as PCIe, USB, HDMI and Ethernet. These interfaces have less stringent requirements for length matching between pairs, so we don't need to devote as much space to length matching. A solid return path management and basic high-speed design approaches on these signals is still very important though placing them second on the routing priority list.
- Last but not least, we can route the remaining lower speed interfaces such as SDIO, GPIO, RGMII and other miscellaneous buses such as UART or I2C and SPI. These interfaces still operate at high edge rates, which means we still need to treat them as high-speed signals.
