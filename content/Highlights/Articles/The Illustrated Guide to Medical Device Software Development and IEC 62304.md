---
draft: true
description:
socialDescription:
title: The Illustrated Guide to Medical Device Software Development and IEC 62304
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[vicky.taylor]]
url: https://medicaldevicehq.com/articles/the-illustrated-guide-to-medical-device-software-development-and-iec-62304/

last highlighted date: [[2024-04#08]]

## Highlights
- “A medical device is any instrument, apparatus, appliance, software, material, or other article intended for use in the diagnosis, prevention, monitoring, treatment, or alleviation of disease or injury. It must achieve its intended purpose primarily through physical or mechanical means, not by pharmacological, immunological, or metabolic means.”
    - Note: definition of medical device in MDR
- Here are a few examples of medical device software:
  • Pacemaker programming software (likely an accessory to pacemaker software, can be SiMD or SaMD)
  • Insulin pump control software (typically SiMD or embedded software)
  • Diagnostic imaging software (likely SaMD software using images from other medical devices)
  • Electronic health record systems (SaMD software, depending on regulations, it might not be a medical device)
  • Telemedicine software platforms (probably SaMD running on generic hardware platforms)
    - Tags: [[Notebook/Pages/medical software]]
    - Note: examples of md software
- The IEC 62304 standard applies to:
  • Medical devices with embedded software, and
  • Standalone software — known as Software as a Medical Device (SaMD).
    - Tags: [[IEC 62304]]
- In the Therac-25 case, a main issue was identified within its control software, which was riddled with numerous glitches. One critical glitch was a ‘race condition’ that happened when the timing or sequence of operations led to a hazardous situation.
    - Note: therac-25 case
- Similarly, if you have a software-based requirements management system, you may not have to create large amounts of paper documents.
- ”This standard does not prescribe the name, format, or explicit content of the documentation to be produced. This standard requires documentation of TASKS, but the decision of how to package this documentation is left to the user of the standard.”
- IEC 82304-1 a product standard for health software (applicable to SaMD)
- IEC 61010-1 on electrical safety (equipment)
- Having a [quality management system (QMS)](https://medicaldevicehq.com/articles/the-illustrated-guide-to-implementing-and-maintaining-a-medical-device-quality-management-system/) is a requirement of the IEC 62304. The most common standard used to establish the QMS would be the ISO 13485.
- ![](https://medicaldevicehq.com/wp-content/uploads/2024/01/Medical-device-software-and-risk-management-1.jpg)
- Software of unknown provenance, (SOUP) is software **component** that is not developed for use in medical devices but that you want to include in a medical device software system.
- [Using SOUP in medical devices](https://medicaldevicehq.com/articles/managing-and-documenting-soup-and-ots-in-medical-device-software/) requires [risk analysis](https://medicaldevicehq.com/articles/how-to-work-with-medical-device-risk-management/) and a robust software design. The purpose is to ensure that the reliability of the SOUP components won’t compromise the medical devices’ overall safety, performance, and efficacy.
- In the US, the FDA term Off-The-Shelf (OTS) is commonly used. The definitions are similar but not identical.
    - Note: difference between SOUP and OTS (off the shelf)
- ![](https://medicaldevicehq.com/wp-content/uploads/2024/01/Legacy-software-1.jpg)
    - Tags: [[IEC 62304]]
    - Note: how to get legacy software complied with iec 62304
- Impact assessments of security risks are often done against CIA, which is NOT the Central Intelligence Agency from the US, but:
  • Confidentiality – how to protect sensitive information, for example patient data.
  • Integrity – how to ensure a device is safe to use in case of a security breach.
  • Availability – how to ensure continued services delivery in case of a hacker attack.
    - Tags: [[cybersecurity]] [[Notebook/Pages/medical software]] 
- ![](https://medicaldevicehq.com/wp-content/uploads/2024/01/IEC-62304-and-IEC-81001-5-1-1.jpg)
- ‘Software items’ are essentially subsets of the software system. They are the individual building blocks that combine to form the software system. Each software item has a specific role in the system, much like “The Brickman” pieces below coming together to form a complete character.
- Finally, ‘software units’ are even smaller, more granular components than software items. Software units represent the smallest testable parts of the software – the basic building blocks that make up the larger pieces (items) of ”The Brickman”.
- Unit verification is required for class B and C while there are no such requirements for class A software.
- Detailed design documentation is required for class C but not for class A and B.
- The software safety classification is based on the potential **injury** the software can contribute to and can be summarised as follows:
  • Class A: No injury
  • Class B: Non-serious injury
  • Class C: Serious injury or death
    - Note: how to classify medical software
- ![](https://medicaldevicehq.com/wp-content/uploads/2024/01/Software-safety-classification-1.jpg)
- While ISO 14971 focuses on the overall process and identifies hazardous situations, IEC 62304 works bottom-up to identify how the software can fail and contribute to hazardous situations.
    - Tags:  [[IEC 62304]] [[ISO 14971]]
    - Note: risk based on 14971 vs 62304
- If you are a SaMD developer, most of your risks are likely to relate to the software. So, it might be convenient to expand your [hazard traceability matrix (HTM)](https://medicaldevicehq.com/store/templates/hazard-traceability-matrix-3-examples-iso-14971-medical-device/) to include IEC 62304 specific information, such as ”software item” and ”software causes”.
- “If you think good design is expensive, you should look at the cost of bad design.”
- ![](https://medicaldevicehq.com/wp-content/uploads/2024/01/IEC-62304-planning-overview.jpg)
- Which methods are you planning to use? You can reference existing processes in your [quality management system](https://medicaldevicehq.com/articles/the-illustrated-guide-to-implementing-and-maintaining-a-medical-device-quality-management-system/) or set out a preferred process in the plan. Explain how your approach aligns with the standard’s criteria, whether you favour XP, Scrum, Kanban, test-driven development, or another process.
- What and when will you create outputs from the project? This is not only about the software binary but should also include the documentation that must be established.
    - Note: release means documentation + binary
- Getting the requirements right is crucial for the development work, and [requirements engineering for medical devices](https://medicaldevicehq.com/introduction-to-medical-device-requirements-engineering-online-course/) is an important knowledge area.
- Even though this is a class C requirement only, it may still be worth considering for all classes. If the architecture can isolate critical functionality to a few items, perhaps that enables you to down-classify class B (or C) items to lower classes, easing the development work.
- Documents can be traditional Word documents but could also be captured in a wiki.
- it is essential to remember unit verification. In many cases, unit verification can be performed with the help of a unit test framework. However, unit testing isn’t the only viable option; you can establish any strategy, method, or procedure you find adequate. This can, for instance, include:
  • Peer reviews
  • Static code analysis tools
  • Conformance with coding standards
- This may sound awkward, but it may be acceptable if the bugs are evaluated as not contributing to hazardous situations or otherwise impacting the software functionality. Acceptable residual anomalies can for example be:
  • Typos
  • Misalignment in graphical elements
  • Bugs with acceptable workarounds
- In addition to dealing with identified problems, the maintenance plan should also address maintenance needs triggered by:
  • Changes to SOUPs 
  SOUPs may be subject to upgrades, bug fixes, patches and obsolescence. 
  • Cyber security updates 
  For products exposed to security threats, there is likely a continuous flow of information that must be evaluated.
- ![](https://medicaldevicehq.com/wp-content/uploads/2024/01/Problem-resolution-in-different-life-cycle-phases-1.jpg)
- Two common mistakes are:
  1. Too much documentation too early
  If a software engineer encounters a minor bug, in most cases, it should suffice to document the finding and correct the issue. Since there are no changes to the requirements, it is a correction of what has already been approved, and the value of triggering a significant investigation with corresponding documentation is in most situations not necessary.
  2. Involving too many in the approval process
  In some organisations, there is a tendency to invite the entire company into the change control process. But less is more! Question what value individuals bring before they are invited to take part in the process.
- Agile promotes frequent communication and feedback loops, ensuring clarity in development stages and meeting most verification requirements as defined by IEC 62304.
