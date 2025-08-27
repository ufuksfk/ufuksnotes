---
draft: true
description:
socialDescription:
title: Clippings Matter by last edited time
date: 2025-03-07
modified: 2025-08-21
---
```dataview
table
    publisher as "Publisher",
    published_date as "Date"
from "Clippings/Matter"
SORT file.mtime DESC
```
