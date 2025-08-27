---
draft: true
description:
socialDescription:
title: Esp-IdfExamplesSystemOta at Master · EspressifEsp-Idf
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
url: https://github.com/espressif/esp-idf/tree/master/examples/system/ota
about [[Espressif]] and [[ESP-IDF]]
last highlighted date: [[2024-02#21]]

## Highlights
- The ESP-IDF offers two methods to perform Over The Air (OTA) upgrades:
  Using the native APIs provided by the app_update component.
  Using simplified APIs provided by the esp_https_ota component, which provides functionality to upgrade over HTTPS.
- If you want to rollback to the factory app after the upgrade (or to the first OTA partition in case the factory partition does not exist), run the command idf.py erase_otadata. This restores the ota_data partition to its initial state.
- Make sure to run "idf.py erase-flash" after making changes to the partition table.
