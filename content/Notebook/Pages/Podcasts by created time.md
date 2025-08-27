---
draft: true
description:
socialDescription:
title: Podcasts by created time
tags:
  - note/list
  - note/highlight
link:
date: 2025-03-05
modified: 2025-08-21
---

```dataview
table
    publisher as "Publisher",
    published_date as "Date"
from "Highlights/Podcast"
SORT file.ctime DESC
```
