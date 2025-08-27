---
draft: true
description:
socialDescription:
title: 004_-_Introduction_to_RTOS_Part_4_-_Memory_Management__Digi-Key_Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


### [0:00 Introduction](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=0s)

Most C programs rely on 3 different types of memory. Static memory is set aside prior to program execution and used for things like static variables, constants, and global variables. Stack is allowed to grow dynamically and consists of local variables declared at the function level. Finally, heap may also grow dynamically and must be specifically allocated and deallocated by the programmer (e.g. using the malloc() and free() functions, respectively).

### [0:16 Memory Allocation](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=16s)

![Untitled](Untitled%201016.png)

![Untitled](Untitled%201017.png)

[0:59](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=59s&type=snipo)
Continually push variables to the stack when making nested function calls upon returning to the caller function variables can be popped off the stack as part of the return data or deleted entirely memory is deallocated when a function returns while the compiler will reserve as much stack as it thinks is needed for local variables the stack can grow in size automatically allocating what's needed from free memory you'll often see this happen with things like recursive function calls local variables 

![Untitled](Untitled%201018.png)

[1:16](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=76s&type=snipo)
Needed for local variables the stack can grow in size automatically allocating what's needed from free memory you'll often see this happen with things like recursive function calls local variables arguments and local pointers are stored in the stack this is known as automatic allocation there's a third area of memory called the heap like the stack it can grow as the program runs and it usually grows toward the stack note that this exact layout can change among 

![Untitled](Untitled%201019.png)

[2:07](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=128s&type=snipo)
Required to free up any memory you dynamically allocated when you are done using it if you forget to do so like at the end of a function you could cause the heap to continue growing indefinitely this is known as a memory leak and can be sometimes difficult to track down additionally the heap and stack could run into each other if you let them grow unbounded and start overwriting each other's memory this is also bad and could cause some nasty undefined effects there is some 

![Untitled](Untitled%201020.png)

[3:29](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=209s&type=snipo)
Automatically set aside a new tcb and stack inside the heap when we start talking about kernel objects like queues and semaphores these will be stored in the heap as well note that there is a way to allocate static memory for tasks and kernel objects in newer versions of freertos this can be really useful in critical applications like medical devices or satellites where a memory leak could be catastrophic to enable this you need to define the config support static allocation parameter as one right now it does not seem that esp idf has this set by default so we can't use static tasks out of the box with our 
 

### [4:26 Heap Allocation](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=266s)

[4:44](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=285s&type=snipo)
This scheme to make parts of the heap act like static memory free rtos considers heap 2 to be obsolete in favor of heap 4 which allows fragmented areas of the heap to be joined together this helps reduce fragmentation note that the normal c malloc and free functions are not thread safe and the time it takes for each to execute cannot be determined at compile time heap 3 wraps the malik and free functions to allow them to be

### [6:00 Bare Bones Example](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=360s)

![Untitled](Untitled%201021.png)

![Untitled](Untitled%201022.png)

![Untitled](Untitled%201023.png)

[7:56](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&t=476s&type=snipo)
With the export get heap size function unlike the stack high watermark this gives us total available heap in bytes rather than words let's see what happens when we print out the heap size before and after we use malik to allocate some memory in vanilla free rtos unless you're using the heap 3 scheme you'll want to use pv port malik as regular malloc is not thread safe in esp-idf you can use regular malloc but i'd like to 

by using thread safe free, heap stays free.

### [9:42 Your Challenge](https://www.youtube.com/watch?v=Qske3yZRW5I&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo&t=582s)