---
layout: page
title: The EEG-EDA Connection
description: Predictive modeling of electrodermal activity (EDA) using EEG, as a proxy of emotional arousal.
img: assets/img/EDA-EEG_project.png
importance: 4
category: research
---

Arousal, a critical component of processes such as vigilance, alertness, attention, and emotion, is intricately linked to both the central and peripheral nervous systems. This project investigates the complex relationship between neural activity and behavioral measures associated with arousal. Our goal is to unravel the coupling dynamics between these elements to improve our understanding of arousal mechanisms.

We've adopted an innovative two-step approach. The first step involves using electroencephalography (EEG) to decode electrodermal activity, a key peripheral marker of arousal. The second step tests whether this predicted electrodermal activity can serve as a proxy for subjective arousal, potentially improving our models for predicting these affective states.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/EDA-EEG_project.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Our methodology focuses on predictive modeling from EEG signals, using spatial filters to reduce dimensionality and better reveal the sources of arousal. We've developed a regression pipeline that allows us to predict electrodermal responses to specific events based on EEG data.

Preliminary results have been enlightening yet challenging, demonstrating the complexity of predicting electrodermal activity from EEG signals alone. This research isn't just about linking two types of physiological data; it's a journey toward a more integrated understanding of how arousal manifests and affects our minds and bodies.

---

_This project was part of my master thesis at the École Normale Supérieure (ENS, Paris) and my internship in the Parietal team (Inria)._

_You can download a PDF copy of my master's thesis [here](/assets/pdf/Thesis_INRIA_damelio.pdf)._
