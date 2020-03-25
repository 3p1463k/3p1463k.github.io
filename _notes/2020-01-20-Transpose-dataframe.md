---
title: "Transpose data frame in R"
layout: single
url: "/notes/Transpose-dataframe.md/"
categories:
  - blog
image:
  feature: /assets/images/qr/qr2.png
  thumb: /assets/images/qr/qr2.png
header:
  teaser: /assets/images/qr/qr1.png
classes: wide
last_modified_at: 2019-03-05T16:20:02-05:00
---







```r
final_df <- as.data.frame(t(starting_df))
final_df
```
