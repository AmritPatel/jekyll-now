---
layout: post
title: Shiny New App
---

I'm unofficially done with the Johns Hopkins Data Science Specialization courses. The final project was building a Shiny app. Mine can be accessed [here](https://amritpatel.shinyapps.io/Project). I put together a brief slide deck explaining what it's all about [here](http://amritpatel.github.io/NCAAB-Win-Prediction/slides/index.html).

I think it came together nicely for a first effort. It does take some time for the app to load however since it is basically re-training the prediction model everytime the app is initialized on the server. This was done intentionally so that the model would always be using the latest data (since the model concept depends strongly on this). The app loads data files from [this]() GitHub repository. This setup allows me to push data file updates (as often as daily) directly to the repository to allow the app to function at its full potential. The data file updates ('scores.csv' which trains the model and 'bpi.csv' which is used to make the predictions) simply come from daily cross-validation, which I discussed in the [previous post](http://amritpatel.github.io/NCAAb-Predictions/). 

The original app design was very basic and simpy returned the predicted winner between two teams. I've since added some bells and whistles. The first thing was a static plot that gives a summary of the model accuracy over time compared to a simple [BPI](http://espn.go.com/mens-college-basketball/story/_/id/7561413/bpi-college-basketball-power-index-explained) predictor - it also shows "upset" accuracy for the model over time (note that by definition, a simple BPI predictor has an upset accuracy of zero).

![_config.yml]({{ site.baseurl }}/images/shinyShot.png)

The second thing added was a dynamic plot that changes as new predictions are made. This plot shows a BPI trend for each team selected and can be used for comparing BPI magnitudes and showing how each team has been performing recently. These plots may give some insight into why the prediction model predicts what it predicts.

Hopefully this app can at least score you some early round upset points come tournament time so check it out and let me know how it goes in the comment section below!
