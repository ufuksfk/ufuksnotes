---
draft: true
description:
socialDescription:
title: Riscure_Whitepaper_The_Price_for_Faults
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Riscure]]
url: https://storage.googleapis.com/omnivore/u/4f7edca2-b607-11ee-9b86-b37f4fcd5703/Riscure_Whitepaper_The_Price_for_Faults.pdf?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=omnivore-production%40appspot.gserviceaccount.com%2F20240227%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20240227T220207Z&X-Goog-Expires=14400&X-Goog-SignedHeaders=host&X-Goog-Signature=a4ebc51f7937e3d022e5ebd262b7391c05e5fb5fff53526f0d3db2832548794874e09cbd8ee66a66d51e8969c8d30de01f2192c7cfe486ce6b14e2b8abf4f53c629622e8fb2fe92e53a73095b71b061740451992f5cda78b5928c57fcb08153c37fcbcaef1dd996dbea32848b4561459abac6f90a478d980a968a5353f15d27e80ce59c75913896c345a2e9fd940d9dd567d9951ee4dc1ec4a0155f64b4cf8b7fe7f81e0e81bab2740f83cde3b69f18277fcc7193c91410f98c12f44d264a9c20d1fda96f952b05757077a5d19d6f835eb8e129d1982119e5122c930e87a3beb6e7bcdb0b8f471a12105d2db5fe2030f95a4195200dd94c0515fd03d4048b56a

last highlighted date: [[2024-01#18]]

## Highlights
- For this purpose , traps can be used, that catch fault injection attempts and subsequently disable product functionality.
- Most devices today are completely vulnerable against these attacks as d evelopers have little awareness of the threat, and do not know how to protect their code.
- A voltage glitch would affect all transistors simultaneously, whereas a light pulse can be directed at a very small group of transistors.
- The price range for attack tools ranges from $100 for t he simplest to $100K for the most precise tool.
- As fault injection leads to a change of digital value in the computer chip. The consequence can be either a calculation mistake or a change in the program flow. The latter is caused by changing the res ult of a condition, changing the termination of a loop, skipping instructions, or changing the program counter at a branch, jump or return. Since these constructs are so common, we estimate that at least one exploitable fault injection vulnerability exists for every ten lines of critical code. That means that the vulnerability density is extremely high compared to logical security issues, which have a 100 times lower density ( on average , one per thousand lines of code ) .
- By changing memory pointers and/or loop termination, it is possible to make a chip transmit other than the intended data at any given data communication event
- By changing critical decisions , it may be possible to escalate pri vileges and bypass an authentication mechanism, such as a password verification or a secure boot verification. The attacker uses this to gain unauthorized control over a device.
- When a computational error is introduced during a cryptographic calculation, it may be possible for an attacker to derive the secret key by comparing the corrupted res ult with the expected result
- Gligli used a short voltage dip in the reset line to br ing the Xbox in a particular state where the memcmp function would return true, even if incorrect
- Escalating privileges in Linux based products [6] Niek Timmers and Cristofaro Mune discovered that with voltage glitch equipment , an attacker can easily get root privilege in a Linux system. Since many products build on a Linux kernel , this puts large product segments at risk.
- Extracting secret keys from a Playstation Vita [5] Yifan Lu demonstrated that cryptographic signatures in a popular gaming console can be corrupted and that cryptographic keys can be extracted using a textbook Differential Fault Analysis method
- Resistance can be introduced by making useful values hard to achieve (avoid 0 vs 1 but use complex values like 0xA5 or 0x3E) or by creating non - determinism , making it hard to find the right timing to manipulate a decision.
- This includes double - checking to verify value correctness and crypto results, but also double - checking conditional statements, branches, loops, and program flow.
- Furthermore, there is typically no need to protect the entire code base: protecting the critical code is often good enough.
- A sad but illustrative example of mounting cost for late - identified issues can be found in the impact of the 737 MAX software bug for Boeing . In March 2019 , the airliner was grounded following two dramatic crashes. Over the next six months , Boeing lost 17 % of market cap value (more than 40B value evaporated ) . CNN estimates that the total incident cost for the company reached $18.7B in a year 's time [8]
- We le arned that applying a Fault Mitigation Pattern costs a trained developer , on average , 12 minutes. We base this on our experience of training developers and observing the speed of applying this knowledge. For repairing code that appeared to be flawed in the field, we follow the 100 - fold factor proposed by IBM , thereby assuming that each vulnerability will cost 20 hrs to fix in maintenance.
- To study the cost of bug fixing, we consider a hypothetical IoT product development case. We base our estimates on the f ollowing assumptions:  An average IoT product has 1 00 K LOC, but only 5% = 5 KLOC critical code  Developing a 1 00 K LOC product costs five man - years of work ≈ 9 k hrs  A developer costs $100 per hour  Total development cost s are: $ 900 K
