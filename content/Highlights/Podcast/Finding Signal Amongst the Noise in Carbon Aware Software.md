---
draft: true
description:
socialDescription:
title: Finding Signal Amongst the Noise in Carbon Aware Software
tags:
- highlight/podcasts
date: 2025-03-07
modified: 2025-08-21
---
publisher: [[Environment Variables]]
published_date: [[2025-01#09]]

# Note
 * Carbon intensity signals play a crucial role in carbon-aware optimizations, with average and marginal signals offering different perspectives on grid emissions.

* Spatial shifting dominates carbon reduction efforts, with location playing a significant role in achieving lower carbon emissions.
* Combining spatial and temporal shifting does not necessarily double the benefits, as spatial shifting tends to have a more significant impact on carbon reduction.


## Highlights
* [[2025-01#10]] 13:01  If you want to schedule based on marginal carbon intensity signal, you wouldn’t do anything because it’s flat. You can just place the workload wherever you want. But if you want to schedule the workload based on the average signal, you’ll be like, I would place my workload at this particular time slot because it had the lowest carbon intensity signal during the day.

* [[2025-01#10]] 12:30  Tammy recently authored the paper on the Limitations of Carbonal Air, Temporal and Spatial Workload Shifting in the Cloud, which examines how shifting computing workloads across time and space can help cut emissions.

* [[2025-01#10]] 12:39  With that, the savings from 96% global reduction drops to 51%. Okay, not everyone can go to Sweden.

* [[2025-01#10]] 12:44  So everyone in the world can schedule their workload if they know about the curve. Perfect forward knowledge. Yeah, yeah, perfect. Perfect knowledge for one year ahead. And with that, we look at the extreme case, the most ideal case, where the workload is a unit job, one hour job, to understand what is the best case scenario for temporal shifting.

* [[2025-01#10]] 15:22  But like, Iceland is usually green because it's running on geothermal, which is like pretty standard. Like it's, it's steady. And even when you look at like, say Sweden, for example, there's like a wind and everything like that, but there's lots of hydro and stuff like that. So again, it's not nearly as spiky as, hey, Germany, where we are the land of like, wind. We're land of coal and solar. We have lots, lots of coal, which is high carbon intensity, and lots and lots of solar, which is very, very low intensity. And flicking back and forth between these things means that we might have big swings, but on average it's not particularly low compared to Iceland or Sweden,

* [[2025-01#10]] 15:20  Things are only obvious with. When you look at it like that. And one thing you shared with me before we spoke about this was that some of this stuff is actually like, if people wanted to kind of explore some of these calculations. Is this online somewhere? Is it like a. Is there like a GitHub repo or something where you can like poke around at some of these things? Yeah. So all the simulations in this paper, it's open source, so please check my lab website, my lab GitHub, for the simulations. Okay, cool. All right, I think I. We've got the link here so that this is from. So there's literally a repo called [[decarbonization]] potential. That's the one you're referring to here, right? On GitHub. Yes, that's correct.

* [[2025-01#10]] 15:22  So this paper came from the fact that, okay, people been suggesting let's shift the workload through time, let's shift the workload to different locations, but we never actually agree on which carbon intensity signal to use for carbon aware optimization. So as the title suggested, there are two types of carbon intensity signals that are mainly used, namely average carbon intensity signal and marginal carbon intensity signal.

* [[2025-01#10]] 15:22  So for average carbon intensity signal, just think of it as a snapshot of the grid at that point in time. Right. And the way it's calculated is the weighted average of carbon emissions weighted by their production. Okay, so if I just check, just if I want to start you there, so make sure I keep keeping up with you. So there's two ways you can measure carbon intensity, like how green the electricity is.

* [[2025-01#10]] 15:22  And this first one, this average one is basically saying, well, I've got maybe two coal fired power generators and one wind farm. So therefore I'll apply double the weighting of the coal versus one of the wind farm. That's kind of what, that's a simplified version, but that's essentially how you work out an average figure. Right, right, right. But marginal carbon intensity signal is different.

* [[2025-01#10]] 15:22  The way it's calculated is the carbon intensity with respect to the change in demand. So let's say just now you said you have two wind farms and one coal. But the next unit of demand is going to be served by gas generator. So then the marginal carbon intensity signal is the current intensity signal of that of the gas generator. Ah, I see.

* [[2025-01#10]] 15:23  The fact that if you follow one signal as a scheduling signal, you might end up in more carbon emission based on the perspective of the other signal. Yeah. So it turns out like you cannot just follow one signal and hoping that you will do well based on the other signals perspective as well

* [[2025-01#10]] 15:21  So I think we need to move beyond the static signal and instead maybe look into other characteristics to take into consideration when doing carbon aware optimization. Maybe in future direction, maybe we would agree on some other signal that captures the long term impact of the grid, like average carbon intensity signal and the current, like the instantaneous change in carbon intensity, like marginal. So yeah, apart from optimizing for carbon efficiency as a community, I think everyone should keep in mind about like we, we need a better metric to capture this carbon emission.

* [[2025-01#10]] 15:21  trying to understand the environmental footprint of software. I think I understand that there's a whole nother set for this and you really opened my eyes to this. Tell me, if people are interested in this field, are there any other projects or work that you've read about recently that you'd like to draw people's attention to? Yeah, I think if you look at Carbon Scaler, I think that's one of the thing. I recommend people to check it out.

