---
draft: true
description:
socialDescription:
title: 007_-_Introduction_to_RTOS_Part_7_-_Semaphore_Digi_488e389582d2448ca83dfe40932bdcf3
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=5JcMtbA9QEE&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


semaphore can count more than one. for the coffee shop analogy it suppose to be a notebook that you can write and read numbers

semaphore is more better for signalling between threads

we have critical section and we want at most 3 threads doing sth on it

![Untitled](Untitled%20995.png)

![Untitled](Untitled%20996.png)

semaphoreTake must be atomic

![Untitled](Untitled%20997.png)

![Untitled](Untitled%20998.png)

let’s check better way to work with semaphore

![Untitled](Untitled%20999.png)

 here's the thing if all this sounds very much like a cue you're right semaphores can often add unneeded complexity in a program and can be very difficult to debug if you can accomplish something using a queue you should probably do that instead 

![Untitled](Untitled%201000.png)

![Untitled](Untitled%201001.png)

![Untitled](Untitled%201002.png)

![Untitled](Untitled%201003.png)

[11:24](https://www.youtube.com/watch?v=5JcMtbA9QEE&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=7&t=684s&type=snipo)
The terminal 3 times in no particular order and then stop do this first with semaphores and then try it again with cues to see if it's any easier you'll only need a few lines of code to control the semaphores and mutex but it can be tricky to figure out where to place them good luck on this challenge o