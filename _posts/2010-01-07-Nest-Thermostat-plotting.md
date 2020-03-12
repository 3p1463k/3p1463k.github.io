---
title: "Nest thermostat data plot using shiny dashboard"
last_modified_at: 2019-03-09T16:20:02-05:00
categories:
  - Blog
tags:
  - Post Formats
  - readability
  - standard
---

This article is to demonstrate the process of making a simple shiny dashboard and plotting the data from csv file.

At the end of of the article i will also describe how to deploy the application on shinyapps.io.
Shiny apps and dasboards are using R language and they are fairly simple to make after you tackle the basis and understand the structure.

The application, i will be demonstrating here today is for plotting the data from the Nest thermostat. The Google provides you the data at Google Takeout, you can just download it from there (instructions how to do it are in help section of the app). However Google doesnt provide any platform where you can see your data, except in the Nest app, where things are really small and you cant see much of details and that didnt satisfy me, so i decided to make my own plots.

Here is the [link](https://p1463k.shinyapps.io/nest-plot/) to the base application.

Here is the example of Daily view of data from csv file.

![App](/assets/images/dashb1.png)

