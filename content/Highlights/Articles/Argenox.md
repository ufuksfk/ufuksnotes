---
draft: true
description:
socialDescription:
title: Argenox
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[argenox.com]]
url: https://www.argenox.com/blog/battle-bluetooth-le-stacks/

last highlighted date: [[2024-01#22]]

## Highlights
- Some vendors can differentiate with their stack, for example Nordic can support up to 20 links whereas most manufacturers support up to 8 or less, but at the end of the day most manufacturers have similar features. This is where the landscape has changed. Over the last 1-2 years, open source options have come in.
- ARM mbed is, from our testing, less suitable for products as it is for educational and other purposes. So, we'll focus on Mynewt and Zephyr
- In the case of a Bluetooth stack, this can be slightly more complicated from a certification perspective. A stack must be certified by the Bluetooth SIG and given a QDID, a unique number that identifies it. This QDID is then used when an end device is declared by anyone that uses the stack and build a product. Changes to the Bluetooth Stack itself will invalidate the QDID and require re-certification.
