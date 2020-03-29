---
title: "Replace character in R dataset"
url: "/notes/"
tags:
  notes
layout: single  
image:
  feature: /assets/images/notes/io3.png
  thumb: /assets/images/notes/io3.png
header:
  teaser: /assets/images/notes/io3.png
classes: wide
last_modified_at: 2019-03-09T16:20:02-05:00
---

Lets assume we have folowing dataset

Name          Date
somefoo       1
anotherfoo    2


```r
library(stringr)

df <-  str_replace_all(df1$Name , 'foo', 'bar')
```

Name          Date
somebar       1
anotherfoo    2



#[![small image](/assets/images/sigm/sigm1.png)](/assets/images/sigm/sigm1.png)
