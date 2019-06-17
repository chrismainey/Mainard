---
abstract: "Patient mortality and its association with healthcare is a contentious topic, with a strong academic history, and various entrenched views.  Despite differing opinions, hospitals and regulatory bodies routinely measure and monitor mortality rates, regarding them as ‘smoke alarms’ related to quality of care.  Many of the techniques used for monitoring were described in an influential RSS paper by Spiegelhalter et al. (2012), and this talk describes them in practice in the NHS.
The risk of death varies between patients according to many factors and these factors must be taken into account when monitoring mortality.  Two of the most common indicators: the Summary Hospital-level Mortality Index (SHMI) and the Hospital Standardised Mortality Ratio (HSMR) are calculated as indirectly-standardised ratios of observed and ‘expected’ deaths.  They vary in their predictors and definitions, but both use logistic regression to predict the risk of death per patient, and the sum of the risk scores form counts ‘expected’ deaths at organisations.  These methods are commonly presented as ‘funnel plots,’ and use control limits to identify outlier organisations.  These techniques, based on the Poisson distribution, suffer from overdispersion and this talk will discuss adjustments techniques. 
Funnel plot methods are only suited to cross-sectional analysis and further techniques are required to monitor over time.  This talk will discuss risk-adjusted CUSUM techniques, as used by NHS regulator the Care Quality Commission (CQC) and Imperial College’s mortality monitoring system.  It explains how they are calculated, the differences between techniques, and how they are used in practice.
Two alternative approaches will be discussed: CUSUMs based on aggregated data using z-scores, and patient-level log-likelihood charts.  These charts have different processes for setting trigger thresholds and involving simulation or approximation techniques.  Examples of techniques will be shown using R, and shortcomings such as the effects of overdispersion and false positives will be discussed."
all_day: false
authors: [~]
date: "2019-09-05"
date_end: "2019-09-05"
event: Royal Statistical Society (RSS) 2019 Annual Conference
event_url: https://www.rss.org.uk/RSS/Events/RSS_Conference/2019_Conference/RSS/Events/Conference/2019_conference.aspx?hkey=2a432b6b-6baf-4bc3-baa4-063221c13ab8
featured: false
image:
  caption: 'Image credit: **Royal Statistical Society (RSS)**'
  focal_point: Center
  preview_only: true
  location: "Belfast, Northern Ireland"
math: true
projects: ""
publishDate: "2019-05-07T00:00:00Z"
slides: ""
summary: Summary of how to use funnel plots and cusums to monitor mortality
tags: 
 - SPC
 - NHS
 - RSS
 - Funnel Plot
 - Cusum
 - mortality
title: "Using funnel plots and CUSUM techniques to monitor hospital-standardised mortality"
url_code: "https://github.com/chrismainey/RSS_2019_CUSUMs"
url_pdf: ""
url_slides: ""
url_video: ""
draft: false
---
