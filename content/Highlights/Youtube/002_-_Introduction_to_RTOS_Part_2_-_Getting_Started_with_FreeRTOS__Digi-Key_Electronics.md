---
draft: true
description:
socialDescription:
title: 002_-_Introduction_to_RTOS_Part_2_-_Getting_Started_with_FreeRTOS__Digi-Key_Electronics
  Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=JIr7Xm_riRs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


downloading freertos source code and create your own version

mcu timer to tick timer

[1:13](https://www.youtube.com/watch?v=JIr7Xm_riRs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=2&t=74s&type=snipo)
Both are amazingly helpful when navigating FreeRTOS. When it's done downloading, extract the zip file, and head into the FreeRTOS directory. The FreeRTOS library is just a scheduler, which is great if you have your own device and file drivers. The FreeRTOS Plus library is the scheduler and a few drivers, mostly for networking, like TCP and UDP. You'll want to copy or link to the source files in your build system. Take a look in the demo folder, 

![Untitled](Untitled%201029.png)

non blocking wait thanks to tick timer.

![Untitled](Untitled%201030.png)

[8:22](https://www.youtube.com/watch?v=JIr7Xm_riRs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=2&t=503s&type=snipo)
For the parameters, we need to tell it what function we want to call for our task, and give the task a name as a string. We then set the stack size in bytes. Note that this would be number of words in Vanilla FreeRTOS. According to the config file we looked at earlier, the smallest stack size we can set here is 768 bytes, which is the minimum required to run an empty task, and whatever overhead the scheduler needs.