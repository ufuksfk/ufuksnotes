---
draft: true
description:
socialDescription:
title: ESD Protection Basics With TVS Diodes
tags:
  - highlight/articles
date: 2025-08-05
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/esd-protection-basics-tvs-diodes
last highlighted date: [[2025-W27#30]]
published date: [[2022-W44#04]]

[[TVS diode]]
[[ESD Protection]]
## Highlights
- In this article, we will be covering the basics of [ESD protection](https://resources.altium.com/p/beginners-guide-esd-protection-circuit-design-pcbs) and TVS diodes. We will cover a few different aspects, such as why we require ESD protection, how an ideal TVS diode operates, and typical TVS diode parameters.
- Integrated circuits are typically very sensitive to electrostatic discharge as [ESD protection](https://resources.altium.com/p/workspace-esd-protection) is not usually included or if only to a small extent. This is because protections take up quite a lot of silicon real-estate. Therefore, we often need to add external ESD protection.
- In an ideal case, during normal operation and signaling, the diode will simply appear as an open circuit. It will be invisible to the connector, and invisible to the integrated circuit.
- As is the case with any diode, a TVS diode will have some capacitance associated with it. For DC or low-speed signals, any capacitance added to the line is normally not a problem. However, at high-speeds and high data-rates, extra capacitance will negatively impact the signal. Therefore, it is advisable to choose “high-speed” (low-capacitance) TVS diodes for those purposes.
- The IEC 61000-4-2 is a robustness rating of our protection device. What rating is needed is very much dependent on design, on required contact, and air discharge ratings. A higher IEC 61000-4-2 rating gives us a higher level of protection or robustness.
