---
layout: post
title:  "Actuator disk model correction published in Wind Energy"
date:   2019-07-17 12:00:00 -0500
categories: Research
---

Our paper "[Filtered actuator disks: Theory and application to wind turbine models in large eddy simulation](https://doi.org/10.1002/we.2376)" was published in the journal *Wind Energy*. By *Carl R. Shapiro, Dennice F. Gayme, and Charles Meneveau*

In most actuator disk model (ADM) implementations, spatial filtering is required to smoothly distribute the applied force distribution on discrete grid points. The filtered ADM overestimates power by upwards of 10% on coarse grids. In this paper, we develop a filtered actuator disk theory that correctly predicts the power coefficient in these simulations at different filter widths Δ. A correction factor is then derived analytically that collapses the power coefficients onto the theoretical power curve. The simulation data and LaTeX source can be found on [Github](https://github.com/crshapiro/ShapiroGaymeMeneveau-WindEnergy-2019). Corrected ADM simulations are now available in the large eddy simulation code [LESGO](https://lesgo.me.jhu.edu).

![adm-correction](/img/adm-correction.png)
*Left: Comparison of filtered actuator disk theory (lines) and simulations (symbols) to axial momentum theory (⋯⋯). Right: Comparison of corrected ADM simulations (symbols) to axial momentum theory (⋯⋯)*
