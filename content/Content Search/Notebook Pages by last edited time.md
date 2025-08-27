---
draft: true
description:
socialDescription:
title: Notebook Pages by last edited time
tags:
date: 2025-03-17
modified: 2025-08-21
---
```dataview
table file.mtime as "Last Modified"
from "Notebook/Pages"
SORT file.mtime DESC
```
