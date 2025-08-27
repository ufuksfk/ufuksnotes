---
draft: true
description:
socialDescription:
title: 010_-_Introduction_to_RTOS_Part_10_-_Deadlock_and_Starvation__Digi-Key_Electronics
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=hRsWi4HIENc&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&type=snipo

[[DigiKey]]


[0:10](https://www.youtube.com/watch?v=hRsWi4HIENc&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=10&t=10s&type=snipo)
Think and eat a giant bowl of noodles is placed in the middle of the table this restaurant is a little odd the server places one chopstick between each diner each philosopher can only eat when they have two chopsticks the challenge is to come up with an algorithm that guarantees each philosopher spends some time eating if you studied operating systems or multi-threading in the past you'll probably recognize this as the classic dining philosopher's problem 

![Untitled](Untitled%201031.png)

![Untitled](Untitled%201032.png)

![Untitled](Untitled%201033.png)

[2:31](https://www.youtube.com/watch?v=hRsWi4HIENc&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=10&t=151s&type=snipo)
Or as we saw in the previous lecture you can have your high priority task only run when it receives some kind of notification from an interrupt or event this allows lower priority tasks to run all other times another way to tackle starvation is through a technique called aging let's say that we have task a running at a higher priority than task b task a is hogging all the processor time the scheduler or another even higher priority task can periodically check the 

![Untitled](Untitled%201034.png)

note that free rtos does not use aging out of the box it's something you would need to implement assuming we keep the critical section 

![Untitled](Untitled%201035.png)

it may rarely occur but hard to debug

[5:53](https://www.youtube.com/watch?v=hRsWi4HIENc&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=10&t=354s&type=snipo)
Can see that task a is waiting for mutex 2 at this point which is held by task b and task b is waiting for mutex 1 which is held by task a this immediately results in a deadlock as neither task can continue i hope this illustrates why the use of multiple mutexes and semaphores can easily get you in trouble the first way to prevent or at least catch deadlock is to never have a task block forever while waiting for a queue

[7:14](https://www.youtube.com/watch?v=hRsWi4HIENc&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=10&t=434s&type=snipo)
Issues back to our philosopher's analogy a timeout simply means that after some set period each philosopher would put down their left chopstick and try again later while likely rare it's possible that all the philosophers pick up their left chopstick time out and put them down at the same time they would continue this process over and over again forever as all the timeouts are now synced this is an issue known as live lock while the 

![Untitled](Untitled%201036.png)

[9:38](https://www.youtube.com/watch?v=hRsWi4HIENc&list=PLXyB2ILBXW5FLc7j2hLcX6sAGbmH0JxX8&index=10&t=578s&type=snipo)
Mutex and do its work when it's done it returns both mutexes so that task b can do its job in the critical section this continues forever with no deadlock another solution to this problem is to introduce an arbitrator that determines who can eat in our analogy this would be like the philosophers requesting permission from a waiter to pick up the chopsticks in front of them the arbitrator can be implemented as a simple mutex that must be taken prior to 

![Untitled](Untitled%201037.png)