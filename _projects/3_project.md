---
layout: page
title: Optimal control
description: Optimal control of transport dominated problems with reduced order modeling
img: assets/img/OC.png
importance: 3
category: work
---

Optimal control for transport-dominated systems becomes tractable and practical when paired with 
carefully constructed reduced-order models. Transport phenomena (shocks, moving vortices, 
concentration fronts) concentrate energy in low-dimensional, moving coherent structures that 
standard global bases struggle to represent. However, nonlinear model order reduction techniques like the 
sPOD-Galerkin method capture those features with far fewer degrees of freedom. 
That dramatic reduction in state dimension cuts the cost of forward 
and adjoint solves by orders of magnitude, enabling faster gradient evaluation, real-time or 
many-query optimization, and easier incorporation of constraints and parameter dependencies. 
When designed and validated carefully, ROM-based optimal control preserves essential physics 
(stability, conservation) while making control synthesis, sensor/actuator placement, and 
uncertainty-aware design feasible for problems that would otherwise be computationally intractable.

Our work presents an in-depth theoretical and numerical analysis of an example transport problem 
applied in an optimal control context and is shown in our paper
## related publications
<div class="publications">
  {% bibliography -f papers -q @*[key=BrBuSc]* %}
</div>