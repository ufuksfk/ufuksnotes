---
title: "Calculating the Environmental Footprint of AI at Google"
draft: true
tags:
  - highlight/articles
---
author: [[Amin Vahdat]]
url: https://cloud.google.com/blog/products/infrastructure/measuring-the-environmental-impact-of-ai-inference
last highlighted date: [[2025-W35#6]] 2025-08-30
published date: [[2025]]

## Highlights
- AI is unlocking scientific breakthroughs, improving healthcare and education, and could add trillions to the global economy. Understanding AI’s footprint is crucial, yet thorough data on the energy and environmental impact of AI inference — the use of a trained AI model to make predictions or generate text or images — has been limited. As more users use AI systems, the importance of inference efficiency rises.
- Using this methodology, we estimate the median Gemini Apps text prompt uses 0.24 watt-hours (Wh) of energy, emits 0.03 grams of carbon dioxide equivalent (gCO2e), and consumes 0.26 milliliters (or about five drops) of water1 — figures that are substantially lower than many public estimates. The per-prompt energy impact is equivalent to watching TV for less than nine seconds.
- over a recent 12 month period, the energy and total carbon footprint of the median Gemini Apps text prompt dropped by 33x and 44x, respectively, all while delivering higher quality responses.
- We developed a comprehensive approach that considers the realities of serving AI at Google’s scale, which include:
- **Full system dynamic power:** This includes not just the energy and water used by the primary AI model during active computation, but also the actual achieved chip utilization at production scale, which can be much lower than theoretical maximums.
- **Idle machines:** To ensure high availability and reliability, production systems require a degree of provisioned capacity that is idle but ready to handle traffic spikes or failover at any given moment. The energy consumed by these idle chips must be factored into the total energy footprint.
- **CPU and RAM**: AI model execution doesn't happen solely in ML accelerators like TPUs and GPUs. The host CPU and RAM also play a crucial role in serving AI, and use energy.
- **Data center overhead:** The energy consumed by the IT equipment running AI workloads is only part of the story. The infrastructure supporting these computations — cooling systems, power distribution, and other data center overhead — also consumes energy. Overhead energy efficiency is measured by a metric called Power Usage Effectiveness (PUE).
- **Data center water consumption**: To [reduce energy consumption and associated emissions](https://blog.google/outreach-initiatives/sustainability/our-commitment-to-climate-conscious-data-center-cooling/), data centers often consume water for cooling. As we optimize our AI systems to be more energy-efficient, this naturally decreases their overall water consumption as well.
- We design models with inherently efficient structures like [Mixture-of-Experts (MoE)](https://arxiv.org/abs/1701.06538) and [hybrid reasoning](https://developers.googleblog.com/en/start-building-with-gemini-25-flash/). MoE models, for example, allow us to activate a small subset of a large model specifically required to respond to a query, reducing computations and data transfer by a factor of 10-100x.
- Our latest-generation TPU, [Ironwood](https://blog.google/products/google-cloud/ironwood-tpu-age-of-inference/), is 30x more energy-efficient than our first publicly-available TPU and far more power-efficient than general-purpose CPUs for inference.
- **Ultra-efficient data centers:** Google’s data centers are among the industry’s most efficient, operating at a fleet-wide average [PUE of 1.09](https://datacenters.google/efficiency/).
- *1. A point-in-time analysis quantified the energy consumed per median Gemini App text-generation prompt, considering data from May 2025. Emissions per prompt was estimated based on energy per prompt, and applying Google’s 2024 average fleetwide grid carbon intensity. Water consumption per prompt was estimated based on energy per prompt, and applying Google’s 2024 average fleetwide water usage effectiveness. These findings do not represent the specific environmental impact for all Gemini App text-generation prompts nor are they indicative of future performance. 
  2. The results of the above analysis from May 2025 were compared to baseline data from the median Gemini App text-generation prompt in May 2024. Energy per median prompt is subject to change as new models are added, AI model architecture evolves, and AI chatbot user behavior develops. The data and claims have not been verified by an independent third-party.*
