---
layout: page
title: Methods of Multimodal Fusion for Stress Detection
description: We compare methods of multimodal fusion in neural networks on the Wearable Stress and Affect Detection (WESAD) dataset 
img: assets/img/projects/wesad_fusion.png
importance: 2
category: work
---

This work was done as part of the seminar in the course "Bio-Inspired Artificial Intelligence" in my master studies.

Using the WESAD Dataset for wearable stress and affect detection, we compared different methods of multi-modal fusion in neural networks. Results employing the
[Gated Multimodal Fusion Unit (GMU)](https://arxiv.org/abs/1702.01992), linear sum and concatenation are presented and compared against AdaBoost as a baseline. In our experiment, all neural fusion
methods achieved similar performance, while being substantially better than the AdaBoost baseline. 

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/projects/wesad_fusion.png title: "Network structure." class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the model architecture, using the GMU for multimodal fusion
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/projects/bar_plot_with_error_bars-2.png title: "Mean accuracy and F1-score results using leave-one-subject-out cross
validation, error bars are indicating standard deviation." class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Mean accuracy and F1-score results using leave-one-subject-out cross validation, error bars are indicating standard deviation.
</div>

To find out if the GMU behaves differently when random noise is introduced, we carried out a second experiment. Noise was applied on one modality at inference time. Cosequently, the performance of all methods dropped, but, surprisingly, the models using the gated fusion module deteriorated most notably, resulting in below chance-level accuracy.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% responsive_image path: assets/img/projects/bar_plot_noise.png title: "Mean accuracy and F1-score results using leave-one-subject-out cross
validation, error bars are indicating standard deviation." class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Mean accuracy and F1-score results using leave-one-subject-out cross validation in the noise condition, error bars are indicating standard deviation.
</div>

For more details, feel free to look at our [seminar report [PDF]](/assets/pdf/Comparing_Methods_of_Multimodal_Fusion_for_Wearable_Stress_and_Affect_Detection.pdf). The source code for our evaluation is available for download [here](https://git.informatik.uni-hamburg.de/6ambsdor/mmfusion-wesad/-/tree/master/).