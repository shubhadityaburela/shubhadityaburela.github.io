---
layout: page
title: sPOD-NN
description: Model order reduction of a wildland fire model with deep learning methods
img: assets/img/Var40_Nonlinear.png
importance: 1
category: work
---

[//]: # (Every project has a beautiful feature showcase page.)

[//]: # (It's easy to include images in a flexible 3-column grid format.)

[//]: # (Make your photos 1/3, 2/3, or full width.)

[//]: # ()
[//]: # (To give your project a background in the portfolio page, just add the img tag to the front matter like so:)

[//]: # ()
[//]: # (    ---)

[//]: # (    layout: page)

[//]: # (    title: project)

[//]: # (    description: a project with a background image)

[//]: # (    img: /assets/img/12.jpg)

[//]: # (    ---)


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

[//]: # (<div class="row">)

[//]: # (    <div class="col-sm mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (    <div class="col-sm mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (    <div class="col-sm mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (</div>)

[//]: # (<div class="caption">)

[//]: # (    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.)
[//]: # (</div>)

[//]: # (<div class="row">)

[//]: # (    <div class="col-sm mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/Tnonlinear-mixed.png" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (</div>)

[//]: # (<div class="caption">)

[//]: # (    The top two plots show the temperature profiles at two different time-instances. The bottom two plots show the cross-sectional views of the profile at those time-instances with the prediction results for sPOD-NN, POD-NN, and sPOD-I procedures.)

[//]: # (</div>)

[//]: # ()
[//]: # ()
[//]: # (More detailed analysis and the results can be found in our publication \cite{BuKrRe23})

[//]: # (You can also put regular text between your rows of images.)

[//]: # (Say you wanted to write a little bit about your project before you posted the rest of the images.)

[//]: # (You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.)

[//]: # ()
[//]: # ()
[//]: # (<div class="row justify-content-sm-center">)

[//]: # (    <div class="col-sm-8 mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (    <div class="col-sm-4 mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (</div>)

[//]: # (<div class="caption">)

[//]: # (    You can also have artistically styled 2/3 + 1/3 images, like these.)

[//]: # (</div>)

[//]: # ()
[//]: # ()
[//]: # (The code is simple.)

[//]: # (Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` &#40;read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system&#41;.)

[//]: # (To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.)

[//]: # (Here's the code for the last row of images above:)

[//]: # ()
[//]: # ({% raw %})

[//]: # (```html)

[//]: # (<div class="row justify-content-sm-center">)

[//]: # (    <div class="col-sm-8 mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (    <div class="col-sm-4 mt-3 mt-md-0">)

[//]: # (        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %})

[//]: # (    </div>)

[//]: # (</div>)

[//]: # (```)
[//]: # ({% endraw %})
