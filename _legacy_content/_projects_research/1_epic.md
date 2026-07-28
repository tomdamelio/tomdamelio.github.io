---
layout: page
title: Continuous emotion prediction (EPiC Challenge)
description: Third place in an international benchmark for predicting moment-to-moment affect from physiology — and evidence that the body moves before the report.
img: assets/img/EPiC_portada.png
importance: 3
category: temporal dynamics
---

**Question.** Most affective computing models are trained on summary annotations collected after the fact. What happens when you train on continuous ones instead — and what does the model's temporal structure reveal about the relationship between physiology and experience?

Summary annotations mean recording participants' physiological responses while they experience a given affective state, but collecting the rating only once the induction is over. That has two costs: far fewer data points to train on, and an oversimplified account of emotion that denies its natural dynamics.

**What I did.** I led our team in the [Emotion Physiology and Experience Collaboration (EPiC) 2023 challenge](https://epic-collab.github.io/competition/), building continuous predictive models of valence and arousal from the eight physiological measures in the [Continuously Annotated Signals of Emotion (CASE) dataset](https://www.nature.com/articles/s41597-019-0209-0), and then analysing *which parts of the temporal window* the models actually relied on.

**Method.** Continuous regression of valence and arousal across four held-out generalization scenarios; feature-importance analysis partitioning the window into pre-annotation, concurrent and post-annotation information; comparison against dummy baselines and the published benchmark.

**Result.** Third place out of 14 international teams, and a first benchmark of continuous predictive models on this dataset, with significant improvements over existing benchmark models in specific challenge scenarios. Models predicting arousal outperformed those predicting valence, consistent with established findings in the affective science literature.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/EPiC_1.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>Fig. 1.</b> Boxplots with scatter plot overlaid comparing the distribution of RMSE values across four different scenarios (scenario 1 to 4) for both the arousal and valence dimensions, with predictions in each scenario also compared to dummy predictions. Each subplot represents one dimension: arousal at the top and valence at the bottom. Each boxplot represents the interquartile range (IQR) with a line at the median. Overlaid scatter plots show the performance of each model.
</div>

Moreover, our analysis revealed a crucial insight: predictive models that incorporate features of past data provide more informative results than those based on future data.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/EPiC_2.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <b>Fig. 2.</b> Distribution of feature importance for the 240 models trained in scenario 1. It illustrates the distribution of feature importance by partitioning the window into past (pre-annotation), present (during annotation), and future (post-annotation) information. Boxplots, violin plots and scatterplots are used to visualize the feature importance distributions.
</div>

This suggests a fundamental role for physiological activity as a *precursor* to affective experience and its subsequent annotation — the body moves before the report. For anyone building models of affect from physiology, that ordering is not a detail: it determines what a model is allowed to see, and when.

**Role and collaborators.** Team lead and first author, with Nicolás Bruno, Leandro Bugnon, Federico Zamberlan and Enzo Tagliazucchi. The challenge was organised by Stanford University, and results were presented at the EPiC workshop at ACII 2023, hosted by the MIT Media Lab.

---

_Paper presented at the International Conference on Affective Computing and Intelligent Interaction 2023 (ACII 2023), EPiC workshop. [PDF](/assets/pdf/papers/D_Amelio_et_al_2023_ACIIW.pdf) · [code](https://github.com/tomdamelio/EPiC-2023-Challenge)._

_A related big-team-science study on the promises and limits of machine learning for modelling physiological markers of affect appeared in [Royal Society Open Science](https://doi.org/10.1098/rsos.241778) (2025)._
