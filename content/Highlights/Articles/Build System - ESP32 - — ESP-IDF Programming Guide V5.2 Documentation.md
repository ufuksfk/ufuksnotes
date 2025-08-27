---
draft: true
description:
socialDescription:
title: Build System - ESP32 - — ESP-IDF Programming Guide V5.2 Documentation
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[docs.espressif.com]]
url: https://docs.espressif.com/projects/esp-idf/en/stable/esp32/api-guides/build-system.html

last highlighted date: [[2024-02#26]]

## Highlights
- [[CMake]] will usually handle circular dependencies automatically by repeating the component library names twice on the linker command line. However this strategy doesn't always work, and the build may fail with a linker error about "Undefined reference to ...", referencing a symbol defined by one of the components inside the circular dependency. This is particularly likely if there is a large circular dependency, i.e., A > B > C > D > A.
