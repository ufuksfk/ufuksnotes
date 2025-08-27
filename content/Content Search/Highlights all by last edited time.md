---
draft: true
description:
socialDescription:
title: Highlights all by last edited time
date: 2025-03-17
modified: 2025-08-21
---
```dataview
table file.mtime as "Last Modified"
from "Highlights"
SORT file.mtime DESC
```
