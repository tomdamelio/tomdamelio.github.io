---
layout: page
title: Decoding arousal from EEG
description: Predicting peripheral autonomic activity directly from cortical signals, treating the body as a supervision signal for the brain.
img: assets/img/EDA-EEG_project.png
importance: 1
category: learning representations
---

**Question.** Can peripheral autonomic activity be predicted directly from cortical signals — and can the spatial structure of that prediction tell us where affective arousal is expressed in the brain?

**What I did.** I designed and led this project as manager and main developer: a regression pipeline that predicts electrodermal and electromyographic activity at the event level from EEG, using spatial filters for dimensionality reduction. Rather than classifying discrete emotion categories, the target is a continuous physiological signal — which turns affective decoding into a cross-modal regression problem with far denser supervision than a label-per-episode design.

**Method.** Spatial filtering on multi-channel EEG to reduce dimensionality and better reveal the sources of arousal; event-level regression against electrodermal and electromyographic activity; MNE-Python; modular, reproducible pipeline structure. A second step tested whether the predicted electrodermal activity can serve as a proxy for subjective arousal.

**Result.** A methodology for predictive modelling of affective arousal from EEG that treats the body as a supervision signal for the brain, together with reusable modules that other researchers in the team could build on. The results also made the difficulty of the problem explicit: predicting autonomic activity from cortical signals alone is far from solved, and that gap is itself informative about how arousal is distributed across central and peripheral systems.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/EDA-EEG_project.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Role and collaborators.** Manager and main developer. Research internship in the Parietal team at INRIA Paris, supervised by Denis A. Engemann, as part of my master's thesis at the École Normale Supérieure.

---

_Code available on [GitHub](https://github.com/tomdamelio/arousal_decoding). You can download a PDF copy of the thesis [here](/assets/pdf/Thesis_INRIA_damelio.pdf)._
