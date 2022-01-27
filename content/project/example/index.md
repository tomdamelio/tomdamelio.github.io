---
slides: example
url_pdf: ""
summary: Regression pipeline to predict EDA (and EMG) activity with data
  obtained from EEG recordings.
url_video: ""
date: 2016-04-27T00:00:00.000Z
external_link: ""
url_slides: ""
title: "Predicting modelling of arousal: an analysis of a public EEG and EDA database"
tags:
  - EEG
  - EDA
  - Prediction
links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://github.com/tomdamelio/ arousal decoding
image:
  caption: ""
  focal_point: Smart
url_code: ""
---
## Objectives

* Disentangle the relationship between the EDA (electrodermal activity) response and EEG predictors.
* Evaluate the performance of our self-reported arousal decoding models.

## [](https://github.com/tomdamelio/arousal_decoding#key-points)Key points

* A regression pipeline to predict EDA (and EMG) activity at the event-level with the data obtained from EEG recordings has been implemented.
* Considering linear models were used, it has been possible to observe patterns of activity at the sensor level in terms of the main components of the predictions.
* We introduced a novel methodology for understanding the dynamics between central and peripheral nervous system signals, and their corresponding behavioural measures.

## Our approach

First, EDA decoding from EEG would be performed, with the idea of boosting high-resolution signals in each subject. Thus, we would train models with continuous inputs (i.e. EDA) and outputs (i.e. EEG) in order to extract as much information as possible from each subject to learn different subject-level function approximations. As an output of this first step, we would represent arousal with a predicted EDA version. This predicted signal would indirectly portray the coupling of autonomic and cerebral arousal, as it is the result of the sum of the EEG features weighted by the different coefficients generated after the fitting process with the EDA output data. This would allow making use of the richness of these signals in a unique representation at the subject level. In this way, the predicted arousal would contain information that is not included in the original EDA data. Consequently, in a second step, we would predict self-reported arousal from the predicted EDA, constituting the second part of the proposed statistical learning approach.

![alt text](https://github.com/tomdamelio/arousal_decoding/raw/master/Fig%20-%20Thesis%20-%20two-step-approach_Mesa%20de%20trabajo%201.png)

## Code Availability

The source code of the implementations used to compute organization, processing and statistical analyses can be obtained from