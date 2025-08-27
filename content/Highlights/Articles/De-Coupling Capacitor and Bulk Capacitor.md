---
draft: true
description:
socialDescription:
title: De-Coupling Capacitor and Bulk Capacitor
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[Electrical Engineering Stack Exchange]]
url: https://electronics.stackexchange.com/questions/170957/de-coupling-capacitor-and-bulk-capacitor/289709#289709
last highlighted date: [[2025-05#02]]
[[Decoupling capacitor]] 
## Highlights
- There is, in a sense, no qualitative difference. The difference is one of scale, both of current and of time.
  A bulk capacitor is used to prevent the output of a supply from dropping too far during the periods when current is not available. For line-powered linear supplies, this would occur during the periods (say, 10s of msec) that the line voltage is near zero. It also applies to the circuit as a whole. That is, an electronics assembly containing multiple circuit cards might have a single set of bulk capacitors in the power supply.
  Decoupling capacitors, on the other hand, are used locally (such as 1 per logic chip in some systems) and are intended to supply current for much briefer periods (typically 10s of nsec for TTL systems) and much smaller currents. As a result, decoupling caps are typically much smaller than bulk caps.