---
title: "Scrape html table in R with rvest"
url: "/notes/"
tags:
  notes
layout: single  
image:
  feature: /assets/images/notes//io2.jpg
  thumb: /assets/images/notes/io2.jpg
header:
  teaser: /assets/images/notes/io2.jpg
classes: wide
last_modified_at: 2019-04-10T16:20:02-05:00
---

[![small image](/assets/images/notes/io1.png)](/assets/images/notes/io1.png)

First get all the tables on the web page:

```r
library(rvest)

webpage <- read_html("https://en.wikipedia.org/wiki/COVID-19_testing")

tbls <- html_nodes(webpage, "table")

tbls
```


Then see which table you need and convert it to dataframe, in this case I am getting table 2


```r
tbls_ls <- webpage %>%
  html_nodes("table") %>%
  .[2] %>%
  html_table(fill = TRUE)
  
df <- as.data.frame(tbls_ls)

```
