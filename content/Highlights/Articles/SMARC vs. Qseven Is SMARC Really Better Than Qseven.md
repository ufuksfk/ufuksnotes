---
draft: true
description:
socialDescription:
title: SMARC vs. Qseven Is SMARC Really Better Than Qseven
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[kontron.com]]
url: https://www.kontron.com/en/blog/embedded/smarc-vs-qseven-smarc-better-qseven

last highlighted date: [[2024-04#10]]

## Highlights
- **Qseven’s** connector is the **MXM2** connector, a connector that was used for graphic cards in high end laptops. Nowadays this is normally done by the **MXM3** connector which is used by **SMARC**. How is the availability of the MXM2 connector secured, when it is not used in its original purpose? This question should be answered by the Qseven manufacturers.
  Regarding connector availability there is higher security in the newer MXM3 connector which is used for **SMARC**:
- ![](https://www.kontron.com/blog/2014/tabelle1.png)
- Compared to **Qseven**, **SMARC** also offers an additional so-called “*Alternate Function Block*”. These 20 specially defined pins allow flexibility between modules. They can be used e.g. as MIPI DSI interface, USB 3.0, MOST, a 2nd Gigabit Ethernet or an industrial Fieldbus interface. The interchangeability is ensured by defined electrical characteristics (some are differential, some are single ended) of these pins.
    - Note: they have alternate function block pins!
- More and more applications need the possibility to use live pictures to connect to the surrounding world: Logistic systems where goods need to be scanned, face and gesture detection or self-controlled vessels. In systems with Qseven these camera implementations cannot be connected over the module connector, but need, if possible at all, an additional flat foil connection to the module.
  **SMARC** has 2 camera interfaces defined on the connector and therefore cameras can be integrated easily on the carrier board. So again regarding interfaces, **SMARC** is the winner:
    - Note: camera connectors
