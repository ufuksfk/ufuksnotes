---
draft: true
description:
socialDescription:
title: Highlights Articles by last edited time
tags:
date: 2025-03-05
modified: 2025-08-21
---
```dataview
table file.mtime as "Last Modified"
from "Highlights/Articles"
SORT file.ctime DESC
```
