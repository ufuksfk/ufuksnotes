---
draft: true
description:
socialDescription:
title: Reverse Polarity Protection
tags:
  - note/electrical
date: 2025-05-18
modified: 2025-08-21
---
There are three principle components used for reverse polarity protection:
- Silicon diode
    - The simplest method for adding DC reverse polarity protection to a circuit is to place a series diode in front of the protected load or circuit. The circuit diagram below shows the correct placement.
    - Cons of series diode:
	    - loss of energy on diode
- [[Schottky diode]]
    For the Schottky diode and the silicon diode, there are two important specifications on these components that have to be considered:
    - Leakage current
    - Breakdown voltage
- P-type [[MOSFET]]
	- ![[Pasted image 20250408095200.png|300]]

## Diode as shunt
![[Pasted image 20250408095447.png|500]]
The **advantage** of this solution is that the added diode has no effect in normal operation and still provides protection in a reverse polarity situation.

The **disadvantage** is that there is still current flowing even if a reverse voltage is applied.

## Solution with series fuse

Another solution is a self-resettable PPTC fuse. The PPTC limits the current once it is heated up by the high current flow caused by the reverse polarity and the conducting protection diode.
![[Pasted image 20250408095532.png|500]]

https://www.monolithicpower.com/learning/resources/designing-a-reverse-polarity-protection-circuit-part-i

_**Series Schottky Diode**_  This circuit is typically used for low-current applications between 2A and 3A. Advantages include simplicity and lower cost, but there is greater power loss.

_**P-Channel MOSFET on the High Side**_  For applications with currents exceeding 3A, a P-channel MOSFET can be placed on the high side. This driving circuit is relatively simple, though it is more expensive due to the P-channel MOSFET.

_**N-Channel MOSFET on the Low Side**_  Another circuit requires placing an N-channel MOSFET on the low side. The simplified gate drive circuit uses a cost-effective N-channel MOSFET. This circuit functions similarly to a P-channel MOSFET that has been placed on the high side; however, the reverse polarity protection structure of this system means that the power supply ground and load ground are separated. This structure is rarely used when designing electronic automotive products.

![[Pasted image 20250408095628.png]]