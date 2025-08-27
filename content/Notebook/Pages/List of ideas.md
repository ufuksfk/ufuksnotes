---
description:
socialDescription:
title: List of ideas
draft: true
tags:
  - note/list
  - note/idea
link:
date: 2025-03-05
modified: 2025-08-21
---
```dataview
table file.ctime as "Created"
from "Notebook/Pages"
where contains(tags, "note/idea")
sort file.ctime desc
```
#note/idea 