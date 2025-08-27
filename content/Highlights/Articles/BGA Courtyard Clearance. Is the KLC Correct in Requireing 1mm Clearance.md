---
draft: true
description:
socialDescription:
title: BGA Courtyard Clearance. Is the KLC Correct in Requireing 1mm Clearance
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[forum.kicad.info]]
url: https://forum.kicad.info/t/bga-courtyard-clearance-is-the-klc-correct-in-requireing-1mm-clearance/9544
last highlighted date: [[2025-06#11]]

[[BGA design notes]]
## Highlights
- Currently the KLC requires a clearance of 1mm around BGA devices. As i don’t have access to industry standards, i can’t check where this requirement comes from. Does it apply to all BGA devices regardless of size? (1mm clearance for a 0.8x1.1mm device is quite a lot.)
- With a small ball size, the placement courtyard can be smaller as less heat is then required to unsolder the BGA component for rework. However, the end user may not plan to rework the BGA if it fails. In that case, there is no need to have a robust placement courtyard, but a recommended minimum placement courtyard excess is 0.5 mm.
- ![](https://kicad-info.s3.dualstack.us-west-2.amazonaws.com/original/3X/c/0/c07c4eef6654355c3764afb29356d6f54134dfcf.png)
