---
layout: page
title: Research
permalink: /research/
---
Growing renewable energy production is putting increased stress on traditional electric power systems. By displacing conventional power sources, wind energy is reducing participation in important [ancillary services](http://www.pjm.com/markets-and-operations/ancillary-services.aspx") that maintain grid stability. My research focuses on developing control algorithms to provide one type of ancillary service, secondary frequency regulation, where participating power plants track a power reference signal sent by the power grid operator.


![Block diagram](/img/block-diagram.png)
*Block diagram of controlled wind farm showing receding horizon controller (top left block), wind farm (top right block), and state estimation (bottom block).*

We use a model-based receding horizon controller (also known as model predictive control) to track a secondary frequency regulation signal. Large eddy simulations (LES) are used as a computational test bed to test the performance of the control algorithm. Closed-loop feedback through ensemble Kalman filtering is used to correct modeling errors. Example results for a controlled 84-turbine wind farm are shown below.

![Control results](/img/enkf-rhc.png)
*Total wind farm power output showing reference signal (<font color="red">&mdash;&mdash;</font>), controlled wind farm (&mdash;&mdash;), and uncontrolled wind farm (<font color="gray">&mdash;&mdash;</font>).*
