---
layout: post
title: NCAA Basketball Predictions
---

I've been taking the Johns Hopkins Data Science Specialization series of courses for about 7 months now and am finally nearing the end. It's been quite a ride, but I'm finally ready to start crunching some numbers! I'm currently taking the Machine Learning course where prediction modeling using R is briefly (but very usefully) discussed. With March Madness quickly approaching, I've been working on building a prediction model using random forests to train based on team Basketball Power Index -- or BPI -- rating data. Below I show how this model has been faring compared to simply using BPI as a winning predictor.

![_config.yml]({{ site.baseurl }}/images/NCAAb_predictions.png)

I'll be doing daily cross-validation up to Round 1 of the NCAA tournament starting in March, so we'll see how it goes! If you're interested in the R code used to generate the above predictions, you can grab it [here](https://gist.github.com/AmritPatel/3dcc7f0724363bc7d0e6).

With the next Data Science Specialization focusing on developing R Shiny applications, I hope to soon build an interactive prediction engine, so stay tuned!