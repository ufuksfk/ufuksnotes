---
draft: true
description:
socialDescription:
title: Infineon-ApplicationNote_PFCCCMBoostConverterDesignGuide-AN-v02_00-EN.pdf
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
from [[Infenion]]
url: https://www.infineon.com/dgdl/InfineonApplicationNote_PFCCCMBoostConverterDesignGuide-AN-v02_00-EN.pdf?fileId=5546d4624a56eed8014a62c75a923b05

last highlighted date: [[2023-10#20]]
[[Boost Converter]]
## Highlights
- FC Inductor and input line current waveforms in the three different operating modes0 1 10 4- 2 10 4- 3 10 4- 4 10 4-051015Iin t( )IL t( )tCritical Conduction Mode (CrCM)
    - Note: how CCM CrCM DCM differs in current-time graph
- For a boostconverter, the following are some major MOSFET selection considerations for high efficiency applicationdesign: Low figure-of merits - RDS(ON)*Qg and RDS(ON)*Eos
    - Note: boost converher MOSFET selection guide
- Fast turn-on/off switching to reduce the device switching losses Gate plateau near middle of gate drive range to balance turn-on/off losses Low output capacitance Coss for low switching energy and to increase light load efficiency Drain-source breakdown voltage VBR(DSS) to handle spikes/overshoots Low thermal resistance RthJC. Package selection must consider the resulting total thermal resistance fromjunction to ambient, and the worst case surge dissipation, typically under low-line cycle skipping andrecovery into highline while ramping the bulk voltage back up. The body diode commutation speed and reverse recovery charge are not important, since body diodenever conducts in the CCM boost converter.
    - Note: Boost converter MOSFET selection guide
- Selection of the optimum on-state resistance of a specific CoolMOS™ series is based on the balancingbetween switching losses and conduction losses of the device at a targeted load point.
