---
draft: true
description:
socialDescription:
title: Engineering the First Fitbit The Inside Story
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
url: https://spectrum.ieee.org/fitbit

last highlighted date: [[2024-08#14]]
A good summary of [[Fitbit]] starting years.
## Highlights
- But back to that “aha moment.” Park quickly called his friend and colleague Eric Friedman. In 2002, the two, both computer scientists by training, had started a photo-sharing company called HeyPix, which they sold to CNET in 2005. They were still working for CNET in [[2006]]
- Park and Friedman weren’t trying to build the first step counter—mechanical pedometers date back to the 1960s. They weren’t inventing the first smart activity tracker— [BodyMedia](https://bodymedia.com/), a medical device manufacturer, had in 1999 included accelerometers with other sensors in an armband designed to measure calories burned.
- They hired [NewDealDesign](https://www.newdealdesign.com/) to figure out some of these details.
- “We wanted to start with something familiar to people,” Park says, “and people tended to clip pedometers to their belts.” So a clip-on device made sense. But women generally don’t wear belts.
- They hid a low-resolution monochrome OLED display behind a continuous plastic cover, with the display lighting up only when you asked it to. This choice helped give the device an impressive battery life.
  ![A black rectangular object displaying a small blue flower and clipped onto light blue fabric ](https://spectrum.ieee.org/media-library/a-black-rectangular-object-displaying-a-small-blue-flower-and-clipped-onto-light-blue-fabric.gif?id=53100713&width=1000&quality=85)
  The earliest Fitbit devices used an animated flower as a progress indicator.
- Fortunately, they knew just whom to call. Friedman’s father, Mark, had for years been working to develop a device for use in nursing homes, to remotely monitor the position of bed-bound patients. Mark’s partner in this effort was Randy Casciola, an electronics engineer and currently president of Morewood Design Labs.
- “Figuring out the right balance of battery life, size, and capability kept us occupied for about a year,” Park says.
  ![A black Fitbit sits vertically in a square stand with a wire coming out. The screen on the device reads \u201cBATT 6%\u201d ](https://spectrum.ieee.org/media-library/a-black-fitbit-sits-vertically-in-a-square-stand-with-a-wire-coming-out-the-screen-on-the-device-reads-u201cbatt-6-u201d.png?id=53100764&width=1000&quality=85)

  The Fitbit prototype, sitting on its charger, booted up for the first time in December 2008.
- After deciding to include a radio transmitter, they made a big move: They turned away from the Bluetooth standard for wireless communications in favor of [the ANT protocol](https://developer.garmin.com/ant-program/overview/), a technology developed by Garmin that used far less power. That meant the Fitbit wouldn’t be able to upload to computers directly. Instead, the team designed their own base station, which could be left plugged into a computer and would grab data anytime the Fitbit wearer passed within range.
- “We couldn’t use USB,” Park says. “It just took up too much volume. Somebody actually said to us, ‘Whatever you do, don’t design a custom charging system because it’ll be a pain, it’ll be super expensive.’
- Most of the electronics they used were off the shelf, including a 16-bit Texas Instruments MSP430 microprocessor, and 92 kilobytes of flash memory and 4 kb of RAM to hold the operating system, the rest of the code, all the graphics, and at least seven days’ worth of collected data.
- “You think counting steps is easy, but let’s say you do three steps. One, two, three. When you bring your feet together, is that a step or is that the end? It’s much easier to count 1,000 steps than it is to do 10 steps. If I walk 10 steps and am off by one, that’s a glaring error. With 1,000, that variance becomes noise.”
- That day, some 2,000 preorders poured in. And Fitbit closed a $2 million round of venture investment the next month.
- “Pushing baby strollers was an issue,” because the wearer’s arms aren’t swinging, Park says. “So one of our guys put an ET doll in a baby stroller and walked all over the city with it.”
- The problem, Park eventually figured out, occurred when the two halves of the Fitbit case were ultrasonically welded together. In previous syncing tests, the cases had been left unsealed. The sealing process pushed the halves closer together, so that the cable for the display touched or nearly touched the antenna printed on the circuit board, which affected the radio signal. Park tried squeezing the halves together on an unsealed unit and reproduced the problem.
- ![Two photos. One photo shows 3 men working in a lab wearing cleanroom suits. One man is seated and handling electronic components, and the others stand observing. The other photo shows a row of six black rectangular devices with green circuit boards hanging out of them ](https://spectrum.ieee.org/media-library/two-photos-one-photo-shows-3-men-working-in-a-lab-wearing-cleanroom-suits-one-man-is-seated-and-handling-electronic-components.png?id=53100989&width=1000&quality=85)

  Getting the first generation of Fitbits into mass production required some last-minute troubleshooting. Fitbit cofounder James Park [top, standing in center] helps debug a device at the manufacturer shortly before the product’s 2009 launch. Early units from the production line are shown partially assembled [bottom]. James Park
- ![Two photos. One photo shows 3 men working in a lab wearing cleanroom suits. One man is seated and handling electronic components, and the others stand observing. The other photo shows a row of six black rectangular devices with green circuit boards hanging out of them ](https://spectrum.ieee.org/media-library/two-photos-one-photo-shows-3-men-working-in-a-lab-wearing-cleanroom-suits-one-man-is-seated-and-handling-electronic-components.png?id=53100989&width=1000&quality=85)
- “I thought, if we could just push that cable away from the antenna, we’d be okay,” Park said. “The only thing I could find in my hotel room to do that was toilet paper. So I rolled up some toilet paper really tight and shoved it in between the cable and the antenna. That seemed to work, though I wasn’t really confident.”
- It turned out the problem came from Casciola’s design of the system-reset trigger, which allowed users to reset the device without a reset button or a removable battery. “Inevitably,” Casciola says, “firmware is going to crash. When you can’t take the battery out, you have to have another way of forcing a reset; you don’t want to have someone waiting six days for the battery to run out before restarting.”
- “If you clipped the tracker onto sweaty clothing—remember, sweat has a high salt content—a very tiny current would flow,” says Casciola. “It was just fractions of a microamp, not enough to cause a reset, but enough, over time, to cause greenish corrosion.”
- Evolution happened quickly, particularly in the way the device transmitted data. In 2012, when Bluetooth LE became widely available as a new low-power communications standard, the base station was replaced by a small Bluetooth communications dongle. And eventually the dongles disappeared altogether.
- The impetus came from some users’ desire to better track their sleep. The Fitbit’s algorithms allowed it to identify sleep patterns, a design choice that, Park says, “was pivotal, because it changed the device from being just an activity tracker to an all-day wellness tracker.”
- “My father, who turned 80 on July 5, is fixated on his step count. From 11 at night until midnight, he’s in the parking garage, going up flights of stairs. And he is in better shape than I ever remember him.”
- Meanwhile, a cultural phenomenon was underway. In the mid-2000s, yellow [Livestrong](https://livestrong.org/) bracelets, made out of silicone and sold to support cancer research, were suddenly everywhere. Other causes and movements jumped on the trend with their own brightly colored wristbands. By early 2013, Fitbit and its competitors Nike and Jawbone had launched wrist-worn fitness trackers in roughly the same style as those trendy bracelets. Fitbit’s version was called the Flex, once again designed by NewDealDesign.
- “We didn’t want to replace people’s watches,” Park says. The technology wasn’t yet ready to “build a compelling device—one that had a big screen and the compute power to drive really amazing interactions on the wrist that would be worthy of that screen. The technology trends didn’t converge to make that possible until 2014 or 2015.”
- The tap part of the interface, though, was “possibly something we didn’t get entirely right,” Park concedes. It took much fine-tuning of algorithms after the launch to better sort out what was **not** tapping—like applauding. Even more important, some users couldn’t quite intuit the right way to tap.
- Fitbit went public in [[2015]] at a valuation of $4.1 billion. In [[2021]] [[Google]] completed its $2.1 billion purchase of the company and absorbed it into its hardware division. In April of this year, Park and Friedman left Google. Early retirement? Hardly. The two, now age 47, have started a new company that’s currently in stealth mode.
