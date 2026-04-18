---
layout: page
title: Research
---

My past and ongoing projects

---

### Early Earth Dynamics

Plate tectonics is one of the defining features that makes Earth unique among the rocky planets. It drives mountain building, volcanism, and the long-term cycling of materials between Earth's surface and deep interior. At the heart of this system lies subduction, where one tectonic plate sinks beneath another. Despite its importance, we still don't fully understand how or when subduction first began nor what conditions allowed the first stable continents to emerge.

A central focus of my research is understanding how subduction initiated and evolved during Earth's early history. My past work suggests that continents alone are not sufficient to initiate subduction, which raises deeper questions about what combination of conditions made it possible on the early Earth.

I am also interested in how early subduction differed from what we observe today. Higher mantle temperatures, more vigorous convection, and differences in the composition and structure of early lithosphere could have produced subduction zones that were more transient, shallower, or structurally distinct from their modern counterparts. Understanding these differences is key to reconstructing the tectonic environment in which the first continents formed and stabilized.

<div style="text-align: center;">
  <img src="/assets/img/jgrb56955-fig-0009-m.jpg" width="50%" alt="Subduction initiation regime diagram">
  <br>
  <em>Regime diagram showing the conditions required for continent-induced subduction initiation, as a function of continental thickness and viscosity jump (μ_jump). Subduction initiation is only possible to the right of the boundary, requiring sufficiently thick and rheologically distinct continental lithosphere. From Choi and Foley (2024)</em>
</div>

---

### Fluid Migration and Continental Crust Formation

Some of the oldest rocks on Earth tell us that continental crust existed very early in Earth's history. Yet the exact mechanisms responsible for producing this crust remain poorly understood. I use numerical models of subduction to investigate how fluids released from a downgoing slab migrate through the mantle wedge and contribute to the generation of buoyant, felsic melts that may have built the earliest continents.

To capture these dynamics realistically, I employ two-phase flow models that explicitly couple solid mantle flow with fluid migration. This approach goes beyond solid-only models, which cannot represent the feedback between dehydration, fluid pathways, and melt production. By tracking porosity fields and fluid fluxes within a subduction zone framework, I aim to link slab dynamics, fluid transport, and TTG-like melt generation in a unified model — and to explore how those processes may have varied under early Earth conditions.

<div style="text-align: center;">
  <img src="/assets/img/porosity_diff2.png" width="80%" alt="Porosity field snapshots from two-phase flow subduction models">
  <br>
  <em>Porosity field (φ) from subduction models with mantle potential temperatures of T₀ = 1673 K (left) and T₀ = 1900 K (right) at t ≈ 3,000 years. Overlaid isotherms highlight the slab geometry and mantle wedge structure. Higher mantle temperatures produce more focused fluid migration near the slab interface.</em>
</div>

---

### Deep Learning-Based Subduction Zone Detection

Numerical simulations of mantle convection generate large volumes of complex image data, and identifying subduction zones within them can be time-consuming and difficult to automate with traditional threshold-based methods. To address this, I developed a deep learning toolkit that uses a Fully Convolutional Network (FCN) to detect and track subduction zones directly from model output images.

The FCN is trained on labeled examples to recognize the spatial patterns associated with subduction, and once trained, it can automatically segment new model outputs to identify subduction zones, even in models with irregular or short-lived features. The result is a scalable, flexible framework that performs well across a range of model configurations and dynamic regimes.

<div style="text-align: center;">
  <img src="/assets/img/jgrb70235-fig-0002-m.jpg" width="80%" alt="FCN subduction zone detection">
  <br>
  <em>Comparison of FCN-predicted subduction zone masks (top) against SAM-generated ground truth labels (middle) and the corresponding RGB model images (bottom), for two examples with different subduction geometries. The FCN closely reproduces the ground truth in both cases. From Choi and Foley (2026)</em>
</div>

Beyond subduction detection, this framework is designed to generalize (e.g., mantle plumes in convection simulations, mineral phases in microscopy images, impact craters in planetary surface data, and other geoscientific pattern recognition tasks). Please contact me if you're interested in collaboration!

The code is openly available:

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17518757.svg)](https://doi.org/10.5281/zenodo.17518757) &nbsp; [![GitHub](https://img.shields.io/badge/GitHub-heec12%2FSZ--detection-181717?logo=github)](https://github.com/heec12/SZ-detection)
