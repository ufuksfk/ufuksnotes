---
draft: true
description:
socialDescription:
title: PCB Design Notes
tags:
  - note/electrical
date: 2025-05-18
modified: 2025-08-21
---
* Don't split ground planes, If you really don't know what you are doing. You are most likely to route a signal between 2 section, and you will create more problem than you solve. [[Proper grounding at PCB Design]]
* Return path of analog signal is tricky. For fast digital signals, ,we have very short rise time and generally return path is just under the signal path. But for low freq analog signal, inductance and capacitance of return path is complicated. Rule of thumb is analog signals return to the source with shortest path.[[Return path of a signal in PCB design]]