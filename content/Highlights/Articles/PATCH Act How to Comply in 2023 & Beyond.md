---
draft: true
description:
socialDescription:
title: PATCH Act How to Comply in 2023 & Beyond
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[ketryx.com]]
url: https://www.ketryx.com/blog/patch-act-how-to-comply-in-2023-beyond

last highlighted date: [[2024-01#10]]

## Highlights
- An effective SBOM tracks all software sources and associated cybersecurity risk and mitigations of said sources. In addition, since you’re typically operating in a validated environment your SBOM needs to link to applicable test cases that verify any assertions. [[(SBOM) Software Bill of Materials]]
- H.R. 7084, also known as the “PATCH Act of 2022,” outlines a framework for minimal cybersecurity focus within medical devices. The Patch Act (Protecting and Transforming Healthcare Act) has been in development for several years, and a key section grants the FDA long-awaited authority to strengthen its cybersecurity guidance for medical device premarket submissions and post market security management.
- That PATCH act “asks,” if a vulnerability is discovered, who and what actions would be necessary to assess and document risk? How would this be communicated with clients and what timeframe for remediation?
- In particular, the requirement for a Software Bill of Materials, or SBOM, while well-intentioned, isn’t particularly useful to regulators or to users. In fact, the guidance can even make it easier for hackers to exploit known vulnerabilities to compromise patient safety.
    - Note: drawback of the regulation
- In regards to an ASAP out-of-cycle release, in my opinion, all organizations should have the minimal capability to generate a narrowly-scoped patch in less than 30 days. (Distribution and application not included).
- The Patch Act comes into force on October 1, 2023\. The act specifies creation, tracking, and submission of the following: 
  * Product monitoring plan
  * Product cyber-anomaly response plan
  * Coordinated messaging of cyber vulnerabilities
  * Product software releases on a ‘reasonably justified regular cycle’
  * Software Bill of Materials (SBOM)
  * Ability to release a critical vulnerability patch ‘as soon as possible’
  * Collect and maintain additional information in the future
- According to the Patch Act, the term “**Cyber Device”** means a device that either (A) incorporates software; or (B) is designed to establish an internet connection.
- Historically, devices were made with little third party software, but today most devices rely on some percentage of Off-the-Shelf (OTS) software and open source software – which may not have been specifically designed for safety critical systems.
- The requirement to supply an SBOM is more than just a listing of what code sources are in use, it’s also tracking the versions, vulnerabilities, and risk evaluations for all code sources. From a risk standpoint, it’s important to know that the libraries in use are vulnerability free or that identified vulnerabilities are not within your specific code path.
- The PATCH act specifically calls for planning on how to communicate vulnerabilities to appropriate parties. Typically this is a subsection of an incident response plan and would be a coordinated effort amongst many internal groups. The key item with disclosure is the coordination of messages over time and that they reach the necessary parties. Think of a future date when an auditor may review all previous disclosures at once; are the messages consistent, accurate, and forthcoming even with the benefit of hindsight?
- Manufacturers of cyber devices must establish a plan to effectively monitor, detect, and address cybersecurity vulnerabilities and potential exploits within a reasonable timeframe after the device's introduction to the market.
- Manufacturers must create, develop, and maintain processes and protocols for providing updates and patches for the cyber device and associated systems throughout its existence.
- * **Medical Device Manufacturers**: Manufacturers of medical devices, especially those incorporating software and having internet connectivity, are directly impacted. They need to comply with new requirements for cybersecurity measures, including monitoring vulnerabilities, developing disclosure plans, providing software bill of materials (SBOM), and issuing timely updates.
  * **Healthcare Providers and Systems**: Healthcare providers using medical devices that fall under the definition of "cyber device" will need to ensure that they have proper processes in place to manage and apply necessary cybersecurity updates and patches. This is particularly relevant in healthcare facilities, where these devices are in use.
- In particular, any cyber devices in these industries that fall under the following premarket submission categories: section 510(k), 513, 515(c), 515(f), or 520(m).
- **Vulnerability Tracking System**: Implement a robust system to track and manage cybersecurity vulnerabilities and risks.
- **Post-market Surveillance and Incident Response Plan**: Create an incident response plan that outlines how the company will respond to identified vulnerabilities or breaches in development and post-market surveillance. Define roles, responsibilities, communication channels, and steps to mitigate risks promptly that are reported from inside the organization or outside from users.
- **Patch Management**: Establish a systematic process for developing, testing, and deploying patches and updates to address vulnerabilities.
- * **Documentation and Traceability**: Maintain comprehensive documentation of all vulnerability management activities, including vulnerability scans, assessments, patch deployments, and incident responses for [ideal traceability](https://www.ketryx.com/blog/traceability-101).
  * **Audit and Compliance Checks**: Regularly conduct internal audits and compliance checks to ensure that your vulnerability management processes align with the requirements of the Patch Act.
