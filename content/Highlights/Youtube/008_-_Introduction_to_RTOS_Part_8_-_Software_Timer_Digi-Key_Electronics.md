---
draft: true
description:
socialDescription:
title: 008_-_Introduction_to_RTOS_Part_8_-_Software_Timer_Digi-Key_Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=b1f1Iex0Tso&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


![Untitled](Untitled%20977.png)

creating a task had a lot of overhead, it requires 1kb of memory for vTaskDelay

using hardware timer means no portability

solution is software timer 😀

![Untitled](Untitled%20978.png)

it creats a unique taslk Timer Service Task

![Untitled](Untitled%20979.png)

![Untitled](Untitled%20980.png)

![Untitled](Untitled%20981.png)

![Untitled](Untitled%20982.png)

![Untitled](Untitled%20983.png)