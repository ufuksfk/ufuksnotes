---
draft: true
description:
socialDescription:
title: IEC 82304 vs IEC 62304 Software Standards for SaMD Explained-2
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[greenlight guru]]
url: https://www.greenlight.guru/blog/iec-82304-vs-iec-62304

last highlighted date: [[2024-04#08]]

## Highlights
- IEC 82304-1 is one of many standards that medical device companies should use while developing [[(SaMD) Software as Medical Device]]. It covers the requirements for manufacturers building health software products that are used without a dedicated hardware device.
- In fact, IEC 82304 requires the use of IEC 62304 and builds on its requirements in places.
- It covers the general requirements for the safety and security of health software products that are “intended to be placed on the market without dedicated hardware.” And while that [does include SaMD](https://www.greenlight.guru/blog/samd-software-as-a-medical-device), the definition of health software used in IEC 82304 is much broader than that.
    - Note: not only SaMD
- The standard defines health software as “software intended to be used specifically for maintaining or improving health of individual persons or the delivery of care.” This could include software not classified as a medical device such as:
  • Prescription management systems
  • Laboratory information management systems
  • Radiology information systems
    - Note: so these are not medical devices?
- IEC 82304 is a “product standard”, meaning it offers you guidance on how to design a product. In this case, the standard is focused on system-level requirements for health software manufacturers, such as:
  • Product use requirements
  • Product validation plans and reports
  • Product identification and instructions for use
  • Post-market activities
    - Tags: [[IEC 82304]] 
    - Note: product standard means..
- IEC 62304 applies to a more narrow subset of software than IEC 82304: medical device software. Medical device software includes both SaMD and embedded software, also known as [software in a medical device](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/content-premarket-submissions-device-software-functions) (SiMD). Some examples of SiMD are:
  • Software that controls the mortar in an infusion pump
  • Software used in closed loop control of a pacemaker or other hardware medical device
    - Tags: [[IEC 62304]]
- This is one of the major differences between the two standards. IEC 82304 is for standalone software only—products that are used “without dedicated hardware.” IEC 62304, on the other hand, can be used for SiMD that is embedded in a hardware medical device.
    - Tags: [[IEC 62304]] [[IEC 82304]] 
    - Note: difference between iec 62304 vs iec 82304
- ![](https://blog.greenlight.guru/hubfs/IEC%2082304%20and%2062304%20graphic.png)
- IEC 82304 helps bridge the gap between IEC 62304 and the [regulations on validation](https://www.greenlight.guru/blog/design-verification-and-design-validation). For SaMD manufacturers already using IEC 62304, adding IEC 82304 should help ensure that their software has been validated and maintained through the entire product lifecycle.
