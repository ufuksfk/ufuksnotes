---
draft: true
description:
socialDescription:
title: How to Find Low ESR and ESL Capacitors in a Catalogue
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[Electrical Engineering Stack Exchange]]
url: https://electronics.stackexchange.com/questions/672014/how-to-find-low-esr-and-esl-capacitors-in-a-catalogue/672097#672097
last highlighted date: [[2025-05#02]]

[[Capacitor]]
## Highlights
- For example the "reverse geometry" caps with the contacts on the long end have lower inductance because of the shape. But that won't reduce the inductance of your vias, and it's the same as putting two smaller "normal" caps next to each other while being more expensive.
- If the cap that has half the inductance (mounted) is three times as expensive as the jellybean cap, just put two jellybean caps in parallel.
- Below is how we think about this in 100G to 200G bypass applications.
  The most important factors will probably be capacitor placement, PCB stackup, and ground routing. I see much less difference from one capacitor to another.
- As a reference, I characterized 0.1uF capacitors to 80-110GHz and saw very little difference between a dozen randomly selected 0.1uF parts from Digikey, even when compared to very high dollar boutique capacitors.
- 0201 was much better than 0402, which was better than 0603, etc. Smaller case size was almost 100% guaranteed to be better than larger, regardless of what cap you pick.
- PCB stackup and capacitor placement are the dominant factors.
- Also, many ASIC/FPGA vendor app notes use antiquated rules of thumb which don’t hold (e.g. the 3 capacitor myth).
- I’d highly recommend watching videos by [[Eric Bogatin]] and [[Rick Hartley]] to get some really good illustrations and explanations of how to handle bypassing.