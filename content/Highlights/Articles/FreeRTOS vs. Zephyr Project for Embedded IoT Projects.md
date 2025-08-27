---
draft: true
description:
socialDescription:
title: FreeRTOS vs. Zephyr Project for Embedded IoT Projects
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Oleksandr Zozulia]]
url: https://lembergsolutions.com/blog/freertos-vs-zephyr-project-embedded-iot-projects

last highlighted date: [[2024-01#22]]

## Highlights
- According to Aspencore market research, 65% of IoT projects use a RTOS.
- The FreeRTOS scheduler runs on the combination of two algorithms — the Prioritized Preemptive and the Time Slicing Scheduling algorithm – and manages Tasks and Co-routines concurrently. However, you can choose only one of them in the configuration file. For communication and synchronization of the tasks, FreeRTOS supports semaphores (both binary and counting), queues, and mutexes (direct and recursive). This OS can also use separated event flags and event groups. For FreeRTOS tasks, there are five ready-made heap implementations, such as heap_1, heap_2, heap_3, heap_4, and heap_5, with the fourth being used the most.
- The second RTOS we will explore in this article, Zephyr Project, was originally developed for the Virtuoso RTOS, which was intended for DSP processors. In 2016, this RTOS was named Zephyr, and development continued in collaboration with the entire Linux Foundation. In 2022, Zephyr OS became the largest open-source RTOS project by the number of commits and developers.
- Zephyr RTOS is an extremely flexible system with a tiny core primarily designed to ensure energy efficiency, which corresponds to its development concept.
- Its core is tickless by default, meaning that Zephyr software is an event-driven system. However, you can change this since this OS is highly configurable.
- Event-driven means that the scheduler will be called not just once in a certain period of time (like in FreeRTOS), but only for specific events that change the state of the thread (also known as "tasks"), which are referred to as rescheduling points.
- As for the scheduler itself, it supports all well-known flow scheduling algorithms. There are two mandatory system threads: the Main thread and the Idle thread. The kernel can create additional system threads if required by system configurations. Another of the Zephyr program’s advantages lies in its flexibility, which makes it possible to exclude multithreading in its configuration. Additionally, you can use the same semaphores, mutexes, event objects, and queues for synchronization.
- Zephyr operating system is often integrated into various SDKs, including nRF SDK, which was produced by Nordic Semiconductor with a strong Zephyr RTOS integration. This company also made significant contributions to the development of this OS.
- I like the thread analyzer the most. You can add it to the project by specifying one additional parameter to the build command in the west environment.
- Another useful feature is the GDB Stub, which enables you to control Zephyr via GDB remotely.
- I also find the west meta-utility (something like git or docker) very convenient since, in addition to git functions, it can start the build process and many more.
- I would recommend learning and using FreeRTOS if you've just started to learn the concept of RTOS. However, if you take on a task to develop a low-power solution or embedded software for a low-memory controller, or you simply want to try using something other than FreeRTOS, turn your attention to the Zephyr Project.
