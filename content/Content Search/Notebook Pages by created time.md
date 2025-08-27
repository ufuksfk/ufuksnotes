---
draft: true
description:
socialDescription:
title: Notebook Pages by created time
tags:
date: 2025-03-17
modified: 2025-08-21
---
```dataview
table file.ctime as "Created"
from "Notebook/Pages"
SORT file.ctime DESC
```
