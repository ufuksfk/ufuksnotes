---
draft: true
description:
socialDescription:
title: 001_-_Introduction_to_RTOS_Part_1_-_What_is_a_Real-Time_Operating_System_(RTOS)__Digi-Key_Electronics
  | Digi-Key Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


### [0:00 Introduction](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=0s)

### [0:27 What is an Operating System](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=27s)

![Untitled](Untitled%20989.png)

[1:45](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=1&t=106s&type=snipo)
Back and a little lag in responsiveness especially if it's not really noticed by a human is acceptable additionally the scheduler is often non-deterministic which means we can't know exactly which task will execute when and for how long if you're making something that requires an os and strict timing deadlines like a medical device or engine controller missing a deadline to say fire a spark 

![Untitled](Untitled%20990.png)

### [3:08 Superloop Architecture](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=188s)

![Untitled](Untitled%20991.png)

it is much easier to debug and saves memory and runtime energy

you can even use Interrupt Service Routine for precise timing

less than 1ms = best bet is interrupt

100 of ns, it is time to look for custom hardware or very fast mcu

you can’t run task concurrently

### [5:07 Task Priority](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=307s)

![Untitled](Untitled%20992.png)

### [6:59 Superloops](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=419s)

![Untitled](Untitled%20993.png)

### [7:57 Wireless Stack](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=477s)

why?

### [9:00 Free RTOS](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=540s)

![Untitled](Untitled%20994.png)

[9:17](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=1&t=557s&type=snipo)
The bare metal super loop architecture is still quite popular and an acceptable solution to many problems free rtos is also free and open source making it easy for you to try out note that as of 2017 amazon has taken over maintenance of the freertos project i also recommend keeping an eye on the zephyr project as it's a relative newcomer to the field backed by the linux foundation the esp32 is a powerful iot microcontroller that's 

### [9:43 Arduino](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=583s)

[10:09](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=1&t=609s&type=snipo)
That it creates a level playing field for anyone wanting to try out rtos concepts i don't need to teach a vendor tool or chip specific libraries on top of trying to teach free rtos because the esp32 runs a modified version of free rtos out of the box there is hardly any setup involved in creating tasks in arduino almost every code example you see including task management semaphores mutexes and so on can easily be ported 

### [10:43 Conclusion](https://www.youtube.com/watch?v=F321087yYy4&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=643s)