---
draft: true
description:
socialDescription:
title: The Energy Footprint of Humans and Large Language Models
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Logan Kugler]]
url: https://cacm.acm.org/blogcacm/the-energy-footprint-of-humans-and-large-language-models/

last highlighted date: [[2024-10#15]]

## Highlights
- It is relatively easy to look at these costs in terms of kilowatt-hours (kWh), but it is hard to compare that to the alternative use of human time.
- To write a text like this one, the process involves a human and a computer running a word processor. If an LLM is involved in the process to make it faster, are we using more energy or, on the contrary, saving resources?
- we can generously assume the consumption of 100 calories per hour of writing [2], about 0.12 kWh.
- If we consider the data on energy consumption per capita, the values are much more significant. In the U.S. it is close to 80,000 kWh per person per year (the range in Europe is from 25,000 to close to 100,000 in the north). Restricting the analysis to electricity, in the U.S. it is around 12,500 kWh per person per year [3]. Assuming an 8-hour workday and considering 260 workdays per year brings the annual energy cost of one person’s hour of daily work to around 6 kWh[[a]](https://cacm.acm.org/blogcacm/the-energy-footprint-of-humans-and-large-language-models/#_ftn1).
- Measurements with Llama 65B reported around 4 Joules per output token [4]. This leads to 1,332 Joules for 333 tokens, about 0.00037 kWh. Even lower energy costs can be obtained by running locally smaller models (I was able to use a local Meta Llama 3 8B model to generate a 250-word essay in 20 seconds on an Apple M3, using less than 200 Joules).
- Considering the 0.00037 kWh of writing 250 words in 20 seconds, our body will use more than 300 times that amount and take one hour.
- Humans also accrue training costs. If we grossly simplify it, in terms of electricity use, we can approach that value by considering a 20-year-old writer who, if raised in the U.S., probably used close to 250,000 kWh of electricity in his/her 20 years of life.
