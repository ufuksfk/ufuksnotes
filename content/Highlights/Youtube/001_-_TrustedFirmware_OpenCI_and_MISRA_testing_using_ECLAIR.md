---
draft: true
description:
socialDescription:
title: 001_-_TrustedFirmware_OpenCI_and_MISRA_testing_using_ECLAIR
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=fzo8dKs2_UY&list=PLlXBA-Zkgo5Y74N9fgjdHXD2VL4-8hSMc&type=snipo

[[BUGSENG]]


advantage of the C programming language

![Untitled](Untitled%20867.png)

disadvantage

![Untitled](Untitled%20868.png)

What is “Behavior”

![Untitled](Untitled%20869.png)

There is no guarantee that compiler generates x++ code.

## Undefined behavior

![Untitled](Untitled%20870.png)

![Untitled](Untitled%20871.png)

- [ ]  why? because str pointer is read only memory? how?

## unspecified behavior

not as bad as undefined

![Untitled](Untitled%20872.png)

![Untitled](Untitled%20873.png)

compiler doesn’t document this. it can be both.

If you compute it 5 times, each time compiler gives different result

### implementation defined behavior

![Untitled](Untitled%20874.png)

## why?

![Untitled](Untitled%20875.png)

great example

![Untitled](Untitled%20876.png)

if the signed integer overflow is undefined behavior, then it would compile as is.

### modifying string literals

![Untitled](Untitled%20877.png)

shifting too much

![Untitled](Untitled%20878.png)

no! why?

![Untitled](Untitled%20879.png)

## strength and weakness of C

![Untitled](Untitled%20880.png)

![Untitled](Untitled%20881.png)

# misra c

good rule from misra c

## Misra C Rule 1.1

![Untitled](Untitled%20882.png)

![Untitled](Untitled%20883.png)

safety critical systems, that can’t be used. as they are not documented.

## Misra C Rule 3.2

![Untitled](Untitled%20884.png)

## misra c rule 9.1

mandatory

![Untitled](Untitled%20885.png)

solution:

![Untitled](Untitled%20886.png)

## misra c rule 13.2

![Untitled](Untitled%20887.png)

![Untitled](Untitled%20888.png)

example:

![Untitled](Untitled%20889.png)

solution:

![Untitled](Untitled%20890.png)

- [ ]  what is the side effect of defining volatile?

certified standarts

![Untitled](Untitled%20891.png)

trustedfirmware

![Untitled](Untitled%20892.png)

[Trusted Firmware - Open Source Secure Software](https://www.trustedfirmware.org/)

![Untitled](Untitled%20893.png)

![Untitled](Untitled%20894.png)