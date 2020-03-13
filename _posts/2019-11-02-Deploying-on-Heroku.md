---
title: "Deploying Python Dash app on Heroku with gunicorn"
classes: wide
last_modified_at: 2019-06-02T16:20:02-05:00
---

Heroku is not a bad place to host your app, you can create a free account and test your apps on Heroku servers.
They have a nice tutorial how to deploy but not everything is crystal clear. Here i will show how to deploy a simple Python app.I will use just a simple app which takes a dataframe and plots values. I will use a Python Dash with Plotly and instead of [Flask](https://flask.palletsprojects.com/en/1.1.x/) server which is not good for production, i will use [Gunicorn](https://gunicorn.org/).
