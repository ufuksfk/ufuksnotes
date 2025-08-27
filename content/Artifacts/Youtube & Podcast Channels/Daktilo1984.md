---
description:
socialDescription:
title: Daktilo1984
draft: true
tags:
  - artifacts/podcast
link:
date: 2025-03-05
modified: 2025-08-21
---
```dataview
TABLE
    publisher as "Publisher",
    published_date as "Date"
FROM
    "Highlights/Podcast"
WHERE 
    contains(publisher,this.file.link)
SORT published_date DESC
```
