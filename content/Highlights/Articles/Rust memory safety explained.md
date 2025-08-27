---
draft: true
description:
socialDescription:
title: Rust memory safety explained
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Serdar Yegulalp]]
url: https://www.infoworld.com/article/3714925/rust-memory-safety-explained.html

last highlighted date: [[2024-04#05]]

## Highlights
- *Immutable-by-default* is distinct from the concept of a *constant*. An immutable variable can be computed and then stored as immutable at runtime—that is, it can be computed, stored, and then not changed. A constant, though, must be computable at *compile* time, before the program ever runs. Many kinds of values—user input, for example—cannot be stored as constants this way.
- Every value in Rust has an "owner," meaning that only one thing at a time, at any given point in the code, can have full read/write control over a value. Ownership can be given away or "borrowed" temporarily, but this behavior is strictly tracked by Rust's compiler. Any code that violates the ownership rules for a given object simply doesn't compile.
    - Note: interesting mechanism
- References to values in Rust don't just have owners, but *lifetimes*—meaning a scope for which a given reference is valid. In most Rust code, lifetimes can be left implicit, since the compiler traces them. But lifetimes can also be explicitly annotated for more complex use cases
- Use-after-free errors or "dangling pointers" emerge when you try to access something that has in theory been deallocated or gone out of scope. These are depressingly common in C and C++. C has no official enforcement at compile time for object lifetimes. C++ has concepts like "smart pointers" to avoid this, but they are not implemented by default; you have to opt-in to using them. Language safety becomes a matter of an individual coding style or an institutional requirement, not something the language ensures altogether.
- Rust's memory safety has costs, too. The first and largest is the need to learn and use the language itself.
    - Note: :)
