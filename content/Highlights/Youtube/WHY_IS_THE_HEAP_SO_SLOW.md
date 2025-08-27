---
draft: true
description:
socialDescription:
title: WHY_IS_THE_HEAP_SO_SLOW
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=ioJkA7Mw2-U&type=snipo

[[Core Dumped]]


Created time: [[2024-05#18]]

### [0:00 Introduction](https://www.youtube.com/watch?v=ioJkA7Mw2-U&type=snipo&t=0s)

stack is limited in size

### [1:32 System Calls](https://www.youtube.com/watch?v=ioJkA7Mw2-U&type=snipo&t=92s)

write is a wrapper of syscall

![Untitled](Untitled%20596.png)

![Untitled](Untitled%20597.png)

requesting a memory with syscall has a cost

### [5:23 Memory Layout](https://www.youtube.com/watch?v=ioJkA7Mw2-U&type=snipo&t=323s)

![Untitled](Untitled%20598.png)

![Untitled](Untitled%20599.png)

### [16:05 Why is the Heap so slow](https://www.youtube.com/watch?v=ioJkA7Mw2-U&type=snipo&t=965s)

if we need to allocate big memory, it started to make sense to use linked list