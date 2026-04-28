---
layout: page
title: sPOD-NN
description: Model order reduction of a wildland fire model with deep learning methods
img: assets/img/Var40_Nonlinear.png
importance: 1
category: work
---


Since global warming has started wreaking havoc on our planet, scientists are actively trying to study its impacts on the environment. Forests are one part of our ecosystem experiencing the most severe damage. Frequent wildfires have started to decimate flora and fauna in many parts of the world, resulting in far-reaching consequences for life on our planet.

To tackle these critical issues, world governments are investing heavily in research to study wildfire behavior and develop mitigating steps to prevent further loss.

This project addresses this challenge by predicting the spread of wildfires in a computationally efficient way. We achieve this by representing the wildfire spread as a high-dimensional state vector depending on time and physical parameters and combining physical dynamics with advanced scientific methods like reduced order modeling (MOR) and artificial intelligence.

However, to achieve true computational speed-ups, the reduced-order model must be low-dimensional. For transport-dominated systems like moving wildfire fronts, standard Proper Orthogonal Decomposition (POD) struggles to capture the dynamics efficiently. To circumvent this problem, we utilize a recent method called the shifted proper orthogonal decomposition (sPOD). The sPOD method addresses the transport phenomena by decomposing the high-dimensional parameter snapshot matrix into co-moving, low-dimensional frames, utilizing space-time-parameter-dependent shifts.

By applying sPOD to the wildfire model, we extract the time amplitudes and the low-dimensional shifts, stacking them to form our training data. We then deploy a purely non-intrusive machine learning method—the sPOD-NN—to learn the mapping from the parameter space to the data. Once the neural network predicts the amplitudes and shifts, the final wildfire state is rapidly reconstructed. This hybrid approach allows us to predict the solution with significantly better accuracy and massive computational savings compared to conventional methods.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/sPOD_NN_Pipeline.png" title="sPOD-NN pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The overview of the sPOD-NN methodology.
</div>

A detailed description of this project is shown in <a href="https://www.tu.berlin/en/fgmso/research/projects/model-reduction-for-multiple-transported-fronts-with-topological-changes">my TU Berlin page</a> and a novel study of the results is given in our paper.

## Related Publications
<div class="publications">
  {% bibliography -f papers -q @*[key=BuKrRe23]* %}
</div>
