---
draft: true
description:
socialDescription:
title: Proper grounding at PCB Design
tags:
  - note/electrical
date: 2025-05-18
modified: 2025-08-21
---
- [ ] https://www.youtube.com/watch?v=ySuUZEjARPY

## Splitting the ground
It is not reccomended for most cases.

 - If you **split digital and analog grounds**, and a signal crosses the split, the **return current has no clear path** — it loops around the split → causing **EMI and signal integrity issues**.
 - Even when splitting is done right, it requires **controlled routing**, **careful stitching capacitors or resistors**, and **a solid understanding of return current behavior**.
🛑 **Rule of thumb**: Use a **solid ground plane** unless you have specific isolation requirements (e.g., patient isolation, high-voltage isolation), and **control return paths via layout** rather than splits.