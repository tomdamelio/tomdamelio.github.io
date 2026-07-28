---
layout: page
title: What emotion models are we actually fitting?
description: A systematic review and meta-analysis of the theoretical commitments hidden inside emotion recognition systems built on electrodermal activity.
img: assets/img/Emotion_review_1.png
importance: 3
category: learning representations
---

**Question.** Every emotion recognition system built on electrodermal activity implicitly assumes a theory of emotion — discrete, dimensional, appraisal-based. Which one, and does it match the one its authors claim?

**What I did.** I led a systematic review and meta-analysis of emotion recognition systems using EDA, examining not only their reported performance but the theoretical commitments embedded in their design: how affect was induced, how it was labelled, and what was treated as ground truth. The hypotheses were [pre-registered](https://osf.io/zbqm6/).

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/Emotion_review_1.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Result.** Models designed to predict arousal outperform those that predict valence — consistent with the theoretical framework linking arousal to the autonomic nervous system, and therefore to EDA.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Emotion_review_3.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The review also reveals a systematic mismatch between the machine learning models predominantly used (classification) and the emotional models actually invoked (usually dimensional). Despite the field's move toward dimensional accounts of affect, the adoption of regression models — better suited to the continuous nature of emotional data — lags well behind.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/Emotion_review_2.png" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The broader point is about evaluation. A large share of these systems inherit assumptions they never state, which limits how far their results can be interpreted or compared across studies — a problem that becomes more acute, not less, as larger pretrained models enter the field.

**Role and collaborators.** First author, with Luis Galán, Emmanuel Maldonado, Anabella Díaz Barquinero, Juan Rodríguez Cuello, Nicolás Bruno, Enzo Tagliazucchi and Denis Engemann.

---

_Published in [Neurocomputing](https://doi.org/10.1016/j.neucom.2025.130831) 651, 130831 (2025). [Code](https://github.com/EmmAMaldonado/review-emotion-recognition-eda) · [preprint PDF](/assets/pdf/papers/D_Amelio_et_al_2023_review.pdf)._
