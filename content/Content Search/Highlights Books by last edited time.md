---
draft: true
description:
socialDescription:
title: Highlights Books by last edited time
tags:
date: 2025-03-17
modified: 2025-08-21
---
```dataview
table file.mtime as "Last Modified"
from "Highlights/Books"
SORT file.mtime DESC
```
