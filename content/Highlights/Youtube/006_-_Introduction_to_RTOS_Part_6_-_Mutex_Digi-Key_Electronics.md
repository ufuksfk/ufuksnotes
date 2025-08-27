---
draft: true
description:
socialDescription:
title: 006_-_Introduction_to_RTOS_Part_6_-_Mutex_Digi-Key_Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


### [0:00 Intro](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=0s)

![Untitled](Untitled%201024.png)

### [1:04 Example](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=64s)

[1:20](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=6&t=80s&type=snipo)
Be accomplished in a single instruction cycle a queue was useful in helping us pass messages to other tasks but what happens if we need to keep the global variable around as a flag or counter for other tasks to see **a race condition is an issue in electronics and software where the system's behavior is dependent on the timing of uncontrollable events** here we have two tasks that call the same inc task function we start both 

### [2:21 Race Condition](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=141s)

![Untitled](Untitled%201025.png)

### [4:09 Critical Section](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=249s)

![Untitled](Untitled%201026.png)

![Untitled](Untitled%201027.png)

mutex is same as lock but for whole system

[6:22](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=383s&type=snipo)
Mutex which is a shortening of the phrase mutual exclusion is the same as a lock but it works for all processes on the system since we're only running one process in our free rtos environment a lock is the same as a mutex a semaphore is similar to a mutex but it contains a counter that allows a limited number of threads to enter a critical section at a time in practice a semaphore is used as a way to signal to other threads we'll explore semaphores in the next lecture 

### [6:56 Mutex](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=416s)

mutex is key to access memory

[7:43](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=464s&type=snipo)
Have access to and it can be represented as a simple zero or one boolean value task a will begin by checking to see if the mutex exists and taking it if so note that this action must be atomic meaning no other tasks can interrupt it in the process of checking for and taking the mutex some processor architectures have special test and set assembly instructions that allow this to occur in one instruction cycle if the 

![Untitled](Untitled%201028.png)

### [9:36 Free RTOS Demo](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=576s)

freertos just generalize mutex and semaphore as semaphore

[11:13](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=674s&type=snipo)
Repeat a value thanks to the protected critical section you can check out the semaphore api section on the freertos site if you'd like to see the available functions for working with mutexes and semaphores just like we saw with cues you should not give and take mutexes and semaphores inside interrupt service routines using the basic functions instead you should use these from isr functions to do that now it's time for your challenge i've been avoiding using 

### [11:39 Hack with Mutex](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=699s)

### [13:10 Outro](https://www.youtube.com/watch?v=I55auRpbiTs&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=790s)