---
draft: true
description:
socialDescription:
title: BlackBerry QNX for Secure Embedded Systems
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[qnx.com]]
url: https://blackberry.qnx.com/en/ultimate-guides/embedded-system-security

last highlighted date: [[2024-04#15]]

## Highlights
- The most secure embedded system is one that is turned off, and the next most secure system is completely isolated
- Many mission-critical systems, such as cars, defense systems and power plants, have a long service life — 20 years or more
- When the OS and all OS services run in kernel space, applying an OS service patch requires a full OS install, OS refresh, and a full system reboot—all of which increase the scope of testing and the time to deploy.
    - Tags: [[embedded]] 
- In comparison, the architecture of a microkernel OS, such as the [QNX® Neutrino® Real-Time Operating System (RTOS)](https://blackberry.qnx.com/en/products/foundation-software/qnx-rtos), makes embedded software updates much easier. OS services in a microkernel run outside of kernel space, which allows for the rebooting of a single service, without a kernel reboot, resulting in very minimal impact on kernel behavior. In addition, the footprint of a microkernel OS service update is generally small—it doesn’t necessarily require the kernel to be updated at the same time—reducing the time and cost of testing a patch.
    - Note: what advantage we have here?
- Some embedded system attacks are active: they change the behavior of the system. Other attacks are passive: they read data and spy.
- Vulnerabilities present in the embedded software from the beginning
- As many as 20 percent of industrial control systems have critical security issues.
- Less code running in kernel space reduces the attack surface and increases security
- A determined hacker, as long as they don’t have root access, can only crash one component at a time when the system runs a microkernel OS or a [secure embedded hypervisor](https://blackberry.qnx.com/en/products/foundation-software/qnx-hypervisor).
- A hardware security module (HSM) or hardware root of trust manages keys, performs encryption and decryption functions, and embeds keys for OS and application use. Often these system-on-a-chip (SoC) components provide CPU offload for bulk encryption and decryption, and they may also be used to offload network cryptographic functions.
    - Note: hardware security module?
- A trusted execution environment (TEE) or hardware security zone provides hardware-enforced isolation in a secure area built into the main processor, which allows the software developer to establish a device root of trust. A TEE may run in a secure mode of the processor (e.g., ARM TrustZone) or on a separated, isolated CPU core that acts as a security co-processor to the SoC. TEEs typically allow trusted applications to perform security-critical processing on behalf of the embedded system.
- Executable space protection (ESP) marks specific memory regions as non-executable, so that an attempt to execute machine code in those regions causes an exception.
- Address space layout randomization (ASLR) allocates the base address of the stack, heap and shared memory regions to new locations every time a new process is executed, making buffer overflow attacks difficult because a threat actor can’t predict where the information will be stored.
- Stack canaries allow the operating system to detect a stack buffer overflow before executing malicious code. The OS places a small random integer before the stack return pointer and checks for it before overwriting memory. If the stack value has changed, the OS will stop execution and cause an exception.
- Although 70 percent of the most popular embedded OS lack at least one of these defense mechanisms, QNX Neutrino RTOS provides all three.
