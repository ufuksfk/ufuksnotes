---
draft: true
description:
socialDescription:
title: Should I Query My Firebase Database Directly, or Use Cloud Functions
tags:
- highlight/articles
date: 2025-03-05
modified: 2025-08-21
---
author: [[Doug Stevenson]]
url: https://medium.com/p/fbb3cd14118c

[[(GCP) Google Cloud]] [[Firebase database]]
## Highlights
- If you make the request via Cloud Functions, there is absolutely no client-side caching done by default.
- The case is similar for database writes. If you write a document using the SDK while the client is offline, the write will be persisted locally, then automatically synchronized later when connectivity returns. However, if you write via a call to Cloud Functions, the HTTP connection will obviously fail fast while offline, and the client will have to retry as needed.
