---
draft: true
description:
socialDescription:
title: Software as a Medical Device What’s a Significant Change
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[dr-oliver-eidel]]
url: https://openregulatory.com/medical-device-significant-change/

last highlighted date: [[2024-02#20]]

## Highlights
- Bug and security fixes aren’t significant changes.
- If I could name one topic which is the most unclear and messy in medical software certifications, it might be this. Evaluating whether a change to your (certified) software as a medical device is a significant one is so subjective, it’s almost ridiculous.
- But before I continue my rant, let’s look at [MDCG 2020-3](https://ec.europa.eu/docsroom/documents/40301/attachments/1/translations/en/renditions/native) which is a guidance document on significant changes.
- Change in database structure is significant? So a migration would be a significant change? That would be a real limitation.
- ### Changes of the Intended Use
  **Not significant:**
  * Limitation of the Intended Use
  **Significant:**
  * Extension of the Intended Use
  * New user or patient population
  * Change of clinical use (anatomical site, access site or deployment methods)
- ### Software Changes
  **Not significant:**
  * Minor change: Bug fixes (corrections of errors which don’t pose a safety risk, security updates, appearances of the user interface (?), operating efficiencies (?), changes to enhance the user interface without changes in performance (?))
  * New languages, layouts
  **Significant:**
  * New or major change of operating system or any component
  * New or modified architecture or database structure, change of an algorithm
  * Required user input replaced by closed loop algorithm
  * New diagnostic or therapeutic feature, or new channel of interoperability
  * New user interface or presentation of data (medical data presented in a new format or dimensions (?))
- New channel of interoperability is significant? Just having another interface doesn’t really change things a lot in my opinion.
- in the real world, changes to the software (even major ones) were generally fine as long as the intended use remained the same and the risk analysis didn’t become worse. To me, this sounds like a good and pragmatic approach.
