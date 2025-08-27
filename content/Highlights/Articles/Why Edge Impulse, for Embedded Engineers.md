---
draft: true
description:
socialDescription:
title: Why Edge Impulse, for Embedded Engineers
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[edgeimpulse.com]]
url: https://docs.edgeimpulse.com/docs/readme/for-embedded-engineers

last highlighted date: [[2024-02#28]]

## Highlights
- **Open-source export formats:** Exported models and libraries contain both digital signal processing code and machine learning models, giving you full explainability of the code.
    - Note: what are open source formats in ml industry?
- Edge Impulse Studio and collect data from the Studio. However, as an embedded engineer, you might want to collect data from sensors that are not necessarily available on these devices. To do so, you can use the [Data forwarder](https://docs.edgeimpulse.com/docs/tools/edge-impulse-cli/cli-data-forwarder) and print out your sensor values over serial (up to 8kHz) or use our [C Ingestion SDK](https://docs.edgeimpulse.com/reference/c-sdk-usage-guide), a portable header-only library (designed to reliably store sampled data from sensors at a high frequency in very little memory).
