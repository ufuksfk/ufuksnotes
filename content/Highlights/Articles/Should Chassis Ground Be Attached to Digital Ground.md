---
draft: true
description:
socialDescription:
title: Should Chassis Ground Be Attached to Digital Ground
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[electronics.stackexchange.com]]
url: https://electronics.stackexchange.com/questions/19561/should-chassis-ground-be-attached-to-digital-ground
last highlighted date: [[2025-06#08]]

[[Proper grounding at PCB Design]]
## Highlights
- Here's the question: **Should the CHASSIS_GND be tied to the digital GND plane in any way?** I've read countless app notes and layout guides, but it seems that everybody has differing (and sometimes seemingly contradictory) advice about how these two planes should be coupled together
- I've done it several ways, but the way that seems to work best for me is the same way that PC motherboards do it. Every mounting hole on the PCB connects signal gnd (a.k.a. digital ground) directly to the metal chassis through a screw and metal stand-off.
- **Tie them together at a single point with a 0 Ohm resistor near the power supply**
  Don't do that. Doing this would assure that any noise on the cable has to travel THROUGH your circuit to get to GND. This could disrupt your circuit. The reason for the 0-Ohm resistor is because this doesn't always work and having the resistor there gives you an easy way to remove the connection or replace the resistor with a cap.
- **Tie them together at a single point with a 0 Ohm resistor near the power supply**
  Don't do that. Doing this would assure that any noise on the cable has to travel THROUGH your circuit to get to GND. This could disrupt your circuit. The reason for the 0-Ohm resistor is because this doesn't always work and having the resistor there gives you an easy way to remove the connection or replace the resistor with a cap.
- **Tie them together with a single 0.01uF/2kV capacitor at near the power supply**
  Don't do that. This is a variation of the 0-ohm resistor thing. Same idea, but the thought is that the cap will allow AC signals to pass but not DC. Seems silly to me, as you want DC (or at least 60 Hz) signals to pass so that the circuit breaker will pop if there was a bad failure.
- **Tie them together with a 1M resistor and a 0.1uF capacitor in parallel**
  Don't do that. The problem with the previous "solution" is that the chassis is now floating, relative to GND, and could collect a charge enough to cause minor issues. The 1M ohm resistor is supposed to prevent that. Otherwise this is identical to the previous solution.
- **Short them together with a 0 Ohm resistor and a 0.1uF capacitor in parallel**
  Don't do that. If there is a 0 Ohm resistor, why bother with the cap? This is just a variation on the others, but with more things on the PCB to allow you to change things up until it works.
- **Tie them together with multiple 0.01uF capacitors in parallel near the I/O**
  Closer. Near the I/O is better than near the power connector, as noise wouldn't travel through the circuit. Multiple caps are used to reduce the impedance and to connect things where it counts. But this is not as good as what I do
- **Leave them totally isolated (not connected together anywhere)**
  This is basically what is done when you don't have a metal chassis (like, an all plastic enclosure). This gets tricky and requires careful circuit design and PCB layout to do right, and still pass all EMI regulatory testing. It can be done, but as I said, it's tricky.
- The chassis ground is for safety only. From what I understand it's best to keep the actual ground plane of the circuit isolated, meaning that the chassis and digital grounds only connect at/outside of the power supply. This is done for several reasons, but two of the big benefits:
  1. Much less chance that any radio energy the chassis (or it's components) pick up leak into the digital circuitry
  2. Significantly reduces the degree that the chassis will serve as an "unintentional radiator" - eg the oscillations and state changes in the digital circuitry are much less likely to be amplified/radiated by the chassis.
