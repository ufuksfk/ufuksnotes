---
draft: true
description:
socialDescription:
title: "PCB_Design_for_EMI_&_SI_-_Phil's_Lab_#64"
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---
https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo

[[Phil’s Lab]]


Created time: [[2024-03#17]]
[[(EMI) Electromagnetic Interference]]
### [0:00 Introduction](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=0s)

### [0:34 Altium Designer Free Trial](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=34s)

### [0:55 JLCPCB & Git Repo](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=55s)

### [1:15 Signals, Energy, and Fields](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=75s)

![Untitled](Untitled%20683.png)

### [2:02 Microstrip and Stripline](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=122s)

![Untitled](Untitled%20684.png)

### [2:49 Frequency in the Digital Domain](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=169s)

![Untitled](Untitled%20685.png)

### [3:34 Highest Frequency of Concern](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=214s)

### [4:08 Rise/Fall Times from IBIS Models](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=248s)

![Untitled](Untitled%20686.png)

problem is here it gave max, which is best case. We need to design to worst case.

Let’s check IBIS model.

In the ramps section.

![Untitled](Untitled%20687.png)

[7:54](https://www.youtube.com/watch?v=VtzPL8wQ8-E&t=475s&type=snipo)
Frequency content is hidden so to speak in these rising and falling edges so it turns out we actually need to take care when our traces so our trace lengths start to look like distributed elements rather than lumped elements this means that the trace length starts to be comparable to the wavelength of the highest frequency component so if our trace length is similar to the wavelength in this example of a 500 megahertz signal then we have to be concerned before we get to traces let's briefly 
 

### [8:19 How do we Control EMI/SI?](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=499s)

![Untitled](Untitled%20688.png)

### [9:20 Stackup](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=560s)

![Untitled](Untitled%20689.png)

[9:15](https://www.youtube.com/watch?v=VtzPL8wQ8-E&t=555s&type=snipo)
Talking about here it's number 56 on my channel and i'll leave a link as usual in the description below the first point is to use thin dielectrics between signal and reference planes for example you can see this full layer stack on the right we have a signal layer then a prepreg or dielectric material layer and then a reference layer underneath we want this preprick layer to be as thin as possible because this improves the coupling reduces inductances because we get small loop areas and if we have power and ground planes adjacent with thin dielectric this of course increases the interplay of capacitance improves power delivery and so on going for example to the jlc pcb manufacturer's 
 

JLC has better stackup!

![Untitled](Untitled%20690.png)

### [12:00 Traces and Termination](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=720s)

![Untitled](Untitled%20691.png)

they should be lumped element

### [13:21 Critical Length](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=801s)

![Untitled](Untitled%20692.png)

### [14:47 Vias](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=887s)

![Untitled](Untitled%20693.png)

this is better

![Untitled](Untitled%20694.png)

### [16:08 Reference Planes](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=968s)

![Untitled](Untitled%20695.png)

### [17:33 Separation](https://www.youtube.com/watch?v=VtzPL8wQ8-E&type=snipo&t=1053s)

![Untitled](Untitled%20696.png)