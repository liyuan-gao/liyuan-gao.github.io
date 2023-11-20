---
layout: page
title: ESM-TFpredict
description: an explainable method for transcription factor prediction within protein sequences
img: assets/img/TF.jpg
importance: 1
category: work
related_publications: gao2023explainable
---
In this study, we propose an ESM-TFpredict model, which leverages a pre-trained protein language model to encode amino acid sequences, followed by 1-D convolutional neural networks for transcription factor prediction.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ESM-TFpredict.png" title="ESM-TFpredict model architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The architecture of ESM-TFpredict model
</div>

To elucidate the model's decision-making, we employ an integrated gradients technique to highlight the important features driving TF identification. The experimental results demonstrate that the TF-related regions have dominant influences on TF prediction task.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/IG_case1.png" title="TF prediction attribution score" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    TF prediction attribution score of Zinc finger and BTB domain-containing protein 32 (Zinc finger position: 373-395, 401-423, and 428-450)
</div>
