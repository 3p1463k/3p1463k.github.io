---
title: "Deploying Python Dash app on Heroku with gunicorn"
classes: wide
last_modified_at: 2019-06-02T16:20:02-05:00
---

Heroku is not a bad place to host your app, you can create a free account and test your apps on Heroku servers.
They have a tutorial how to deploy apps but not everything is crystal clear. Here i will show how to deploy a simple Python app.I will use just a simple app which takes a dataframe and plots values. I will use a Python Dash with Plotly and instead of [Flask](https://flask.palletsprojects.com/en/1.1.x/) server which is not good for production, i will use [Gunicorn](https://gunicorn.org/).


Here is an image of the app, it measures a ratio of annotators and displays the value on chart, where you can compare as many workers as you want.
[![small image](/assets/images/heroku/her1.png)](/assets/images/heroku/her1.png)


Here are the imports for the app:
~~~python
import pandas as pd 
import numpy as np
import dash
import dash_html_components as html
import dash_core_components as dcc
import plotly.graph_objs as go
from textwrap import dedent

~~~
