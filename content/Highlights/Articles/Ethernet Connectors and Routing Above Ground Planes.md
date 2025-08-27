---
draft: true
description:
socialDescription:
title: Ethernet Connectors and Routing Above Ground Planes
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[signal integrity journal]]
url: https://www.signalintegrityjournal.com/articles/1808-ethernet-connectors-and-routing-above-ground-planes
last highlighted date: [[2025-06#08]]

[[Ethernet related electronics notes]]
## Highlights
- Traces between the MAC/PHY, magnetics circuit, and the RJ45 connector are routed as differential pairs with defined impedance. Note that this includes traces within a discrete magnetics circuit. The differential impedance is set to 100 Ohms to provide matching to the cable’s differential impedance. Shorter traces are generally preferred throughout, especially at higher frequencies (e.g., gigabit Ethernet and higher) to reduce losses. Everyone who works with Ethernet is pretty clear on these requirements.
- The controversy around the ground plane (or planes) starts with placement of discrete magnetics and any other components needed for termination with respect to the PHY and RJ45 connector. There are generally three possibilities:
  **Option 1:** Run the system ground up to the RJ45 connector, regardless of whether magnetics are integrated into the connector; or
  **Option 2:** Use a split ground plane, where chassis ground is placed below the RJ45 and system ground runs to the input edge of the common-mode choke; or
  **Option 3:** Place no ground plane between the magnetics input and the RJ45 connector.
- Before we look at which of these options is objectively best for routing between a PHY, magnetics, and the RJ45 connector, it helps to review the overall design goals:
  **Design Goal 1: ESD/overvoltage protection.** The 802.3 standard specifies the Ethernet PHY must be isolated from the rest of the system in order to withstand high-potential AC up to 1500 V(RMS) at 50 to 60 Hz for 60 seconds.
  **Design Goal 2: noise isolation.** Any noise picked up on the cable should be prevented from coupling back into the PHY and rest of the board.
  **Design Goal 3: common-mode noise shunt.** Common-mode noise in any ground region should be diverted away from the magnetics and PHY side through low impedance paths.
- The distance between the output of the PHY and the magnetics input should be at least 25 mm. The intention here is to provide sufficient isolation between the magnetics and the PHY, although making these lines too long leads to greater attenuation, and this attenuation is greater at higher frequencies. In both types of connectors, common-mode capacitors can also be placed on the end taps as a shunt to the system ground at the magnetics input to provide greater high frequency noise rejection.
