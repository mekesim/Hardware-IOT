---
ID: 164
post_title: >
  Compact Component Models and a Problem
  of Exchange
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/164
published: true
post_date: 2016-01-31 18:53:19
---
<i>Tom Gregory, 6SigmaET Product Specialist</i>

The development and use of compact component models or compact thermal models (CTMs) has been a critical element to produce accurate thermal analysis and simulation of electronic components and assemblies, and not only in the initial design of a system but also in the test and validation phase.<span id="more-4567"></span>

CFD (Computational Fluid Dynamics) based thermal analysis tools have been around now for the best part of a quarter of a century and the importance of thermal models became quickly apparent to users and the industry in general. The standard junction-to-ambient thermal resistance often quoted on semiconductor component datasheets is not nearly good enough and does not really interpret how heat is dispersed from a silicon chip’s package. On the other hand, a fully detailed thermal model (DTM) that more or less exactly replicated the physical geometry of a chip package was and still is IP that semiconductor vendors do not wish to disclose. In addition to which, this is a model that would be impractical to solve by a CFD tool, especially for a board-level simulation involving hundreds of components if each package part was defined in detail.

<img class="alignnone size-full wp-image-165" src="http://en.mekesim.com/wp-content/uploads/2016/01/6SigCompactComponent.png" width="252" height="146" alt="6SigCompactComponent" />

This need for a better representation of component models led to the set up in the mid-1990s of the European Delphi project (Development of Libraries and PHysical models for an Integrated design environment). The Delphi mission, in conjunction with its successor SEED and PROFIT projects, was to create compact thermal models that comprised fewer elements than a DTM and did not disclose package IP, but offered an abstracted representation with a high degree of accuracy. In addition it should require significantly less computational time in thermal simulation. Importantly it also needed to be boundary condition independent: in fact, Delphi set a number of boundary conditions (initially 48 but revised down to 38 cases) with using uniform heat transfer coefficients to predict temperature at a number of discrete points on a package such as at the junction, regardless of the environment and potentially any forced-convection cooling system.

In 2008, the methodology for relatively simple two-resistor thermal models (junction-to-board and junction-to-case) and more complex resistance/capacitance-network compact models was absorbed into JEDEC standards (JESD15-3 and JESD15-4, respectively). These compact models have been shown to be highly accurate, often within 4 per cent of maximum temperature. In addition, the Delphi project also defines measurement calibration to enable engineers to validate compact thermal models.

However, as one can imagine, this does not mean all thermal analysis problems are now solved for all eternity. For example, the widespread use of packaging technologies such multi-chip modules and also the development of Dynamic Compact Thermal Model (DCTM) for the simulation of transient thermal phenomena are major issues today for engineers working in thermal simulation and analysis.

A further issue, and a very important one, is the creation and distribution of compact models. Sometimes models of specific components are available in a numerical tabular form or occasionally in a proprietary file format for a particular software tool. What is required to drive our industry forward, and we strongly support this initiative, is a vendor neutral format to report and share compact models. In fact, this initiative is currently going through a JEDEC standards committee, but results may take some time to come through.

<img class="alignnone size-full wp-image-166" src="http://en.mekesim.com/wp-content/uploads/2016/01/6SigServer-airflow.png" width="252" height="164" alt="" />

The latest version of our 6SigmaET tool – Release 9 – builds in full support for compact component models. The tool allows a specific component to be represented at different modelling levels including detailed geometry, two-resistor thermal models, compact resistance/capacitance network models (DCTM) or as just a simple block.  This allows users to select the appropriate modelling level for the analysis they are carrying out.

Unfortunately few people are using compact models today and certainly, the industry needs an increased commitment from component manufacturers to provide them, and in an industry-standard format, which can only accelerate and proliferate usage. This will bring significant benefits to all, as there is no doubt that the increased adoption of the compact component models will enhance the accuracy of thermal simulations across the electronics industry.

<em>For more information please visit <a href="http://www.6sigmaet.info/">www.6sigmaet.info</a></em>