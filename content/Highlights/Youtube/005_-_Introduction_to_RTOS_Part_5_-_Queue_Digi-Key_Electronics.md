---
draft: true
description:
socialDescription:
title: 005_-_Introduction_to_RTOS_Part_5_-_Queue_Digi-Key_Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


### [0:00 Intro](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=0s)

using queue instead of global variable

### [0:19 Example](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=19s)

what happens taskA and TaskC race for it 

![Untitled](Untitled%201004.png)

### [1:07 Memory Overwriting](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=67s)

ESP32 is little endian

![Untitled](Untitled%201005.png)

one way is using atomic operations 

### [3:19 Queue](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=199s)

![Untitled](Untitled%201006.png)

[3:42](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=5&t=223s&type=snipo)
Functions writing to a queue is atomic which means that another task cannot interrupt it during the writing process also note that adding something to a queue is done by value and not by reference that means whenever you save something to the queue the entire contents of that variable struct string or buffer are copied you can place a pointer into a queue but you'll want to be sure the referenced value is still in scope by the time the pointer is read by 

### [5:09 Queue Functions](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=309s)

![Untitled](Untitled%201007.png)

[5:18](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=5&t=318s&type=snipo)
Delete send and receive which i'll show you how to use in a minute notice that there are static cues which means that the basic cues are created in heap memory additionally you should not send or receive items from a queue from within an interrupt service routine using these basic functions that's because interrupts do not depend on the tick timer and should not wait any amount of time for the queue as a result you should use these special from isr functions when working with a cue inside 

### [5:48 Arduino Sketch](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=348s)

[7:55](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=5&t=475s&type=snipo)
After 10 ticks if it can't copy the value to the queue the function will return pd false which we can check i'll print out an error message here note that it's generally a good idea to assign one hardware peripheral per task which means that i should have my print messages task handle all serial input and output and not have serial commands in other tasks however this is a demo so i'll leave this print statement here it 

### [9:40 Challenge](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=580s)

![Untitled](Untitled%201008.png)

### [10:48 Serial Terminal](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=648s)

### [11:31 Outro](https://www.youtube.com/watch?v=pHJ3lxOoWeI&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=691s)