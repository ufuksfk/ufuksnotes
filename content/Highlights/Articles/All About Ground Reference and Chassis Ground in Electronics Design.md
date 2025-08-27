---
draft: true
description:
socialDescription:
title: All About Ground Reference and Chassis Ground in Electronics Design
tags:
  - highlight/articles
date: 2025-06-16
modified: 2025-08-21
---
author: [[Zachariah Peterson]]
url: https://resources.altium.com/p/stay-grounded-digital-analog-and-earth-ground-pcb-layout
last highlighted date: [[2025-06#08]]
published date: [[2018]]

[[Proper grounding at PCB Design]]
[[Chassis Ground]]
## Highlights
- Ground provides a reference point that is used to measure voltages. All voltages are defined in terms of the electric field (and potential energy) between two points. One of these points can be defined as "0 V", and it just so happens that we call this 0 V reference a "ground". This is one of the reasons we say that a ground plane in a PCB is a "reference plane".
- This can even happen when two devices reference the same conductor as a ground connection. If you were to measure the potential difference across a long conductor (e.g., with a multimeter), it could be non-zero, meaning some current is being driven along the conductor. This difference in potential along a large ground or between two ground connections is called "ground offset". In larger multiboard systems, or in areas like industrial and networking equipment, ground offset is one of the drivers for using differential signaling (e.g., [CAN bus](https://resources.altium365.com/p/Controller-Area-Network-Bus-Introduction-and-History), [Ethernet](https://resources.altium.com/p/gigabit-ethernet-101-basics-implementation), etc.). Because differential protocols use the voltage difference across two wires, their respective ground references are irrelevant, and signals can still be interpreted.
- ![Electronics ground symbol](https://files.resources.altium.com/sites/default/files/inline-images/pcb-ground-symbols.png)
- This type of earth ground connection from provides three functions:
  1. Because the chassis is now set to a global 0 V ground reference potential, the chassis now acts as a Faraday cage and provides broadband shielding.
  2. It provides a safety function that dissipates spurious currents (ESD, shorts, or noises) back to earth. This is one reason we sometimes call the chassis ground a "safety ground".
  3. It can provide a low-impedance sink for common-mode noise on this input EMI filter without placing a ferrite or large choke on the board.
- In a battery-powered system, or in a system with a simple 2-wire DC power connection, the PCB ground plane can be tied back to the chassis via mounting holes. The idea here is to ensure there is no floating conductor as an ungrounded conductor can act as a radiator due to capacitive coupling of current into the chassis. An ungrounded chassis or other floating conductors in the board can be sources of radiated EMI that can be easily eliminated by connecting to a ground.
- In an un-isolated 3-wire AC system, or in a 3-wire AC system that gets rectified to DC, if you connect the signal reference ground in a circuit to earth, you're just shorting out the negative wire on the AC or DC line. Don't do this because now the chassis can be a big current-carrying conductor! There is now a risk of shock (in high voltage/current systems) or intense EMI (in high frequency systems). When this is done, current will move back to the earth connection as long as that is the path of least reactance back to ground, and that path might be through someone who touches the device while it carries high current.
- In a 2-wire system (no earth ground connection), there are varying guidelines on how or if to connect the signal ground back to the chassis. Some guidelines say multipoint grounding is okay, others say to use a single point near the I/O, and still others say to use a single point near the power connector for safety. If RF noise is a problem throughout the system, you can tie back to chassis at multiple points to dissipate noise, but you probably have a bigger problem in your layout because you did not build the stackup correctly, and the device is just receiving too much radio energy. Focus on [building the stackup correctly](https://resources.altium.com/p/how-design-perfect-pcb-stack-altium-designer) and you might not need to stitch mounting hole connections all over the board, you'll just need it at a few points. You should not make a connection back to earth in this case.
