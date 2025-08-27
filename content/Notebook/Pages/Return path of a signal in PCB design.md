---
draft: true
description:
socialDescription:
title: Return path of a signal in PCB design
tags:
  - note/electrical
date: 2025-05-18
modified: 2025-08-21
---
- [ ] https://www.youtube.com/watch?v=9A7LtxiP6fk
- [ ] https://www.youtube.com/watch?v=cAh4RyQHjOo
- [ ] https://www.youtube.com/watch?v=icRzEZF3eZo

- **High-speed digital signals**:  
    Return currents **follow the signal path tightly**, hugging the **lowest-impedance path**, which is usually the **directly adjacent ground plane under the trace** (due to mutual inductance).
- **Low-frequency analog signals**:  
    Return currents **don’t follow the signal trace directly**. They **spread out**, and their path is influenced by **impedance**, **loop area**, and nearby **capacitive/inductive elements**. You can’t always assume a narrow, clean return like in digital signals.
🔧 **Rule of thumb for analog**: Keep **return paths short and direct to the source**. Avoid creating **large loop areas**, which makes the system susceptible to noise pickup.