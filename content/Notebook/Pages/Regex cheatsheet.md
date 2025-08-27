---
draft: true
description:
socialDescription:
title: Regex cheatsheet
tags:
  - notes/cheatsheet
date: 2025-03-05
modified: 2025-08-21
---
## To search for a word but not with [ ] squared brackets:
(?<!\[\[)George Bush(?!\]\])

## to search for all YYYY-DD-MM in [] and replace it with YYYY-MM#DD
\[\[(\d{4}-\d{2})-(\d{2})\]\] 
[[$1#$2]]