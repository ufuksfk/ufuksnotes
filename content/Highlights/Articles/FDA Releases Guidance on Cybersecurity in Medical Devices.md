---
draft: true
description:
socialDescription:
title: FDA Releases Guidance on Cybersecurity in Medical Devices
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[John Giantsidis]]
url: https://www.meddeviceonline.com/doc/fda-releases-guidance-on-cybersecurity-in-medical-devices-0001

last highlighted date: [[2024-04#10]]

## Highlights
- Internet of Medical Things (IoMT
- latest FDA effort is [a draft guidance that expects security](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/cybersecurity-medical-devices-quality-system-considerations-and-content-premarket-submissions) throughout the total product life cycle (TPLC)
- However, let’s revisit the PATCH Act if/when it gets passed.
    - Note: did it passed?
- First, it is important to understand that the scope of FDA’s guidance is exceptionally broad and covers devices that contain software (including firmware) or programmable logic, as well as SaaMD, and would be expected for
- Secure Product Development Framework (SPDF
- • Cybersecurity is an integral part of device safety and the QSR
  • Security by design
  • Transparency
  • Security risk management
  • Security architecture
  • Testing/objective evidence
- Define Security Requirements for Product Development:
- This includes requirements from internal sources (e.g., the organization’s policies, business objectives, and risk management strategy) and external sources (e.g., applicable laws and regulations).
- mplement Supporting Toolchains: Use automation to reduce human effort and improve the accuracy, reproducibility, usability, and comprehensiveness of security practices throughout the TPLC, as well as provide a way to document and demonstrate the use of these practices.
- Archive and Protect Each Product Release: Preserve product/software releases in order to help identify, analyze, and eliminate vulnerabilities discovered in the product/software after release.
- Create Source Code by Adhering to Secure Coding Practices: Decrease the number of security vulnerabilities in the software and reduce costs by minimizing vulnerabilities introduced during source code creation that meet or exceed organization-defined vulnerability severity criteria
- Decrease the number of security vulnerabilities in the software and reduce costs by eliminating vulnerabilities before testing occurs.
- Test Executable Code to Identify Vulnerabilities and Verify Compliance with Security Requirements
- Assess, Prioritize, and Remediate Vulnerabilities: Help ensure that vulnerabilities are remediated in accordance with risk to reduce the window of opportunity for attackers.
- devices must meet the security objectives of authenticity, integrity, authorization, availability, confidentiality, and secure and timely updatability and patchability.
- the type of cybersecurity vulnerabilities present
- the risk of patient harm due to vulnerability exploitation.
- a device would be deemed that it appropriately accounts for authenticity when it evaluates and ensures authenticity for
- entity authentication of communication endpoints, whether those endpoints consist of software or hardware,
- Install cryptographically authenticated firmware and software updates and do not allow installation where such cryptographic authentication either is absent or fails
- Disable or otherwise restrict unauthorized access to all test and debug ports (e.g., JTAG, UART) prior to delivering products
    - Note: always? what about medbeat?
- Verify the integrity of all incoming data
- Protect the integrity of data necessary to ensure the safety and effectiveness of the device.
- Review all code that handles the parsing of external data using automated (e.g., static and dynamic analyses) and manual (i.e., code review) methods.
    - Note: ci pipeline
- Any risks transferred to the user should be detailed and considered for inclusion as tasks during usability testing (e.g., human factors testing) to ensure that the user has the capability to take appropriate actions to manage those risks
- A list of network ports and other interfaces that are expected to receive and/or send data.
- Log file descriptions should include how and where the log file is located, stored, recycled, archived, and how it could be consumed by automated analysis software.
- The FDA guidance further expects that manufacturers institute a formal plan for how they will identify and communicate vulnerabilities that are identified after releasing the device to users.
- This plan is to be in unison with risk management processes under 21 CFR 820.30(g) and corrective and preventive action processes in accordance with 21 CFR 820.100.
- “Security risk management should be part of a manufacturer’s quality system.”
- FDA considers threat modeling “foundational” and an integral part of security risk management
- capture cybersecurity risks introduced throughout
  • supply chain,
  • manufacturing,
  • deployment,
  • interoperation with other devices,
  • maintenance/update activities, and
  • decommission activities processes.
- Moreover, manufacturers must put in place processes and controls to ensure that their suppliers conform to the manufacturer’s cybersecurity requirements
- That means that cybersecurity would have to be extended to supplier management practices and documented in the Device Master Record as required by 21 CFR 820.181
- The FDA guidance places great emphasis on the process and issuance of a Software Bill of Materials (SBOM) and considers the changes in the SBOM as part of the Design History File (21 CFR 820.30) and Device Master Record (21 820.181). [[(SBOM) Software Bill of Materials]]
- • the asset(s) where the software component resides,
  • the software component name,
  • the software component version,
  • the software component manufacturer,
  • the software level of support provided through monitoring and maintenance from the software component manufacturer,
  • the software component’s end-of-support date, and
  • any known vulnerabilities.
    - Note: SBOM
- FDA recommends, under 21 CFR 820.100, manufacturers develop and maintain security architecture view documentation as part of the process for the design, development, and maintenance of the system.
- The FDA draft guidance, under the existing QSR, declares that verification and validation activities shall include sufficient testing performed on the cybersecurity of the system through which the manufacturer verifies and validates their inputs and outputs
- The following cybersecurity testing and corresponding objective evidence would be considered the minimum that may support a premarket submission:
- Abuse case, malformed and unexpected inputs
  • Robustness
  • Fuzz testing
- Closed box testing of known vulnerability scanning
- Static and dynamic code analysis, including testing for credentials that are “hardcoded,” default, easily guessed, and easily compromised.
- Overall, the FDA understands that the cybersecurity threat landscape is rapidly evolving and requires constant monitoring and appropriate corrective and preventive action from medical device manufacturers, alongside timely communication to medical device users to establish their awareness of cybersecurity threats.
