---
draft: true
description:
socialDescription:
title: So, So Many Lines of Memory-Unsafe Routines in Crucial Open Source, and Unsafe Dependencies
  Dependencies
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Thomas Claburn]]
url: https://www.theregister.com/2024/06/28/cisa_open_source/

last highlighted date: [[2024-11#14]]

## Highlights
- The US government's Cybersecurity and Infrastructure Security Agency (CISA) has analyzed 172 critical open source projects and found that more than half contain code written in languages like C and C++ that are not naturally memory safe.
- [Memory safety errors](https://www.memorysafety.org/docs/memory-safety/), such as buffer overflows, use of uninitialized memory, type confusion, and use-after-free flaws, have been a matter of concern in the technical community for years. They're commonly the result of programming errors in C/C++ code and account for the [majority of the vulnerabilities](https://alexgaynor.net/2020/may/27/science-on-memory-unsafety-and-security/) in large codebases.
- Whatever the case, Google and Microsoft have made a show of moving toward memory-safe languages, [initially for new projects](https://www.theregister.com/2022/09/20/rust_microsoft_c/) and lately for application rewrites. Google, for example, earlier this year said its Rust development teams are [twice as productive](https://www.theregister.com/2024/03/31/rust_google_c/) as its C++ teams.
- 55 percent of the total lines of code (LoC) for all projects were written in a memory-unsafe language.
- Dependency analysis of three projects written in memory-safe languages demonstrated that each one depended on other components written in memory-unsafe languages.
- The projects evaluated include: Chromium, Gecko, KVM, Linux, LLVM, GCC, JDK, Node, and many others.
- Gunnar Braun, technical manager at the Synopsys Software Integrity Group, told *The Register* that it's important to raise awareness of memory safety as a means to make software more secure.
- "Memory safety should be one of the key considerations when deciding on a programming language," said Braun. "The report and its preceding 'Case for Memory Safe Roadmaps' bring this to C-level executives – where it belongs. Software security and safety are no longer a purely technical concern."
