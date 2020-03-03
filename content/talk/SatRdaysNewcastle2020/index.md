---
abstract: "George Box is often credited with the phrase ‘…all models are wrong, but some are useful.’ Whilst this makes sense to me now, it was frustrating in my early career, when I didn’t know if I was wrong, my model was the wrong choice, I coded it badly, or if it was working as well as it could. This talk summarise part of my PhD work, attempting to build predictive models on NHS Incident Reporting data in R. Firstly, the data quality was terrible. This is to be expected when you understand the context in which it was generated, and I’ll discuss data generating mechanisms and some of our assumptions about them. To get around my poor data, I ‘borrowed strength’ from other datasets and used them at the same level of aggregation. This became a ‘panel’ dataset, and I was modelling count data. I will discuss our default assumption of Poisson regression (GLM), why it is not perfect with real-word data, and what overdispersion is. There are a variety reasons for overdispersion, and my models proceeded by testing different sources and assumptions including: clustering, aggregation, and ‘noise’ from poor data quality. I will discuss methods for fitting these assumptions including GEE, GLMM, Boostrapping / Cross-validation, GAMs with smoothers, and a Random Forest thrown in for good measure. The ultimate question here is: ‘is my model any good?’ I will briefly discuss how we can assess predictive model accuracy, and a few different schools of thought on it. All examples will be presented with a why, and a how, including R code made available on GitHub. I will focus both on the how I chose and learnt the methods, as well as practical tips for analysing count data with overdispersion."
all_day: true
authors: [~]
date: "2020-04-04"
date_end: "2020-04-04"
event: SatRdays Newcastle 2020
event_url: https://newcastle2020.satrdays.org/
featured: false
image:
  caption: 'Image credit: **SatRdays**'
  focal_point: Center
  preview_only: true
  location: "Newcastle, United Kingdom"
math: true
projects: ""
publishDate: "2020-03-03T00:00:00Z"
slides: ""
summary: Tales of learing to build count data models when you can't tell if you're wrong.
tags: 
 - R
 - NHS
 - EARL
title: "Why is my model so bad?: Tales of a wandering PhD studentDriving R adoption in an NHS information service, barriers and solutions"
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
draft: false
---
