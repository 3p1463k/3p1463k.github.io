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

The application, i will be demonstrating here today is for plotting the data from the Nest thermostat. The Google provides you the data at Google Takeout, you can just download it from there (instructions how to do it are in the help section of the application). However the Google doesnt provide any platform where you can see your data on chart, except in the Nest app, where things are really small and you cant see much of the detail and that didnt satisfy me, you could probably feed it to Google Data Studio but i decided to take different step and make my own plots using R language.

Here is the [link](https://p1463k.shinyapps.io/nest-plot/) to the base application.

Here is the example of Daily view of data from csv file.
Main plot in the middle and on the right side, there is two smaller info charts of minimum and maximum temperature and humidity.

[![small image](/assets/images/dashb1.png)](/assets/images/dashb1.png)

It has semi expandable side panel, where you can upload your file and change time periods between daily,weekly and monthly.

# Building the app

The best is, in my opinion to start with simple base and keep adding the features. Here is a base dashboard example:

~~~R
## app.R ##
library(shiny)
library(shinydashboard)

ui <- dashboardPage(
  dashboardHeader(),
  dashboardSidebar(),
  dashboardBody()
)

server <- function(input, output) { }

shinyApp(ui, server)
~~~

If you dont have R Studio on your PC and you want to try this code, you can sign up for free account at [R Studio Cloud](https://rstudio.cloud/), sign up with Google acct and you set in seconds. Then you can copy the code snippet and run this example.
