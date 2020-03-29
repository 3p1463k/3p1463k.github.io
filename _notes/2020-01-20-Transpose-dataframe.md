---
title: "Transpose data frame in R"
layout: single
url: "/notes/Transpose-dataframe.md/"
categories:
  - blog
image:
  feature: /assets/images/notes/io5.jpg
  thumb: /assets/images/notes/io5.jpg
header:
  teaser: /assets/images/notes/io5.jpg
classes: wide
last_modified_at: 2019-03-05T16:20:02-05:00
---







```r
final_df <- as.data.frame(t(starting_df))
final_df
```
