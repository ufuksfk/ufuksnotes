---
draft: true
description:
socialDescription:
title: Google Has Finally Dethroned ChatGPT
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Ignacio de Gregorio]]
url: https://medium.com/p/87a8f8c10d92

last highlighted date: [[2024-03#02]]

## Highlights
- Specifically, it‘s capable of processing millions of words at a time, 40-minute-long videos, or 11 hours of audio in seconds with 99% context retrieval accuracy, absolutely unheard of in the field until today.
- Simple, instead of forcing the model to learn a global map of all possible inputs to all possible outputs, you create ‘experts’, smaller neural networks that focus on specific input regions.
- If you’re interested in knowing how this is done, check Mistral’s paper [[Mistral AI]]
- Quantization reduces the precision of the model’s parameters to save up memory. For instance, for a 50-billion-parameter model at float32 precision (32 bits per parameter, or 4 bytes), your weights file occupies 200 GB, needing at least 3 state-of-the-art 80GB-GPUs just to host the model.
- In Transformers, the entire model runs for every prediction, thus requiring to be stored in RAM. Some techniques like Flash LLMs by [[Apple]] can help store some parts of the model in flash memory.
- Some suspect that [[Google]] has also introduced a less compute-intensive variation of the attention mechanism, although no confirmation has been made on this.
