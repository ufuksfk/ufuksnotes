---
draft: true
description:
socialDescription:
title: WHY_IS_THE_STACK_SO_FAST
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=N3o5yHYLviQ&type=snipo

[[Core Dumped]]


Created time: [[2024-05#18]]

### [0:00 Introduction](https://www.youtube.com/watch?v=N3o5yHYLviQ&type=snipo&t=0s)

### [0:36 What is a stack](https://www.youtube.com/watch?v=N3o5yHYLviQ&type=snipo&t=36s)

fast but why

LIFO memory

Seg fault (Core dumped) means going to somewhere else in memory that we shouldn’t go.

External fragmentation

![Untitled](Untitled%20647.png)

requesting memory takes time

### [1:43 The role of the operating system](https://www.youtube.com/watch?v=N3o5yHYLviQ&type=snipo&t=103s)

linux-swap is virtual memory to support ram

![Untitled](Untitled%20648.png)

### [3:21 Virtual memory](https://www.youtube.com/watch?v=N3o5yHYLviQ&type=snipo&t=201s)

### [5:10 Cache](https://www.youtube.com/watch?v=N3o5yHYLviQ&type=snipo&t=310s)

cache miss

![Untitled](Untitled%20649.png)

when using heap, we should ask operating system

[9:03](https://www.youtube.com/watch?v=N3o5yHYLviQ&t=543s&type=snipo)
Where we can write more data and that's it that's all it takes to allocate memory on the stack as you'll discover in my upcoming video this process is not as straightforward when allocating memory on the Heap in that scenario we must request memory from the operating system wait for it to locate available space and due to the system not returning the exact amount of needed memory we must employ fancy strategies to avoid fragmentation and all of those are extra steps that make the process 
 

### [11:40 Conclusion](https://www.youtube.com/watch?v=N3o5yHYLviQ&type=snipo&t=700s)

![Untitled](Untitled%20650.png)