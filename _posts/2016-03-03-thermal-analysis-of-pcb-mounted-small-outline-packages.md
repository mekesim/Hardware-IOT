---
ID: 250
post_title: >
  Thermal Analysis of PCB Mounted Small
  Outline Packages
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/250
published: true
post_date: 2016-03-03 11:30:26
---
<b>Robert Day, Analog Devices and Prasad Tota, Mentor Graphics</b>

How thermal analysis tools can be used for testing and evaluating the small outline packages found on reduced-sized PCBs in modern consumer devices.<span class="bigsmall strong">
</span>

Throughout the electronics industry, submicron feature size at the die level is driving package component sizes down to the design-rule level of the early technologies. Today’s integrated circuit (IC) package technology must deliver higher lead counts, reduced lead pitch, minimum footprint area, and significant reduced volume, which has led to semiconductor manufacturers developing the small outline package (SOP), surface-mount memory packaging.

SOP packages support the trend toward miniaturization by consuming one-third to one-half the volume of earlier packaging alternatives. SOP components are a logical choice for the small form factor of handheld instruments, portable communication devices, laptop and notebook PCs, disk drives, and numerous other applications. The mechanical dimensions of the power SOP (PSOP) package, combined with a heat spreading thermal mass (copper slug), make it a good choice for office automation, industrial controls, networking, and consumer applications that generate internal heat and are exposed to stressful temperature conditions.

The PSOP leads are located on the long side of the package, which leaves two sides of the package open. The open sides of the package can be used to route traces under the component, conserving board layers and simplifying board layout. Compared to older versions, the packages can be placed much closer to each other and to other components on the board.

When IC packages are downsized, thermal power density increases, and the heat-transfer path from the die to the external ambient needs to be optimized to allow for maximum possible power dissipation at the die while still ensuring the die temperature is under the maximum allowable value. Although PSOPs undergo tests for reliability under temperature stresses, electrical flow, and solderability, as well as mechanical inspection at the manufacturer before shipping, it would be time-consuming and expensive to physically test or design test boards to test a package in all its possible applications and configurations.

Computational fluid dynamics (CFD) software is useful in such situations because it can simulate and estimate the junction temperature (<em>T<sub>j</sub></em>) of the IC when attached to the PCB under various conditions, including different powering conditions, board conductivity, thermal via distribution, bill of materials, and the IC package construction itself. A CFD tool enables a mechanical or electrical engineer and/or IC designer to quickly see the effect of design changes from a thermal management perspective both qualitatively and quantitatively.

To test this, we performed computational thermal analysis of an Analog Devices high-speed, high-voltage, 1-A output drive amplifier, the ADA4870-1, PSOP mounted on a PCB,<sup>[1]</sup> using Mentor Graphic's CFD FloTHERM. Specifically, we wanted to identify the maximum power that could be dissipated on the die active area while keeping the <em>T<sub>j</sub></em> at less than 150 °C. We studied various environments to estimate this maximum power, for example, changing the board area, adding thermal vias, and attaching a heatsink.

This package can be surface-mounted on the board either slug down or slug up (Figure 1), depending on the direction of the formed leads. In a slug-down configuration, the component is surface-mounted on the primary side of the board where the copper slug is soldered to the top side of the board. In a slug-up configuration, the leads are soldered to the primary side of the board. For our experiment, we used a slug-down configuration; first with no heatsink, and then with a heatsink attached to the secondary side of the board with thermal grease between the board and the heatsink base.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=1" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-1.png" alt="Figure 1: The PSOP dimensions in millimeters, with the copper slug on the bottom.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 1: The PSOP dimensions in millimeters, with the copper slug on the bottom.</span></div>
</div>
For the CFD simulation, the test board we used was a six-layer board, with dimensions of 59 x 61 mm. We assumed that the copper coverage for each of the conducting layers was smeared uniformly within the layer’s volume. Based on this, we calculated the thermal conductivity (<em>k</em>) of each layer as a volume average based on the percent of copper coverage within an individual layer (Table 1). For further accuracy, we could also have processed the images for copper coverage within a layer to provide a conductivity mapping within the plane of the board.<sup>[2]</sup>
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=2" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Table-1.png" alt="Table 1: Board stack-up and percent of copper coverage.
" border="0" /></a>
<div><span class="docimagecaptiontext">Table 1: Board stack-up and percent of copper coverage.</span></div>
</div>
We recommend discretely modeling each of the conducting layers with orthotropic conductivity for the entire thickness of the board to accurately predict the value of the junction temperature. Modeling the layers discretely, rather than with a lumped model, captures the effect of heat spreading within the board more accurately for various heat-transfer paths.

<strong>Thermal simulation without a heatsink</strong>
We conducted the first set of simulations to study the thermal behavior of the PSOP mounted on the primary side of the board where the copper slug was soldered to the board. We kept the board horizontal with respect to gravity in an ambient temperature of 85 °C.

To emulate real working conditions, we applied heat to two-thirds of the top of the die. In the simulation, the junction temperature (<em>T</em><sub>j</sub>) was measured at the geometric centroid of this area, and case temperature (<em>T<sub>c</sub></em>) was measured at a point in the copper slug just above the soldered interface (Figure 2). It is possible to also monitor the temperature of the leads, plastic surface, or any given position to validate the computational results with available test data.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=3" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-2.png" alt="Figure 2: Temperature measurement locations.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 2: Temperature measurement locations.</span></div>
</div>
We added thermal vias under the slug to provide a more conductive path from the copper slug into the board. The vias were placed right under the copper slug because our numerical investigations revealed a small advantage of adding vias beyond the slug area. This also helps in lowering the manufacturing cost of the board.

We investigated two possible scenarios for thermal vias: one where the inner layers were isolated, and a second where the inner layers were stitched together. Stitching the inner layers lowers the junction temperature because a fraction of the heat entering the slug can spread in inner layers; however, including the inner layers raises the core body temperature of the board. So depending on the application, the inner layers could be isolated or used for thermal management. In this study, the secondary side of the board was completely covered with copper.

Figure 3 shows the temperature plots for the package in still air at 85 °C and thermal power <em>P</em> = 2 W with die-attach material of <em>k</em> = 1.6 W/mK [watts per meter kelvin]). We replaced the die-attach with the more conductive material, <em>k</em> = 50 W/mK, which significantly reduced the junction-to-case thermal resistance (<em>θ<sub>jc</sub></em>) of the package from 6.61 °C/W (celsius per Watt) to 1.12 °C/W.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=4" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-3.png" alt="Figure 3: Temperature plots for the package in still air at 85  degrees C.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 3: Temperature plots for the package in still air at 85 °C.</span></div>
</div>
<span class="bigsmall strong">

</span>

<strong>Thermal simulation with a heatsink</strong>
We soldered a heatsink to the back side of the board to increase the power dissipation through the package, using thermal grease between the board and heatsink. Adding the heatsink significantly reduced the junction-to-ambient thermal resistance (<em>θ<sub>ja</sub></em>) from 16 °C/W to 5.73 °C/W. Heat-flux plots for a plane cutting through the package show the heat spreading over a larger surface area hence reducing the junction temperature for a given value of thermal power (Figure 4).
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=5" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-4.png" alt="Figure 4: Heat-flux plots for a plane cutting through the package.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 4: Heat-flux plots for a plane cutting through the package.</span></div>
</div>
Table 2 shows the results for maximum power (<em>P<sub>max</sub></em>) allowed in the slug-down configuration in still air with and without a heatsink for the two die-attach materials. Based on these results, we focused our next study with the more conductive die-attach material (Cookson).
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=6" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Table-2.png" alt="Table 2: Thermal resistance for different die-attach materials.
" border="0" /></a>
<div><span class="docimagecaptiontext">Table 2: Thermal resistance for different die-attach materials.</span></div>
</div>
We wanted to find the shortest heatsink sufficient to dissipate 10 W of heat at the die. We used the parametric study capability in the CFD software to quickly set up and solve for different scenarios.<sup>[3]</sup> The variable parameter in this case was the heatsink fin height. The results are shown in Figure 5; junction temperature (<em>T<sub>j</sub></em>) is represented by circles and case temperature (<em>T<sub>c</sub></em>) by squares. We found that a heatsink with fin height of 10.36 mm is sufficient to dissipate 10 W.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=7" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-5.png" alt="Figure 5: Junction temperature (Tj) and case temperature (Tc) for different heatsink fin heights.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 5: Junction temperature (Tj) and case temperature (Tc) for different heatsink fin heights.</span></div>
</div>
These results prompted us to investigate further to find Pmax that could be dissipated if there were tighter constraints on the size of board and heatsink, and hence we reduced the size of both to 30 x 30 mm. We also studied the effect of different fin heights on junction-to-ambient thermal resistance, <em>θ<sub>ja</sub></em> (Table 3).
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=8" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Table-3.png" alt="Table 3: Thermal resistance vs fin height in still-air environment.
" border="0" /></a>
<div><span class="docimagecaptiontext">Table 3: Thermal resistance vs fin height in still-air environment.</span></div>
</div>
With forced airflow, the junction-to-ambient thermal resistance could be further reduced, allowing higher powers to be dissipated and <em>T<sub>j</sub></em> to be kept under 150°C. Figure 6 shows the package simulation in a forced-air environment. Table 4 shows the results for heatsink optimization in forced air. It is interesting to see that, with forced airflow of 2 m/s, the package could dissipate over 20 W of heat for a fin height of 21 mm and 17 W with fins just 10-mm high.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=9" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-6.png" alt="Figure 6: Package with heatsink in a forced-air environment
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 6: Package with heatsink in a forced-air environment</span></div>
</div>
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=10" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Table-4.png" alt="Table 4: Thermal resistance versus fin height in forced air. θja: junction-to-ambient thermal resistance, Pmax: maximum power.
" border="0" /></a>
<div><span class="docimagecaptiontext">Table 4: Thermal resistance versus fin height in forced air. θja: junction-to-ambient thermal resistance, Pmax: maximum power.</span></div>
</div>
We did a similar parametric study for the smaller heatsink with a base of 30 x 30 mm for different fin heights in forced air (Table 5). This smaller heatsink with 10-mm high fins (lower weight) offered the same performance as a larger heatsink with 5-mm fin height.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=11" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Table-5.png" alt="Table 5: Thermal resistance and maximum power for forced air. θja: junction-to-ambient thermal resistance, Pmax: maximum power.
" border="0" /></a>
<div><span class="docimagecaptiontext">Table 5: Thermal resistance and maximum power for forced air. θja: junction-to-ambient thermal resistance, Pmax: maximum power.</span></div>
</div>
Several parameters effect the thermal conductivity of the board in the region of the vias.<sup>[4]</sup>Creating a test board for every possible thermal via configuration and testing in a lab is practically infeasible. The CFD tool can be used to perform sensitivity studies of thermal performance to various via parameters, such as the pitch, plating thickness, and fill material (Figure 6). Such computational studies reduce the number of prototypes needed for testing or validation.

In a CFD program, it is computationally intensive to model each and every via discretely, so we took a lumped approach where we replaced the region of vias with a block of orthotropic conductivity that had in-plane conductivity (<em>k<sub>xy</sub></em>) and through-plane conductivity (<em>k<sub>z</sub></em>). A board-import tool in the software was used to calculate the <em>k<sub>xy</sub></em> and <em>k<sub>z</sub></em> of this via block, but we could also have calculated these values analytically.<sup>[2, 5]</sup>

Thermal vias with an outer diameter of 0.3 mm were studied. Figure 7 shows the sensitivity of thermal conductivity of via block to pitch and plating thickness (<em>t</em>). The dielectric material used in this calculation was FR4 (<em>k</em> = 0.3 W/mK), and the fill material was pure copper (<em>k</em> = 385 W/mK).
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=12" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-7.png" alt="Figure 7: Sensitivity to via pitch and plating thickness. kz: in-plane conductivity.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 7: Sensitivity to via pitch and plating thickness. kz: in-plane conductivity.</span></div>
</div>
Thermal simulations were conducted for PSOP in still air based on the conductivity values of the via cuboid, and results are shown in Figure 8. The results show that when plating thickness <em>t</em> is 75 µm or higher, even sparsely populated vias are sufficient. However, at low plating thickness, say 25 µm or lower, the vias need to be populated densely to ensure the component does not experience thermal failure.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=13" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-8.png" alt="Figure 8: Junction-to-ambient thermal resistance (θja) to via pitch and plating thickness in still air.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 8: Junction-to-ambient thermal resistance (θja) to via pitch and plating thickness in still air.</span></div>
</div>
<strong>Validating the simulation results</strong>
We conducted lab experiments to validate the CFD model results. The IC inside the PSOP package is capable of dissipating 10 Watts of power and has an integrated temperature monitor. The relationship of the voltage at monitor-to-die temperature is not an absolute temperature indicator. However, the change in voltage verses temperature is a reliable indicator of relative changes in die temperature. Calibrating the temperature-monitor voltage verses temperature function was the first step in understanding die temperature used to determine thermal resistance.

The PCB we used in the lab was FR4-grade with six layers of copper and exposed copper planes, onto which the ADA4870-1 PSOP package was soldered and heatsinks were mounted. We used copper-filled thermal vias to conduct heat from the IC side to the bottom of the board where a precise temperature sensor was soldered directly below the thermal slug of the PSOP package onto the back side of the PCB. We bolted a heatsink to the back side that straddled the sensor using silicon grease as a thermal interface material between the heatsink and the PCB. We used commercially available heatsinks (Table 6).

Then, we placed the PSOP assembly into a still-air chamber using automated instruments and power supplies and allowed it to soak overnight without any power applied. The ADA4870-1 IC and temperature sensor were then both turned on and measurements of the PSOP temperature-monitor voltage and sensor-trimmed PTAT (power sub-threshold proportional to absolute temperature) current were made immediately. The temperature-monitor voltage measurement was related to the absolute temperature indicated by the temperature sensor. We repeated this process at several temperatures to develop a calibration of the temperature-monitor voltage to absolute temperature (Figure 9).
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=14" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Figure-9.jpg" alt="Figure 9: Temperature monitor (TM) volts versus sensor temperature.
" border="0" /></a>
<div><span class="docimagecaptiontext">Figure 9: Temperature monitor (TM) volts versus sensor temperature.</span></div>
</div>
Using a linear fit to the curve (<em>T</em> [°C] = <em>TM</em> [<em>V</em>] – 1.93/0.003), we converted the voltage to temperature. We conducted additional steady-state tests to reveal the practical limits of power dissipation (maximum power) as a function of the applied heatsink. As shown in Table 6, large heatsinks are necessary when operating at the limits of power dissipation for the tested IC. We calculated the junction-to-ambient thermal resistance (<em>θ<sub>ja</sub></em>) from the measured data by the following relations ships at steady state: <em>θ<sub>ja</sub></em> = Δ<em>TM</em>(<em>V</em>) − 1.93 (<em>V</em>) − 0.003 <em>V</em>/°C Δ <em>Power</em> (<em>W</em>) = °C/W.
<div class="docimage" align="center"><a href="http://www.eetimes.com/author.asp?section_id=36&amp;print=yes&amp;doc_id=1328282&amp;image_number=15" target="new"><img class="docimage" src="http://www.mekesim.com/wp-content/uploads/2016/03/Table-6.png" alt="Table 6: Thermal testing versus simulation results. θja: junction-to-ambient thermal resistance, Pmax: maximum power.
" border="0" /></a>
<div><span class="docimagecaptiontext">Table 6: Thermal testing versus simulation results. θja: junction-to-ambient thermal resistance, Pmax: maximum power.</span></div>
</div>
The results showed the CFD simulation to be in good agreement with the lab test results with a heatsink mounted, where the dominant heat-transfer path is from the die into the heatsink. There is a higher difference for simulations with no heatsink, where an appreciable fraction of the total heat travels through bond wires and leads into the top layer of the PCB. This difference can be attributed to assumptions in simulation we made in modeling the leads and bond wires in the simulation.

<strong>A complimentary tool</strong>
With these experiments, we found that CFD software is a complimentary tool to laboratory testing, enabling quick parametric and design optimization studies in the thermal design. Such data is useful for studying electronics in harsh environments with increasing demands on power. The next step would be to analyze the transient behavior of the package and thermal characterization using structure functions generated by hardware testing, such as the Mentor Graphics T3Ster. A transient thermal simulation validated by test data would go a long way in simulating the transient response of a package for various powering conditions and reduce the number of laboratory tests needed.

<strong>References</strong>

1. Analog Devices, High Speed, High Voltage, 1 A Output Drive Amplifier ADA4870, http://www.analog.com/media/en/technical-documentation/data-sheets/ADA4870.pdf

2. Blackmore, Byron, “Validation and sensitivity analysis of an image processing technique to derive thermal conductivity variation within a printed circuit board,” Semiconductor Thermal Measurement and Management Symposium, 25th Annual IEEE SEMI-THERM Symposium, San Jose, CA, March 2009, pp.76-86.

3. Bornoff, Robin, Blackmore, Byron, Parry, John, “Heat Sink Design Optimization using the Thermal Bottleneck Concept,” Proceedings of 28th IEEE SEMI-THERM Symposium, San Jose, CA, March 2011, pp.76-80.

4. Li R.S., “Optimization of thermal via design parameters based on an analytical thermal resistance model,” <em>Thermal and Thermomechanical Phenomena in Electronic Systems</em>, 1998. ITHERM 1998, pp 475-480.

5. Incropera, F., Dewitt, D., et al., <em>Fundamentals of Heat and Mass Transfer</em>, John Wiley and Sons (New York, 1993), pp. 65-67.

<em>Note: Mentor Graphics sells a CFD tool called FloTHERM.</em>