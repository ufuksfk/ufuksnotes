---
draft: true
description:
socialDescription:
title: Üretimin Tarihi 1
tags:
  - artifacts/podcast
date: 2025-03-05
modified: 2025-08-21
---
```dataview
TABLE
    publisher as "Publisher",
    published_date as "Date"
FROM
    "Highlights/Matter"
WHERE 
    contains(publisher,this.file.link)
SORT published_date DESC
```
