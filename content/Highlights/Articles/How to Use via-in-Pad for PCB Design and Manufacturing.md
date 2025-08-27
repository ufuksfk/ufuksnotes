---
draft: true
description:
socialDescription:
title: How to Use via-in-Pad for PCB Design and Manufacturing
tags:
  - highlight/articles
date: 2025-05-25
modified: 2025-08-21
---
author: [[The Sierra Team]]
url: https://www.protoexpress.com/blog/via-in-pad-pcb-design-manufacturing/
last highlighted date: [[2025-05#25]]
published date: [[2020-05]]

[[Via-in-pad]]
[[Via (electronics)]]
## Highlights
- • Implementing via-in-pad technology facilitates the miniaturization of PCBs and allows you to use fine-pitch components.
  • VIP eases the routing of complex designs with BGAs and high component density.
  • The via-in pad allows for close placement of bypass capacitors, increasing the heat dissipation of your design.
- ![](https://www.protoexpress.com/blog/wp-content/uploads/2020/05/all_via_types-1024x740-1.png)
- ![](https://www.protoexpress.com/blog/wp-content/uploads/2020/05/3commonvias_prosandcons.png)
- Microvias are minute holes with a size equal to or less than 6 mils, drilled in a PCB using a laser. Microvias are generally implemented in [HDI PCB](https://www.protoexpress.com/products/hdi-printed-circuit-boards)s.
- Here, the via is placed directly on the copper pad of a surface-mounted component and plated with copper (VIPPO), as opposed to a conventional via in which the signal-carrying trace is routed away from the pad (dog-bone) to the via. A via-in-pad serves the function of **miniaturizing the PCB** form factor by reducing the space taken up by trace routing. The most typical applications of these via-in-pads are with BGA components of pitches 0.5mm or less.
- ![](https://www.protoexpress.com/blog/wp-content/uploads/2020/05/via-in-pad_edit-2.png)
- There are other advantages to using VIP routing. Compared to other routing options, via-in-pad has the following benefits:
  • It is easier to route fine pitch ball grid arrays (BGAs), which can turn out to be smaller than 32 and 40 mils (0.8mm and 1mm). To learn how to break small-pitch BGA and microcontroller using via-in-pad, see our [case study on routing microcontroller and BGA in rigid-flex PCBs](https://www.protoexpress.com/blog/case-study-routing-microcontroller-and-bga-in-rigid-flex-pcbs/).
- When you eliminate surface routing, you can place bypass capacitors closer to components, therefore minimizing inductance. This is useful for enhanced thermal management.
- VIP routing also works wonders for high-frequency component grounding.
- ![](https://www.protoexpress.com/blog/wp-content/uploads/2020/05/via_in_pad_02_01.png)
- The capped vias are sometimes prone to [offgassing](https://www.protoexpress.com/blog/how-to-mitigate-outgassing-effects-pcbs/). Offgassing or outgassing refers to blow-off vapor due to the thermal expansion of gas. The gas is a result of a phase transition from liquid to vapor due to heating during the [soldering process](https://www.protoexpress.com/blog/8-soldering-tips-to-watch-out-for/).
- [Thermal pads](https://www.protoexpress.com/blog/use-thermal-pads-pcb-design-manufacturing/) don’t require soldering, so you don’t need to count them as via-in-pad for online quoting.
- ![](https://www.protoexpress.com/blog/wp-content/uploads/2020/05/connector-pad-q1-1.png)
- You can use the via-in-pad guidelines given below for surface mount device routing:
  • Stick to recommendations from component manufacturers for component placement and via capping and filling.
  • Limit microvias to one layer of the PCB.
  • Ensure you cap the non-component side with a solder mask.
  • Avoid leaving vias open unless absolutely necessary – leaving vias open exposes the via copper to the environment, leading to oxidation effects or worse. This can shorten PCB life.
