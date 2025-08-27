---
draft: true
description:
socialDescription:
title: Highlights Books by created time
tags:
date: 2025-03-17
modified: 2025-08-21
---
```dataview
table file.ctime as "Created"
from "Highlights/Books"
SORT file.ctime DESC
```
**