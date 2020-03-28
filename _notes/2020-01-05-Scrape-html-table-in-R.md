---
title: "Scrape html table in R"
url: "/notes/"
tags:
  notes
layout: single  
image:
  feature: /assets/images/notes//io2.jpg
  thumb: /assets/images/notes/io2.jpg
header:
  teaser: /assets/images/notes/io1.png
classes: wide
last_modified_at: 2019-04-10T16:20:02-05:00
---

```r
webpage <- read_html("https://en.wikipedia.org/wiki/COVID-19_testing")

tbls_ls <- webpage %>%
  html_nodes("table") %>%
  .[2] %>%
  html_table(fill = TRUE)
df <- as.data.frame(tbls_ls)

```
