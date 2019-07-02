---
layout: page
title: Research
permalink: /research/
---
**Wind farm control algorithms for improved power grid integration**
Growing renewable energy production is putting increased stress on traditional electric power systems. By displacing conventional power sources, wind energy is reducing participation in important [ancillary services](http://www.pjm.com/markets-and-operations/ancillary-services.aspx") that maintain grid stability. My research focuses on developing control algorithms to provide one type of ancillary service, secondary frequency regulation, where participating power plants track a power reference signal sent by the power grid operator.

![Block diagram](/img/block-diagram.png)
*Block diagram of controlled wind farm showing receding horizon controller (top left block), wind farm (top right block), and state estimation (bottom block).*

We use a model-based receding horizon controller (also known as model predictive control) to track a secondary frequency regulation signal. Large eddy simulations (LES) are used as a computational test bed to test the performance of the control algorithm. Closed-loop feedback through ensemble Kalman filtering is used to correct modeling errors. Example results for a controlled 84-turbine wind farm are shown below.

![Control results](/img/enkf-rhc.png)
*Total wind farm power output showing reference signal (<font color="red">&mdash;</font>), controlled wind farm (&mdash;), and uncontrolled wind farm (<font color="gray">&mdash;</font>).*

**Wind farm wake modeling**
Design and control studies rely on engineering models that can be easily computed and optimized because high-fidelity simulations are too computationally expensive to be practical. Our wake model is derived directly from the Reynolds-averaged mean momentum equations, yielding a one-dimensional partial differential equation that governs the velocity deficit in the wake \\(\delta u\\)

\\[ \frac{\partial \delta u_i}{\partial t} + U_\infty \frac{\partial \delta u_i }{\partial x} = - w(x) \,\delta u_i(x,t) + \,S_i \, G(x). \\]

This model provides the basis for the wind farm control algorithms described above.

**Lifting line model of yawed wind turbines**
Yawing of wind turbines has the potential to increase wind farm power production by deflecting wakes away from downstream turbines. A practical, yet accurate, aerodynamic theory can be found by treating the yawed wind turbine as a porous lifting surface. This approach yields accurate predictions for the magnitudes of the transverse velocity and the axial velocity deficit, the circulation of the shed counter-rotating vortex pair.

![Yawed turbine](/img/yaw.png)
*Comparison of (a) transverse velocity, (b) disk-averaged velocity, (c) streamwise velocity, and (d) skewness angle measured in simulations (squares) with present theory (solid black line) and prior models (other lines).*
