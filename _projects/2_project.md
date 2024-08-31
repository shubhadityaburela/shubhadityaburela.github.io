---
layout: page
title: NsPOD
description: Automated transport separation with neural networks
img: assets/img/NsPOD.png
importance: 2
category: work
---



Simplifying complex, transport-dominated systems is essential for optimizing flows in areas like fluid dynamics, heat transfer, and mass transfer. 
This optimization is crucial across industries such as aerospace and automotive engineering. 
Reduced order models allow for quick prototyping and design exploration, making it easier to identify ideal flow patterns. 
Moreover, these models support the creation of effective control strategies to dynamically fine-tune and optimize flow behavior in real-time.

Optimizing complex flows, such as convection-dominated problems and flows with moving fronts like shock waves or flames,
is challenging due to the nonlinear dynamics involved and the reliance on computationally intensive simulations with numerous degrees of freedom. 
To wit the primary goal of this project is to develop effective transport separation framework which can decompose the transport phenomena
into simpler processes such that efficient model order reduction techniques could then be effectively applied on the decomposed processes 
instead of the complex full process without sacrificing model precision.

This work presents a neural network-based methodology for the decomposition of transport-dominated fields using the shifted proper orthogonal decomposition (sPOD).
Classical sPOD methods typically require an a priori knowledge of the transport operators to determine the co-moving fields.
However, in many real-life problems, such knowledge is difficult or even impossible to obtain, limiting the applicability and benefits of the sPOD.
To address this issue, our approach estimates both the transport and co-moving fields simultaneously using neural networks.
This is achieved by training two sub-networks dedicated to learning the transports and the co-moving fields, respectively.
Applications to synthetic data and a wildland fire model illustrate the capabilities and efficiency of this neural sPOD approach,
demonstrating its ability to separate the different fields effectively.

Following successfull application of the neural network strategy we were able to obtain the desired transport separation as shown below for a toy example
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/NsPOD_toy.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Transport separation of two traveling waves.
</div>

Detailed theoretical aspects behind the network and more examples are given in our paper
## related publications
<div class="publications">
  {% bibliography -f papers -q @*[key=ZoBuKrMaSc24]* %}
</div>