---
draft: true
description:
socialDescription:
title: Highlights Podcasts by last edited time
tags:
date: 2025-03-17
modified: 2025-08-21
---
```dataview
table file.mtime as "Last Modified"
from "Highlights/Podcast"
SORT file.mtime DESC
```
