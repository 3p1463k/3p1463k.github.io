---
title: "Replace character in R dataset"
url: "/notes/"
tags:
  notes
layout: single  
image:
  feature: /assets/images/notes/io3.jpg
  thumb: /assets/images/notes/io3.jpg
header:
  teaser: /assets/images/notes/io3.jpg
classes: wide
last_modified_at: 2019-03-09T16:20:02-05:00
---

Lets assume we have folowing dataset


| Name    | Date |
|---------|------|
| somefoo | 1    |
| another | 2    |

```r
library(stringr)

df <-  str_replace_all(df1$Name , 'foo', 'bar')
```
| Name    | Date |
|---------|------|
| somebar | 1    |
| another | 2    |



