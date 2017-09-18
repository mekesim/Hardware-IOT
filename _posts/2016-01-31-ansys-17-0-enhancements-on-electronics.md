---
ID: 174
post_title: ANSYS 17.0 Enhancements on Electronics
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/174
published: true
post_date: 2016-01-31 19:08:34
---
ANSYS 17.0 employs a new modeling approach based on electrical parts and data that can help in predicting warping and fatigue of printed circuit boards (PCBs) under thermal loading.

<img class="img-responsive" src="http://en.mekesim.com/wp-content/uploads/2016/01/1_qq9txt.jpg" alt="Multiphysics simulation based on ECAD is necessary to accurately calculate DC current flow, determine temperature fields and predict thermal-mechanical stresses and deformation. (Image courtesy of ANSYS.)" />

Multiphysics simulation based on ECAD is necessary to accurately calculate DC current flow, determine temperature fields and predict thermal-mechanical stresses and deformation. (Image courtesy of ANSYS.)

Until now, structural analysis of detailed PCBs usually meant simplifying existing models or enduring long set-up and solve times. Both efforts can impact the quality and accuracy of subsequent simulations.

<strong>Metal Trace Mapping</strong>

In the past, users had the choice of approximating PCBs with a single material.
<ul>
	<li>An average property value applied across the entire board, such as Young’s modulus, would not be accurate in areas stiffened by large components or solder joints. This “smearing” of properties is often too much of a simplification to be realistic but doing otherwise was far too time-consuming.</li>
	<li>An engineer would have to try to map layouts onto models using images or manually apply layout details onto geometry. The new ability to take electrical CAD (ECAD) data and directly map trace information onto a structural finite element analysis (FEA) model means higher fidelity PCB simulations can be built more quickly.</li>
</ul>
A hexahedral mesh is initially created which discretizes each layer of the PCB, ignoring the interfaces between the thousands of metal traces and silicon. Next, the ECAD information is imported and the material information for each element is calculated and mapped onto the mesh. The result is a fast, easily defined mesh and mapping that looked like it would take just minutes to set up.
<div align="center">

<img class="img-responsive" src="http://en.mekesim.com/wp-content/uploads/2016/01/2_aegypo.jpg" alt="Trace metal mapping simulates PCB properties under thermal loading. (Image courtesy of ANSYS.)" />
<div>Trace metal mapping simulates PCB properties under thermal loading. (Image courtesy of ANSYS.)</div>
</div>
Using ANSYS Icepak, the temperature fields on and around the PCB are determined using computational fluid dynamics (CFD). Users can apply the temperature fields to the model as input conditions for a coupled thermal-stress analysis in ANSYS Mechanical. Model creation and model analysis can be performed on a single platform.

<strong>DC Current Calculations</strong>

First, ANSYS Slwave software is used to compute DC currents and voltages throughout the PCB. Slwave calculates the current density throughout the board which determines Joule heating. Joule heating is the process by which heat is produced due to electrical resistance when an electrical current flows through a conductor.

<strong>Thermal Simulations</strong>

ANSYS 17.0 integrates and automates bidirectional workflow between Slwave and Icepak systems, thereby making it easier to determine Joule heating. This function imports the board, trace mapping and current density predictions, and sets the thermal boundary conditions for Icepak. Icepak then uses the trace map to calculate the orthotropic thermal conductivity of the PCB.

Much of the heat generated on the PCB is dissipated via convection or radiation from the board and the material makeup of the PCB has a directional nature. Icepak solves fluid flow equations and includes all modes of heat transfer—conduction, convection, and radiation—to compute temperatures at every point in the solution domain. The macro exports the resulting temperatures from Icepak back to Slwave which updates the electrical properties for the DC solution based on the temperature filed. Slwave then recalculates the DC field and exports it to Icepak. This iterative process continues until the power dissipation and temperature results have converged.

<strong>Trace Metal Fraction Determination</strong>

ANSYS 17.0 allows users to build the structural model for computation of deformation, strain and stress. ANSYS SpaceClaim reads the ECAD geometry, converting it into a 3D model of simplified layers, mapping and metal dielectric properties onto the layers. The geometry is opened in ANSYS Mechanical where it is meshed due to the layer nature of the geometry. Each layer can have a combination of metal and dielectric properties.
<div align="center">

<img class="img-responsive" src="http://en.mekesim.com/wp-content/uploads/2016/01/3_m0mnwe.jpg" alt="Full geometry in ANSYS SpaceClaim Direct Modeler. (Image courtesy of ANSYS.)" />
<div>Full geometry in ANSYS SpaceClaim Direct Modeler. (Image courtesy of ANSYS.)</div>
</div>
Some elements can be entirely metal, others entirely dielectric, and others a combination of metal and dielectric. The resulting mesh is a simpler swept hexahedral mesh that users can adjust to suit their purposes. A higher mesh density will create a more accurate representation of the model and take more time to compute. Conversely, a lower mesh density will take less time to compute and be less accurate.

Users can also create a color-coded, source point cloud that takes advantage of the data map but is independent of the mesh. The point cloud assesses if a point is metal, dielectric, or a combination of both. Users can make use of point cloud visualization to asses where the import data is and how it aligns to the created mesh.

<strong>Calculating Thermal-Mechanical Stress and Deformation</strong>

The resulting model with the mesh is the basis of a structural simulation with appropriate material properties taken into consideration. Its solution will quantify thermal stresses, strains and deformation at any location on the PCB. Knowing these locations, users can determine whether some aspects of the model are at risk of failure, including attachment locations such as solder balls. Icepak simulations also account for the cooling conditions of the board. Users can also perform dynamic analysis to investigate modal frequencies and effects of random vibration on the PCB with thermal loading taken into account.

This new, multiphysics approach helps engineers efficiently, accurately and quickly simulate the effects of thermal and mechanical loading. They can use this method to evaluate proposed designs, determine whether thermal or mechanical loading might cause problems and evaluate the effect of proposed design changes in solving these problems. This method also makes it possible to design products that are free of thermal loading problems at the early stages of the design process, thus reducing product failures and warranty claims. They can also help lower time to market and engineering expenses by avoiding expensive late-stage design changes.

The ability to model complex material properties can increase model resolution and save valuable time versus traditional and manual means. According to ANSYS Inc., using ANSYS 17.0, model accuracy and processing speed are significantly increased, leading to a tenfold improvement in which simulations are solved—minutes, not hours or even days.

The new release of the flagship ANSYS 17.0 software is now available. ANSYS will be offering an ANSYS 17.0 <strong><a href="http://www.engineering.com/LinkClick.aspx?link=http%3a%2f%2fwww.ansys.com%2fProducts%2fRelease-Highlights%2fwebinar-16-02-18-10x-more-reliable-electronic-systems%3futm_source%3dengineeringdotcom%26utm_medium%3dreferral%26utm_campaign%3dr17-str1-applebox327&amp;tabid=6011&amp;portalid=0&amp;mid=429" target="_blank">webinar series</a></strong> on Feb. 18.

<img class="img-responsive" src="http://en.mekesim.com/wp-content/uploads/2016/01/4_qymkxf.jpg" alt="" />

Laura Carrabine has been writing about the CAD/CAM/CAE industry since the late 1980s. She is a former editor of <em>Computer-Aided Engineering</em>, <em>Flowfront</em> (a publication for the plastic injection molding community) and <em>Design World</em>.

<em>ANSYS has sponsored this post. They have no editorial input. All opinions are mine. — Laura Carrabine</em>