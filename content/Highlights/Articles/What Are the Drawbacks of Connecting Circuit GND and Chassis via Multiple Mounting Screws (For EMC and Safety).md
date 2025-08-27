---
draft: true
description:
socialDescription:
title: What Are the Drawbacks of Connecting Circuit GND and Chassis via Multiple Mounting Screws (For EMC and Safety)
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[electronics.stackexchange.com]]
url: https://electronics.stackexchange.com/questions/609376/what-are-the-drawbacks-of-connecting-circuit-gnd-and-chassis-via-multiple-mounti
last highlighted date: [[2025-06#08]]

[[Proper grounding at PCB Design]] [[(EMC) Electromagnetic Compatibility]]
## Highlights
- **My question is what are the drawbacks of the first approach (GND = chassis) that make the second approach ever worthwile, in particular for EMC and for safety. I am not interested in potential drawbacks for *analog precision***, as I believe that both these design are not ideal in this respect and single-ended analog return currents must never share the same medium with any other return currents for highest precision.
- Although the chassis is used as a protective element it also provides an additional support for EMC. But care must be taken because a bad layout and bonding design may turn the chassis into a good antenna, especially if it has some cornered shapes and randomly placed holes. I remember that I saw a competitor's power supply when I was working in automotive, and it was working like a jammer (disturbing lots of radio channels) when it's fully loaded.
