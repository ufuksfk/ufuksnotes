---
draft: true
description:
socialDescription:
title: Calculating Power Dissipation for a H-Bridge or Half Bridge Driver
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[ti.com]]
url: https://www.ti.com/lit/an/slva504a/slva504a.pdf

last highlighted date: [[2023-10#10]]

## Highlights
- Power dissipation from conduction loss of each FET due to its on-resistance is given by:PRON [W] = RON × IL2, where, (1)a. RON = FET on-resistance [ohm]b. IL = Load current [A]
    - Tags: [[electronics/power-dissipation]] 
    - Note: power dissipation from conduction loss
- Power dissipation due to output slewing during rising and falling edges is given by:PSW1 [W] = (0.5 x VM x IL x VM / SRrise x fPWM) + (0.5 x VM x IL x VM / SRfall x fPWM), where, (2)i. fPWM = PWM switching frequency [Hz]ii. VM = Supply voltage to the driver [V]iii. IL = Load current [A]iv. SRrise = Output voltage slew rate during rise [V/sec]v. SRfall = Output voltage slew rate during fall [V/sec]Output slewing rate is a balance between EM (Electro magnetic) performance and device powerdissipation.
    - Tags: [[electronics/power-dissipation]] 
    - Note: power dissipation due to output slewing
- Power dissipation due to the dead times between switching FETs is given by:PSW2 [W] = (VD x IL x tDEADrisex fPWM) + (VD x IL x tDEADfallx fPWM), where, (3)i. fPWM = PWM switching frequency [Hz]ii. VD = FET body diode forward bias voltage [V]iii. IL = Load current [A]iv. tDEADrise = dead time during rise [sec]v. tDEADfall = dead time during fall [sec]Dead times are necessary to mitigate any risk of current shoot through between the switching powerFETs. Integrated FET drivers often have a feedback based self timed FET switching sequence to ensurethe smallest possible dead times while avoiding any shoot through current.
    - Tags: [[electronics/power-dissipation]] 
- Power dissipation due to OUTPUT slewing during FET turn ON in the recirculation path is given by:PSW3 [W] = (0.5 x VD x IL x VD / SRrise x fPWM) + (0.5 x VD x IL x VD / SRfall x fPWM), where, (4)i. fPWM = PWM switching frequency [Hz]ii. VD = FET body diode forward bias voltage [V]iii. IL = Load current [A]iv. SRrise = Output voltage slew rate during rise [V/sec]v. SRfall = Output voltage slew rate during fall [V/sec]This dissipation is typically not considered as it is quite insignificant.
    - Tags: [[electronics/power-dissipation]] 
