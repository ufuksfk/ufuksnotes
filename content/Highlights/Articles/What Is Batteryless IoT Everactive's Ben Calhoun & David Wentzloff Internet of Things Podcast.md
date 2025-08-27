---
draft: true
description:
socialDescription:
title: "What Is Batteryless IoT Everactive's Ben Calhoun & David Wentzloff Internet of Things Podcast"
tags:
  - highlight/articles
date: 2025-08-18
modified: 2025-08-21
---
author: [[IoT For All Podcast]]
url: https://share.snipd.com/episode/411acb23-5cef-4c71-b232-ce2f16fc6a25
last highlighted date: [[2025-W33#2]] 2025-08-12
published date: [[]]

## Highlights
- **Batteryless IoT**
  - Everactive delivers sustainable, scalable, and cost-effective IoT solutions.
  - They focus on low-power energy harvesting and wireless tech for battery-less, always-on systems.
  Transcript:
  Speaker 2
  On today's episode, we have Dr. Ben Calhoun, the co-founder and co-CTO of Ever Active. They are a company that is delivering a sustainable, scalable and cost-effective Internet of Things and Solutions with a focus on low-power energy harvesting and wireless technology That enables completely battery-less and always-on IoT systems powered entirely from micro-renewable energy. So we're going to talk a lot about that.
- **Ben Calhoun's Background**
  - Ben Calhoun is a technical co-founder and co-CTO of Everactive, as well as a professor at the University of Virginia.
  - His research focuses on low-power circuit design.
  Transcript:
  Speaker 1
  My name's Ben Calhoun. Along with Dave, I'm one of the technical co-founders of Everactive and Co-CTOs. I'm also a professor of electrical and computer engineering at the University of Virginia. My research at UVA is in low power circuit design, and my training for that was as a PhD student at MIT where I'm at Dave, so I'll turn it over to him.
- **Everactive's Founding Story**
  - Ben Calhoun and Dave Wentzloff, after becoming faculty members, collaborated on low-power chip design research across their universities.
  - They tackled batteryless applications, initially in wearable devices, even building a chip powered by body heat for ECG/EEG signal processing.
  Transcript:
  Speaker 1
  Well, it follows on to the story Dave started telling. After we went back to become faculty members and started research groups in low power chip design, we stayed in touch and talked about what it was like to grow our research groups and To be in the faculty setting. But then we started working together. And we were doing that across the two universities, writing grants together, getting funded research and then having students in Dave's group and students in my group working together As one big team to build these systems on chip or SOCs that were ultra-low power. And we were tackling applications that were batteryless. And initially those applications were mostly in the wearable device space. So we were part of a large national science foundation funded center to build batteryless wearables. So we built a chip that could operate entirely from body heat with no battery in the system and measure signals like your electric cardiogram or electroencephalogram and then do processing On the chip and a lot of sophisticated signal extraction and then use radios that Dave's group built to communicate back that data.
- **Batteryless Device Energy**
  - Batteryless devices harvest energy from the environment through transducers, converting it into electrical energy.
  - This intermittent energy is stored in a capacitor for sensing, processing, and communication tasks.
  Transcript:
  Speaker 1
  So the basic idea with a batteryless device is that you still need energy, so you harvest that energy from the environment. So you have some sort of a transducer that converts energy into the environment into electrical energy. So one that everybody's familiar with is a photovoltaic cell that converts light into electricity. But there are other options, for example, thermoelectric generators that convert differences in temperature into energy. You can also harvest from motion, electromagnetic energy, RF energy, a lot of other sources. So you take that energy from the environment, which is by nature intermittent, sometimes you have more available, sometimes you have less, sometimes you have none depending on the Environment. You convert it into usable energy. You want to make that conversion efficient. And then you store that energy locally in a capacitor, which is like a battery in the sense that it stores energy, but unlike a battery in the sense that it behaves richer and has some other Good features. And then you use that energy to do useful work. The work that you do is similar to what you might do with a battery, you know, in a sense or sensing something, processing it, communicating it, you can do actuators. But the difference is the energy source, which sounds maybe at first like it's troublesome and in ways it is troublesome. You don't have a constant source of power. It comes, it goes, it varies.
- **Industrial Batteryless IoT Use Cases**
  - Everactive deploys over 10,000 batteryless sensors in the industrial space to monitor numerous pieces of equipment.
  - Motors and steam traps are examples where batteryless sensors enable continuous monitoring without maintenance.
  Transcript:
  Speaker 1
  So to give the examples wherever active has started deployments, those are in the industrial space and they deal with pieces of equipment that are highly numerous that when they're Working, it's great. But when they fail, it's a real problem. So for example, motors, there are lots of motors all over the place and many different kinds of use, use environments. And there are a large amounts of money and effort spent on trying to monitor motors and other vibrating and rotating equipment. But we and there are a lot of solutions that use batteries to monitor vibration in motors. But typically, people only deploy them on a small set of the total number of motors in a particular setting in the industrial space. With a batteryless vibration monitor, a bracket can monitor vibration essentially continuously, do fast-furrier transforms right on the device, extract frequency information And have a continuous solution for knowing exactly what's going on with that motor. And because it's batteryless, it means nobody needs to go back and maintain it later. So people will deploy them in thousands. A similar example that we've also deployed is for steam traps, which are valves in a steam distribution system that let condensate out of the system but keep steam in. Like motors, these are highly numerous. And when they fail, it's a real problem. It costs a lot of money because you're pouring steam down the drain or you're backing condensate up into the system. Fantastic.
- **Batteryless IoT Key Components**
  - To build batteryless IoT, use an ultra-low-power system on chip for efficient energy harvesting and computation.
  - Use a network that connects many devices, even in industrial environments, and delivers data to the cloud.
  Transcript:
  Speaker 1
  The ultra low power system on chip is a key piece of this. It does the energy harvesting efficiently. It does ultra low power computation right on the node efficiently. We have an always on receiver that lets the device stay in communication with the network continuously for power as low as 300 nanowatts. That's 0.0003 milliwatts compared to Bluetooth. That's like four or five milliwatts. So that's critical, but it's not enough. You know, in addition to the chip, we have technology that puts that chip together with the battery list node to allow our developers to bring their own sensors into that platform or To bring their own reputation into that platform. And then we need to have a network that can connect lots of devices and bring data back to those devices. So, ever-actives network doesn't devices for one gateway with a range over a kilometer, even in an industrial environment, and allows that data to flow backward into the cloud where It can be delivered as a data stream.
