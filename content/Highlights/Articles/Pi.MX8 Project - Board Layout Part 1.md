---
draft: true
description:
socialDescription:
title: Pi.MX8 Project - Board Layout Part 1
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[Altium]]
url: https://resources.altium.com/p/pimx8-project-chapter-three
last highlighted date: [[2025-06#13]]
published date: [[2024-02-22]]

## Highlights
- ![Component placement top side](https://files.resources.altium.com/sites/default/files/styles/max_width_1300/public/inline-images/Pi.MX8_Chapter_III_Image%201.jpg?VersionId=ILtc2h9jAtJbNhQROCw.xvpFtaqqjWHx&itok=kWk9TY5d)
- ![Component placement bottom side](https://files.resources.altium.com/sites/default/files/styles/max_width_1300/public/inline-images/Pi.MX8_Chapter_III_Image%202.jpg?VersionId=g7c5qKoaDiG.BUkCVZU9.22DCVRkWnZF&itok=G8ObWS_o)
- For the Pi.MX8 module we will be using a 2+N+2 layerstack. This is a type III layerstack as defined in the IPC-2226 standards and is one of the most commonly used HDI stacks.
- In contrast to mechanically drilled VIAs, micro VIAs are created by punching holes in the prepregs using short laser pulses. Typically, VIA diameters between 0.08mm and 0.15mm are used. An aspect ratio suitable for mass manufacturing usually is in the range of 0.6:1 – 0.8:1.
- The final stackup for the Pi.MX8 board was created in cooperation with the PCB manufacturer and looks as follows:
- ![Pi.MX8 Layerstack](https://files.resources.altium.com/sites/default/files/styles/max_width_1300/public/inline-images/Pi.MX8_Chapter_III_Image%203.png?VersionId=1ZmIpgLnjriWG1IEdVfGyLJI8Y_DWyXG&itok=kFEj7wNp)
- Overall, the module will be built on a 10-Layer stackup. The top, L2, L7, and bottom layers will be used as signal layers. Layer L1, L3, L6 and L8 will be used as ground planes. The two remaining layers L4 and L5 will act as the power planes. The power planes are built using a thin foil of only 18μm thickness. We have to keep an eye on the IR drop for these layers. The power planes are closely coupled to the neighboring ground planes with only a 75μm prepreg separating these layers. This results in additional plane capacitance which can be beneficial for providing a low PDN impedance at high frequencies. We´ll verify the PDN behavior by simulation once we have the layout completed.
- Another important aspect to note about this stackup is that we will be using only staggered instead of stacked micro VIAs. This means that micro VIAs can´t be placed directly on top of each other and instead must be offset with a pitch of at least 0.35mm center to center.
- Using staggered VIAs makes the registration of the sequential layers easier which decreases manufacturing cost with some PCB providers. This approach is also recommended for HDI stackups using more than two micro VIA programs to increase the reliability of the micro VIAs.
- This is especially true for VIAs that are part of the power distribution network as they usually connect through the whole stackup. Placing VIAs during the routing stage may require previously routed traces to be deleted to make room for VIAs.
- One such example is the i.MX8 SoC. The small pin pitch of only 0.5mm requires a trace width of 0.08mm and a trace to pad spacing of 0.085mm.
- One way is by using extra design rooms that are assigned a dedicated set of rules. This enables a smooth routing workflow as the trace width gets automatically adjusted once the cursor crosses the border of the design room.
- ![Trace width and spacing requirements for the i.MX8 break-out routing](https://files.resources.altium.com/sites/default/files/styles/max_width_1300/public/inline-images/Pi.MX8_Chapter_III_Image%205.png?VersionId=sWfSpi2K6hj4JF3qu0_XGC8icVP2vdwU&itok=DAsYio-p)
