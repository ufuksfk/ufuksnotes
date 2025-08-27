---
draft: true
description:
socialDescription:
title: USB Powered Device With Multiple Decoupling Capacitors
tags:
  - highlight/articles
date: 2025-05-18
modified: 2025-08-21
---
author: [[Electrical Engineering Stack Exchange]]
url: https://electronics.stackexchange.com/questions/38361/usb-powered-device-with-multiple-decoupling-capacitors
last highlighted date: [[2025-05#02]]
[[USB]] [[Decoupling capacitor]]
## Highlights
- According to [this source](http://www.beyondlogic.org/usbnutshell/usb2.shtml), the maximum allowed decoupling capacitance for a USB device is 10uF.
- Ultimately, any capacitance "behind" the power-management IC (i.e. hooked up to the IC outputs) isn't "seen" by the USB; the bus only sees the capacitance "in front of" the IC (i.e. hooked up to IC inputs).
- A USB device cannot present more than 10uF of capacitance when connected. This does not necessarily mean that you can only have 10uF of capacitors, it means that you need to limit the inrush current to that required to charge a 10uF upon connection. From the USB specification:
  > The maximum load (CRPB) that can be placed at the downstream end of a cable is 10 μF in parallel with 44 Ω. The 10 μF capacitance represents any [[bypass capacitor]] directly connected across the VBUS lines in the function plus any capacitive effects visible through the regulator in the device. The 44 Ω resistance represents one unit load of current drawn by the device during connect.
  Furthermore:
  > If more bypass capacitance is required in the device, then the device must incorporate some form of VBUS surge current limiting, such that it matches the characteristics of the above load.
  As you probably know, your device is allowed to draw 1 power unit, or 100mA, upon connection without any negotiation.
- The ["maximum capacitance across the Vbus pin"](https://www.microchip.com/stellent/groups/sitecomm_sg/documents/market_communication/en534460.doc) rule is intended to keep the Vbus voltage from dropping low enough to reset the other USB devices whenever a new USB device is plugged in.
- I've seen a few USB devices that only need a ferrite bead to keep the inrush current within specs. They connect only 2 things to the Vbus pin of the USB connector: the 1uF minimum VBUS decoupling capacitance directly across the Vbus and GND pins of the USB connector, and a ferrite bead that supplies power to the rest of the device. That allows them to use a net capacitance of slightly more than 10 uF on the other side of that ferrite bead.
