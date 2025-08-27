---
draft: true
description:
socialDescription:
tags:
  - geography/city
about:
  - "[[Italy]]"
title: Rome
date: 2025-03-05
modified: 2025-08-21
---
## Notes referenced to 
```dataview
table
    SourceDate as "Source",
    Date as "Noted"
from "100 Notes Box"
where contains(reference,this.file.link)
SORT Date DESC
```

## Notes about to
```dataview
table
    Date as "Noted",
    SourceDate as "Source",
    reference as "Reference"
from "100 Notes Box"
where contains(about,this.file.link)
SORT Date DESC
```
