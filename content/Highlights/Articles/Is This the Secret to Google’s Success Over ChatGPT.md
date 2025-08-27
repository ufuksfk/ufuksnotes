---
draft: true
description:
socialDescription:
title: Is This the Secret to Google’s Success Over ChatGPT
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Ignacio de Gregorio]]
url: https://medium.com/p/b2a545f39ad5

last highlighted date: [[2024-03#02]]

## Highlights
- And that secret might be Ring Attention, a discovery by researchers at Berkeley University as a new way of running LLMs that enables efficient distribution to maximize their raw power and reach new, unreached heights.
- It’s important to note that models like ChatGPT and Gemini are autoregressive decoders. In layman’s terms, words can only pay attention to words that appear previously in the sequence.
- NVIDIA, the company that owns 90+ market share of the GPU market has added, since the beginning of 2024, the entire value of Tesla to its valuation, more than 700 billion dollars.
- But with Ring Attention, the GPU paradigm might change completely.
- The memory issue is so relevant that it completely overtakes the whole process, meaning that LLMs, in inference (execution time) are ‘memory bound’, meaning that GPUs saturate on memory before they saturate their compute accelerators, meaning that GPUs are often ‘idle’ computationally speaking
- Ring Attention proposes a new way of distributing the computation of Transformers across GPUs.
- Imagine you had to reread all the previous pages in a book for every new word you want to read.
- That’s how Transformers like ChatGPT or Gemini read.
- As long as the GPU takes longer to process its block computations than sending/receiving the K and V vectors from the next/previous GPUs, this communication among GPUs does not cause a temporal overhead, as the GPU is occupied with its own calculations during transfer.
- Additionally, the sequence length scales linearly to the GPU count, allowing it to, theoretically, increase to infinity.
