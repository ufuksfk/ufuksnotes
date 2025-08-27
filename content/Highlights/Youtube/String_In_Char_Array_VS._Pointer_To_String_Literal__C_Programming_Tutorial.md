---
draft: true
description:
socialDescription:
title: String_In_Char_Array_VS._Pointer_To_String_Literal__C_Programming_Tutorial
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=Qp3WatLL_Hc&type=snipo

[[Portfolio Courses]]


Created time: [[2024-03#10]]

### [0:00 Introduction](https://www.youtube.com/watch?v=Qp3WatLL_Hc&type=snipo&t=0s)

### [0:24 String Literal](https://www.youtube.com/watch?v=Qp3WatLL_Hc&type=snipo&t=24s)

string literal means someone in memory there is abcdef and termination char

### [2:00 String In Char Array](https://www.youtube.com/watch?v=Qp3WatLL_Hc&type=snipo&t=120s)

s1 is in stack

![Untitled](Untitled%20717.png)

<aside>
💡 both case printf get the pointer to the first character

</aside>

![Untitled](Untitled%20718.png)

we modify place in memory.

with s1[] it means it is a string in stack, with *s2=”sdifk” we can’t be sure where it is!

if we use s1[], we can’t increment pointer. it is const pointer.

but for char *s2, you can just use s2++ means referencing next character

![Untitled](Untitled%20719.png)

here we changed the s2 to another char array in memory, who knows where?

s1[] is char array in stack size of 7 bytes

s2 is a pointer to char array, size of 8 bytes as it is only pointer.

if we use const char, it makes fixed value referencing to fixed part of the memory