---
layout: page
title: sPOD-NN
description: Model order reduction of a wildland fire model with deep learning methods
img: assets/img/Var40_Nonlinear.png
importance: 1
category: work
---


Since global warming has started wreaking havoc on our planet, scientists are actively trying to study its impacts on our environment.
Forests are the one part of our ecosystem that are experiencing the most amount of damage due to the warming.
Frequent wildfires have started to decimate the flora and fauna in many parts of the world and has a far-reaching consequence for life on our planet.

To tackle such issues world governments are investing heavily in research to study the wildfire behaviour and come up with 
mitigating steps to prevent further loss.

This project deals with one such research topic where we predict the spread of the wildfires in a computationally efficient way by combining our knowledge of the 
wildfire behaviour with the current advanced scientific methods like reduced order modelling and artificial intelligence.

However, to get computational speeds ups the reduced order model should be low-dimensional which for transport-dominated systems like the wildfire model is not the case. 
For the last few years, multiple methods have emerged to circumvent this problem. 
A recent method shifted proper orthogonal decomposition (sPOD), decomposes the high-dimensional solution field into multiple 
co-moving low-dimensional fields following which we can either use conventional model order reduction methods or purely 
non-intrusive machine learning-based methods to predict the solution.

By applying the sPOD to the wildfire model and predicting the solution with neural networks we get a significantly better reduced-order result with computational savings.

A detailed description of this project is shown in <a href="https://www.tu.berlin/en/fgmso/research/projects/model-reduction-for-multiple-transported-fronts-with-topological-changes">my TU berlin page</a> 
and a novel study of the results is given in our paper.
## related publications
<div class="publications">
  {% bibliography -f papers -q @*[key=BuKrRe23]* %}
</div>
