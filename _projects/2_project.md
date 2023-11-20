---
layout: page
title: word embedding explanation
description: explain word embeddings via automatic rule learning in text classification
img: assets/img/word.png
importance: 2
category: work
related_publications: gao2023word
---

In this project, we introduce a novel methodology to find out task-related dimensions within word embeddings. By harnessing the power of automatic rule learning, we effectively extract the critical dimensions relevant to particular tasks.

Rule-based Representation Learner (RRL) is a classifier that automatically learns interpretable non-fuzzy rules for data representation and classification.

<div class="d-flex justify-content-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/RRL.png" title="RRL architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The architecture of RRL
</div>

In this project, the word embeddings of text are initially fed into the RRL for gender classification, then we can derive the gender-related dimensions (identified as the “red dimensions”) from RRL learned rules. These gender-related dimension values will then be removed for subsequent tasks.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/explanation.png" title="explanation process" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Word embedding explanation process
</div>
