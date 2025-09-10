---
draft: true
description:
socialDescription:
title: Understanding_Signal_Integrity
tags:
- highlight/youtube
date: 2025-05-18
modified: 2025-08-21
---

[[Signal Integrity]]
link: https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo
author: [[Rohde Schwarz]]
Created time: [[2024-03#17]]

### [0:00 Introduction](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=0s)

### [0:13 About signals, digital data, signal chain](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=13s)

### [0:53 Requirements for good data transmission, square waves](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=53s)
Requirements for good data transmission:
* Most digital data is transmitted as "square wave" signals
	* Consist of multiple frequency components
* Good digital data transmission requires:
	* Constant amplitude change for all frequency components
	* Constant time shift/delay for all frequency components
* If either of these are not constant, signal distortion may occur
![[Pasted image 20250313102205.png|200]]

### [1:47 Definition of signal integrity, degredations, rise time, high speed digital design](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=107s)
* [[Signal Integrity]] is the ability of a system to transfer (data) signals without excessive distortion
* Signal degradations are present in all systems
	* Signal integrity becomes more important at higher speeds (shorter rise times)
* "High speed" is not strictly define [[High Speed Signals]]
	* Rise times on the order of 1ns
### [2:55 Channel (ideal versus real)](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=175s)

![Untitled](Attachments/Untitled%20206.png)

### [3:46 Channel formats](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=226s)

![Untitled](Attachments/Untitled%20207.png)

### [4:16 Sources of channel degradations](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=256s)

![Untitled](Attachments/Untitled%20208.png)

### [4:36 Impedance mismatches](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=276s)

[[Impedance mismatch]]:
* Signal should see constant impedance along the path
* Mismatches (changes) -> reflections -> distortion
* Sources of mismatch:
	* Changes in trace dimensions
	* Improper terminations / unterminated stubs
	* Via characteristics
	* Discontinuities
	* Variations in board materials
	* Return path
### [5:39 Frequency response / attenuation, skin effect](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=339s)

![Untitled](Attachments/Untitled%20210.png)

### [6:52 Crosstalk](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=412s)

[[Crosstalk of PCB traces]]
* Coupling of energy between conductors (traces)
	* Usually caused by mutual inductance and or mutual capacitance
* Near end crosstalk
* Far end crosstalk
* Faster rise times create greater levels of crosstalk
* Can be minimized by:
	* Increased seperation between traces
	* Minimizing parallel run lengths
	* Placing conductors close to ground plane
![[Pasted image 20250313102917.png|300]]

### [7:47 Noise, power integrity, EMC, EMI](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=467s)
[[(EMC) Electromagnetic Compatibility]] 

![Untitled](Attachments/Untitled%20212.png)

### [8:38 Jitter](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=518s)
[[Jitter of digital signal]] is variations in timing of the signal
* Signal is sampled at defined bit times
* Signal transitions must occur between sample times
* Can cause undefined or incorrect values at sample times
	* Cretates bit errors
Types of jitter
* Data dependent jitter
* Periodic jitter
* Random jitter
![[Pasted image 20250313103137.png|200]]

### [9:30 About signal integrity testing](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=570s)

![Untitled](Attachments/Untitled%20214.png)

### [9:41 Simulation](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=581s)

### [10:22 Instruments used in signal integrity measurements, oscilloscopes, VNAs](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=622s)

[[Wiki/Technical/Oscilloscope]] vs [[Network Analyzer]]

![Untitled](Attachments/Untitled%20215.png)

### [11:16 Eye diagrams, mask testing](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=676s)
[[Eye diagram testing]]:

![Untitled](Attachments/Untitled%20216.png)

![Untitled](Attachments/Untitled%20217.png)

### [12:22 Eye diagrams along the signal path](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=742s)

![Untitled](Attachments/Untitled%20218.png)

### [12:48 Summary](https://www.youtube.com/watch?v=anX8QZMhVjI&type=snipo&t=768s)

![Untitled](Attachments/Untitled%20219.png)