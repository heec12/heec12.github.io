---
layout: page
title: Research
---

My research asks how Earth became the planet it is today. There are three big questions guiding my work: How did plate tectonics begin? What did subduction look like when Earth was younger and hotter? And how did the first continents form?

No single method can answer questions that span geodynamics, petrology, and data science, so I combine geodynamic models, thermodynamic models, and machine learning. On the machine learning side, I develop tools that automate the analysis of large simulation datasets and surrogate models that make forward modeling faster, so I can explore far more conditions than full simulations alone would allow.

### How did plate tectonics begin?

Plate tectonics is one of the defining features that makes Earth unique among the rocky planets. It drives mountain building, volcanism, and the long-term cycling of materials between Earth's surface and deep interior. At its heart is subduction, where one tectonic plate sinks beneath another. Yet we still don't know how or when subduction first began.

My past work using numerical models of subduction initiation shows that continents alone are not sufficient to start subduction. That result narrows the possibilities and raises the next question: what combination of conditions made subduction possible on the early Earth?

<div style="text-align: center;">
  <img src="/assets/img/jgrb56955-fig-0009-m.jpg" width="50%" alt="Subduction initiation regime diagram">
  <br>
  <em style="font-size: 0.75em;">Regime diagram showing the conditions required for continent-induced subduction initiation, as a function of continental thickness and viscosity jump (μ_jump). Subduction initiation is only possible to the right of the boundary, requiring sufficiently thick and rheologically distinct continental lithosphere. From Choi and Foley (2024)</em>
</div>

---

### What did early subduction look like?

Higher mantle temperatures, more vigorous convection, and differences in the composition of early lithosphere could have produced subduction zones that were more transient, shallower, or structurally distinct from their modern counterparts. Reconstructing these differences is key to understanding the tectonic environment in which the first continents formed.

One way to probe ancient subduction is to follow the water. Subducting slabs carry water into the mantle bound in hydrous minerals, and where that water is released affects melting, slab behavior, and the long-term exchange of water between Earth's surface and interior. I couple geodynamic models of Archean subduction with thermodynamic phase-equilibrium modeling to estimate how much water ancient oceanic crust could carry and where it would have been released. Because early oceanic crust was likely more Mg-rich than today's, I explore a range of plausible compositions rather than relying on a single assumed one.

<div style="text-align: center;">
  <img src="/assets/img/pt_maps_webpage.png" width="100%" alt="Bound H2O in subducting Archean oceanic crust">
  <br>
  <em style="font-size: 0.75em;">Bound water in subducting Archean oceanic crust, from thermodynamic modeling combined with slab pressure-temperature paths from a geodynamic model. Left and middle: bound H₂O in the upper and lower crust as a function of pressure and temperature, with slab paths in red, for lower-MgO (top) and higher-MgO (bottom) crust. Right: bound H₂O along the slab. Higher-MgO crust carries more water and releases more of it between 1 and 5 GPa.</em>
</div>

---

### How did the first continents form?

Some of the oldest rocks on Earth tell us that continental crust existed very early in Earth's history. Yet the exact mechanisms responsible for producing this crust remain poorly understood. I use numerical models of subduction to investigate how fluids released from a downgoing slab migrate through the mantle wedge and contribute to the generation of buoyant, felsic melts that may have built the earliest continents.

To capture these dynamics realistically, I employ two-phase flow models that explicitly couple solid mantle flow with fluid migration. Unlike solid-only models, this approach can represent the feedback between dehydration, fluid pathways, and melt production. By tracking porosity fields and fluid fluxes within a subduction zone framework, I link slab dynamics, fluid transport, and TTG-like melt generation in a single framework, and to explore how those processes may have varied under early Earth conditions.

<div style="text-align: center;">
  <img src="/assets/img/porosity_diff2.png" width="80%" alt="Porosity field snapshots from two-phase flow subduction models">
  <br>
  <em style="font-size: 0.75em;">Porosity field (φ) from subduction models with mantle potential temperatures of T₀ = 1673 K (left) and T₀ = 1900 K (right) at t ≈ 3,000 years. Overlaid isotherms highlight the slab geometry and mantle wedge structure. Higher mantle temperatures produce more focused fluid migration near the slab interface.</em>
</div>

---

### New tools for old questions

Numerical simulations of mantle convection generate large volumes of complex image data, and identifying subduction zones within them can be time-consuming and difficult to automate with traditional threshold-based methods. To address this, I developed a deep learning toolkit that uses a Fully Convolutional Network (FCN) to detect and track subduction zones directly from model output images.

Once trained on labeled examples, the FCN segments new model outputs automatically, including models with irregular or short-lived features. This turns a visual judgment into a reproducible measurement, making it possible to ask when, where, and how often subduction occurs across large sets of simulations. I am now extending this approach to surrogate models that approximate expensive forward simulations, making it feasible to explore much broader parameter spaces.

<div style="text-align: center;">
  <img src="/assets/img/jgrb70235-fig-0002-m.jpg" width="80%" alt="FCN subduction zone detection">
  <br>
  <em style="font-size: 0.75em;">Comparison of FCN-predicted subduction zone masks (top) against SAM-generated ground truth labels (middle) and the corresponding RGB model images (bottom), for two examples with different subduction geometries. The FCN closely reproduces the ground truth in both cases. From Choi and Foley (2026)</em>
</div>

Beyond subduction detection, this method is designed to generalize (e.g., mantle plumes in convection simulations, mineral phases in microscopy images, impact craters in planetary surface data, and other geoscientific pattern recognition tasks). Please contact me if you're interested in collaboration!

The code is openly available:

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17518757.svg)](https://doi.org/10.5281/zenodo.17518757) &nbsp; [![GitHub](https://img.shields.io/badge/GitHub-heec12%2FSZ--detection-181717?logo=github)](https://github.com/heec12/SZ-detection)
