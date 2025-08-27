---
description:
socialDescription:
title: Medical Device Software Process Blackbelt
draft: true
tags:
  - highlight/course
link:
date: 2025-03-05
modified: 2025-08-21
---
I am taking this course starting from [[2025-02#27]] to refresh my knowledge and prepare for interviews
..

Safety Critical Foundations
How to analyze effects of change on software that has already been released.
Always around risk management.
![[Pasted image 20250227112747.png]]

# Safety Critical Foundations
International Standards - Regulatory Overview - Quality Systems - Design & Risk Controls
Medical, Aviation, Industrial Controls, Transportation, Nuclear

2 highly reccomended book from mid  [[1990s]]
[[Safeware System Safety and Computers]]
[[Safety Critical Computer Systems (book)]]

## Example Design Architectures
### Single channel pattern
Source -> Input processing -> data transformation -> output processing -> actuation
### Dual channel pattern
Source     -> Input processing -> data transformation -> output processing -> actuation
		-> Input processing -> data transformation -> output processing ->

He is giving 2 example from his career.

[[Bluetooth]] has a stack and it is [[(SOUP) Software of Unknown Provenance]] example for [[(SiMD) Software in Medical Device]]
but for [[(SaMD) Software as Medical Device]] there are lots of libraries, programming languages, operating systems or off the shelves.

If a medical device integared together with an app can't operate without a mobile or desktop app, this software can be considered as [[(SiMD) Software in Medical Device]]

[[Example of not medical devices]]
* medical dictionaries
* library of clinical descriptions for diseases and conditions
* encyclopedia of first-aid or emergency care information
* medical abbreviations and definitions
* translations
* medical flash cards with medical images
* quiz apps
* interactive anatomy diagrams or videos
* surgical training videos
* medical board certification or preparation apps
* determine billing codes like ICD-9
* enable insurance claims data collection and processing and other apps that are similarly admin in nature
* medical business accounting apps
* manage shifts for doctors
* manage or schedule hospital rooms or bed spaces

safety critical means failure can result with hazard

# Standards
[[IEC 82304]] is mainly for [[(SaMD) Software as Medical Device]] while
[[IEC 62304]] is for [[(SiMD) Software in Medical Device]]

# Regulatory
TGA, ECA, Health Canada, [[FDA]]

Milestones in [[FDA]] history
[[1906]] Food and Drug Act
[[1938]] Food Drug and Cosmetic Act
[[1970]] Cooper Panel Report
[[1976]] Medical Device Amendments
* 510(k) notification process
* PMA process

[[FDA device classification]]:
Class 1, 2 or 3
Only Class III needs pre-market approval

# Quality Systems & Design Control
Components of Quality System
Acceptance Activities, Servicing, Corrective and preventive action, traceability
Main standard is [[ISO 13485]] is aligned with [[21 CFR 820]]
[[Design Planning of Medical Device]]: Each manufacturer shall establish and maintain plans that describe or reference the design and development activities and define responsibility for implementation. The plans shall identify and describe 
[[Design Input of Medical Device]] : ..
[[Design Output of Medical Device]]: ..
[[Design Review of Medical Device]]: ..

[[Design Verification of Medical Device]]: Each manufacturer shall establish and maintain procedures for verifying the device design. Design verification shall confirm that the design output meets the design input requirements. The result of the design verification, including identification of the design, method(s), the date, and the individual performing the verification shall be documented in [[(DHF) Design History File of Medical Device]]

[[Design validation of Medical Device]]: Each manufacturer shall establish and maintain procedures for validating the device design. Design validation shall be performed under defined operating conditions on initial production units, lots, or batches, or their equivalents. Design validation shall ensure include testing of production units under actual or simulated use conditions. Design validation shall include software validation and risk analysis, where appropriate. The result of the design validation, including identification of the design, method(s), the date, and the individual performing the validation shall be documented in [[(DHF) Design History File of Medical Device]]


All is for reducing risk, initial risk should get smaller thanks to risk controls to mitigate risk hazards

# Risk fundementals
Notable lifecycle types:
Waterfall
Spiral
V-model = every step at left has a testing step at right
agile

## Intro
### Definitions
[[Harm of Medical Device]]: Injury or damage to the health of people or environment (hasar)
[[Hazard of Medical Device]]: Potential source of harm (tehlike)
[[Risk of Medical Device]]: Combination of probability of occurence of harm and the severity PoS
[[Risk Management of Medical Device]]: Systematic application of management policies, procedures, and practices to the task of analyzing, evaluating, controlling and monitoring risk
[[Risk Analysis for Medical Device]]: systematic use of available information to identify hazards and to estimate the risk
[[Risk Control of Medical Device]]: Process in which decisions are made and measures implemented by which risks are reduced to, or maintained within, specified levels
[[Risk evaluation of medical device]]: process of comparing the estimated risk against given risk criteria to determine the acceptability of the risk
[[Safety of Medical Device]] freedom from unacceptable risk

[[AAMI TIR 57]] is also very aligned with [[ISO 14971]]

[[Safety Classification of Medical Software]]:
[[IEC 62304]] says by default all software is Class C,
If no software hazard, Class A
Once you evaluate external risk control measures If risks are acceptable and Class A
If risks are resulting harm, then Class B or C. Serious injury goes to Class C
![[Pasted image 20250227153526.png]]
![[Pasted image 20250227153543.png]]
It can be a bit confusing but each item can have their safety classification
Higher classification means more requirements
![[Pasted image 20250227154016.png]]
## Legacy Software
Integration of legacy software can have risk and should be maintained. 
Gap Analysis: Asses continuing validity of available deliverables
Gap closure: 

## Software Risk Management
Risk is product of all probability and severity of harm

Risk calculations of software is different than hardware.

100%  probability to begin with and risk control to reduce.
If risk control is only reducing probability but severity is dead?

In reality, all medical softwareis under the scope of [[IEC 62304]] while [[(SaMD) Software as Medical Device]] is under the scope of [[IEC 82304]] = Health software

### Real world scenario
Imagina you have a sw algorithm that is generating an image that doctor reads. It is critical input to diagnose cancer.
![[Pasted image 20250227160727.png]]
software risk controls only affects P1
![[Pasted image 20250227161853.png]]
Pitfalls!
![[Pasted image 20250227162510.png]]
How to verify software risk control
# SDLC for Medical Software
## Software Planning
Inputs -> planning -> outputs
Inputs:
Security Analysis, System requirements specs, usability analysis, risk management plan, Hazard analysis, safety classification
Output: Software Development Plan, Software Configuration Management Plan, Software Unit test plan, software integration test plan, software verification plan

Verification is a process of determining if 
Are you building product, right > verification
Are you building right product > validation

[[(SDP) Software Development Plan for Medical Software]]
* Clear and spesific objectives
* Realistic and feasible
* Comprehensive and detailed
* Flexible and Adaptable
* Collaborative and Involves Stakeholder
* Communication Focused
* Supports Continuous Improvement
* Aligned with Best Practices

Needs to address:
* Lifecycle model used
* Safety Classification
* Processes used
* Deliverables
* Requirements traceability
* Config management
* Problem resolution
* Risk management
* Document produced
* System requirements
* Procedures for coordinating development per quality system
* Standards, Methods, tools associated with development
* Identification and avoidance of common software defects
* Integration and Test planning

[[(SCM) Software Configuration Management Plan for Medical Software]]:
* Classes, types, categories or lists of items to be controlled
* Activities and tasks
* Organization responsible for performing SCM and activities
* When the items are to be placed under config control
**SCM is used on items BEFORE they are verified!**

Software Unit Test Plan
Software Integration Test Plan
## Software Requirements Analysis
Types of requirements:
* Functional and capability
* security
* User interface
* Data & database
* Installation and acceptance
* Operation and maintenance
* IT and network
* Regulatory


I stop this course at Section 6 - Software Requirement Analysis. It was mainly because he is just reading text with very boring voice...