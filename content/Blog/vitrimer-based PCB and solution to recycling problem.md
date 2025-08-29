---
draft: false
description:
socialDescription:
title: vitrimer-based PCB and solution to recycling problem
tags:
  - blog/recycling
date: 2025-08-24
modified: 2025-08-28
---
We are hopefully all on the same page that e-waste is now a big problem. And it is growing problem of humanity.

Or maybe not. I don't know. Personally, I like to keep my old stuffs as a memoir, I barely remember myself throwing electronics to garbage. Even If I do, it is probably not 8kg per year. Let's say in every 15 years I need to get rid of my white appliances.

Refrigerator: ~100 kg

Washing Machine: ~ 70 kg

Dishing Machine: ~50 kg

Oven: ~50 kg

Microwave: ~15 kg

285 kg / 15 years = 19 kg. Let's say average family is 3 people. 6 kg per person per year.

Hmm..

And  I forgot batteries and toys are also in the same pocket. Now I started to feel guilty about that e-waste problem.

OK. I probably have more than 8 kg per year. Found guilty!

# Some eye-catching statistics about e-waste
I don't want this blog post to be a normal SEO driven blog post. But even back in the last century, to catch reader attention, it is always nice to talk with numbers :) So, let me introduce you some numbers about this specific problem of humanity.

According to United Nations, [^1] around 7.8 kg per capita e-waste is generated at 2022. That means 62 billion kg yearly, but that number probably doesn't mean much for an individual - yet only **22.3%** of it was formally collected and recycled.

While former collection numbers are better in global north, e-waste per capita is way less in south asia or africa.

The economic value of the metals contained in the e-waste generated globally in 2022 is estimated at USD 91 billion.
Currently, e-waste management generates USD 28 billion worth of secondary raw materials out of the maximum of USD 91 billion. Most losses occur due to incineration, landfilling or substandard treatment. The current secondary raw material production avoids extraction of 900 billion kg of ore.
[^1] 

In 2019, the world generated **53.6 million metric tons of e-waste** (Global E-Waste Monitor). That’s like throwing away 1,000 laptops every second.

---
So, I don't know what is your profession but I hope I can do something about it. At least we can learn more about it and try to vocalize that problem as much as we can. Just for that reason, I started to take an online course from edX DelftX: Designing Electronics for Recycling in a Circular Economy[^2]. While watching that course, I realized plastic as a material is kind of biggest issue while grinding electronics waste.

![[Pasted image 20250826115118.png]]
_​​Baldé, C.P., R. Kuehr, T. Yamamoto, R. McDonald, E. D’Angelo, S. Althaf, G. Bel, et al. 2024. The Global E-waste Monitor 2024. Geneva/Bonn: International Telecommunication Union (ITU) & United Nations Institute for Training and Research (UNITAR)._

For the first couple of weeks, they focused on plastic as a case material, that might be another blog post topic for me. But today, I would like to have a quick journey with you to the very core of the electronics: ==Electronics circuit themselves!==

![[Pasted image 20250826105406.png]]
Source: https://www.wastetrade.com/sv/resources/recycling/e-waste-recycling-and-management/

Our usual suspect is named FR-4.
# What is FR-4

FR stands for flame retardant. FR-4 is popular because it has the right mix of electrical, thermal, and mechanical properties that make it a great “default” choice for electronics. In plain words, it has:
* **low moisture absorption.** Meaning it won’t swell or get ruined by a bit of water.
* **stable dielectric constant.** Something technical, but basically means it is cheap and easy to use them as substrate. We can roughly be sure that it is going to be flat dielectric constant all around the pcb.
* good electric insulation. Means you can safely put copper traces with FR-4 in between. No way to have  short circuit between them in normal circumstances.
* **Mechanical stiffness.** Your board doesn’t bend like cardboard. It can actually do that If it is too thin to 0.4mm. But it is out of the topic for now :)
* **Heat resistance.** Crucial, because the way we still connect electronics is old-school: we literally melt solder to attach components.
And that last part hit me — after all this time, we’re still basically using **tiny molten metal puddles** to hold circuits together. It works, but think about the carbon footprint of heating every single joint to a few hundred degrees. That’s not small when you scale it to billions of devices.


Technically, FR-4 is just **glass fiber cloth soaked in epoxy resin and pressed flat**. But at the end of the day, it’s plastic. And here’s the catch: it’s a **thermoset plastic**. That’s why it’s strong and durable… but also why it’s a nightmare to recycle. Once it’s cured, it won’t melt or reshape. End of life? You can grind it, you can burn it, but you can’t really recycle it.

That can be later another blog post but here we should quickly put a side info: What makes plastics recyclable? It is a bit material science, but basically high school chemistry that everyone can basically understand. But I am skipping to describe it in detail to stay in context. You can actually jump to that side note from down below.

# 2 types of plastics
There are mainly 2 types of plastics. 

Most of the daily plastics we know - bottles, packaging, toys -  is **thermoplastics**. That means you can melt it down with heat and mold it again. Simple, right? Well, not that easy. Each time you melt and reform it, the plastic loses a bit of quality. Because of basic hight school chemistry. Even the “good ones” are usually not recyclable more than five or six times. And almost every recycling loop is a **downstream** step — the plastic comes back as something lower-grade. Think: not another shiny bottle, but maybe a structural material, a park bench, or filler for construction.

And, you can't easily find a pure plastic without any additive to make it shiny in electronics industry.

Other types is **thermosetting** plastics. One well known example is epoxy. Once you build it, it is chemically very hard to reverse it. Sure, with clever chemistry you can sometimes break it apart, but in “money language” that’s way too expensive.

Guess what! ==FR-4 is also under the group of thermoset family.== If you imagine yourself recycling an old electronics, even if you recycle all the plastics, you ends up having that green plates: printed circuit boards a.k.a PCB.

# Do we have a solution?

We’ve been using FR-4 for so long that the whole electronics industry basically married it. Every design tool, every factory, every soldering line — all built around this one material. So changing it is not like swapping batteries. It’s more like asking the entire world to stop eating bread and figure out a new breakfast.

But yesterday I learned there are some efforts to shake things up. Instead of epoxy + glass fiber, researchers are experimenting with new substrate materials — ones you can actually recycle. Imagine melting down an old circuit board, pulling out the copper traces and chips, and starting fresh.
## New player joined game: Vitrimers
Back in 2015, in France, scientists introduced a new type of plastic called **vitrimers**. One-line summary: _they behave like thermosets (strong, rigid, heat resistant) but they’re actually recyclable like thermoplastics._ Basically the best of both worlds.

And that’s why they look like a great candidate to end the old FR-4 tyranny.

Fast forward to today — teams at the **University of Washington** together with **Microsoft Research** are building actual **vitrimer-based PCBs** (they call them _vPCBs_). These are not just lab curiosities; they’ve already made boards that transmit Wi-Fi signals, survive soldering, and still get recycled afterwards. Heat them, separate the layers, recover the copper, glass fibers, and the polymer — and reuse them again. They claim recovery rates like **98% for the polymer and 100% for the glass fibers.** That’s basically unheard of in the e-waste world.

Of course, it’s still early days. These vPCBs are coming out of research labs, not your local electronics store. But the fact that people are working on this — and that big players like Microsoft are paying attention — makes me hopeful. Maybe in a few years, when I finally throw out that 100 kg refrigerator, the little green board inside it won’t be doomed to landfill anymore.

# Some questions left

Can we delegate e-waste seperation process of e-waste by educating public? 
	At least as an engineer, I believe I can do that for free as a evening activity with my son. But, it is probably hard to educate public to do that safely. There can be some hazardous chemicals.. Nevermind, actually.

Would you be willing to pay a little more for a phone or a laptop if you knew its circuit boards could be fully recycled? 
	It is economical question, but probably early adapters suppose to pay more for that vPCB's.

Is it really big deal in e-waste. I mean percentage of pcb in e-waste is missing here in this blog.
	They are probably around 5% of the total mass of e-waste. But the thing is most of the precious metals are either soldered to it or already in it.
		Quick side note: We are using gold in PCB's :) Not everytime but sometimes. But not that much.

In 500 years, will future archaeologists dig up our landfills and call this the “age of green PCBs”?
	That would be cool futuristic solarpunk story.

Besides metals and rare metal minerals in e-waste, does it really matter to reuse plastic substrate?
	I keep asking myself. What is going to happen after we completely find a plastic eating bacterias. Viable, environmental solution to all of our pains?

Last disclaimer. This blog post is mainly my attempt to organize my thoughts and learnings. I can delete or update it however I want. I am trying to fact check myself, but I just wrote it with  a couple of hours of effort.

But thank you If you read it so far.
# Internal links
[[e-waste]]
[[thermosetting plastics vs thermoplastics]]
 [[Plastic]] [[Vitrimers]]
[[(PCB) Printed Circuit Board]]
[[United Nations]]
## Internal Notes
[[Can we delegate seperation process of e-waste by educating public]]
[[Don't we have any other chemical methods instead of soldering components]]
[[What makes plastic recyclable]]
[[Numbers related to e-waste]]
## Internal organization links
[[Microsoft Research]]
# References
https://arxiv.org/pdf/2308.12496 - their research article.
https://vpcb.cs.washington.edu/ - To read about their story.
https://www.eenewseurope.com/en/researchers-address-e-waste-with-recyclable-healable-circuit-boards/ - Further reading
https://www.youtube.com/watch?v=BjMNgSB8ufs - The podcast they talked about it. And how I learned about it.
[Spotify](https://open.spotify.com/episode/5R27LIPxAMMEF3HQWOvLSh) [Apple Podcast](https://podcasts.apple.com/il/podcast/collaborators-sustainable-electronics-with-jake-smith/id1318021537?i=1000661906954)

[^1]: https://ewastemonitor.info/wp-content/uploads/2024/12/GEM_2024_EN_11_NOV-web.pdf

[^2]: https://www.edx.org/learn/circular-economy/delft-university-of-technology-designing-electronics-for-recycling-in-a-circular-economy
