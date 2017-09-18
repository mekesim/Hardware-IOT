---
ID: 215
post_title: >
  Advances In High-Performance Cooling For
  Electronics
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/215
published: true
post_date: 2016-03-02 12:57:43
---
<h3>Introduction</h3>
The need for new cooling techniques is driven by the continuing increases in power dissipation of electronic parts and systems. In many instances standard techniques cannot achieve the required cooling performance due to physical limitations in heat transfer capabilities. These limitations are principally related to the limited thermal conductivity of air for convection and copper for conduction.

Figure 1 shows a comparison of various cooling techniques as a function of the attainable heat transfer in terms of the heat transfer coefficient. To accommodate a heat flux of 100 W/cm at a temperature difference of 50 K requires an effective heat transfer coefficient (including a possible area enlarging factor) of 20,000 W/mK. From Figure 1 it can be concluded that there will be a need for liquid cooling in the future of thermal management. This article briefly discusses a number of promising thermal management technologies that are emerging for possible electronics applications.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-217" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure01.jpg" width="500" height="230" alt="" /></td>
</tr>
</tbody>
</table>
Figure 1. Heat transfer coefficient attainable with natural convection, single-phase liquid forced convection and boiling for different coolants [1].
<h3>Conduction and Heat Spreading</h3>
In all cooling applications, heat from the device heat sources, must first travel via thermal conduction to the surfaces exposed to the cooling fluid before it can be rejected to the coolant. For example, as shown in Figure 2, heat must be conducted from the chip to the lid to the heat sink before it can be rejected to the flowing air. As can be seen thermal interface materials (TIMs) may be used to facilitate thermal conduction from the chip to the lid and from the lid to the heat sink. In many cases heat spreaders in the form of a flat plate with good thermal conductivity may be placed between the chip and lid to facilitate spreading of the heat from the chip to the lid or heat sink. Vapor chambers are also used to spread heat from a concentrated chip or module heat source to a larger heat sink.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-218" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure02.jpg" width="400" height="219" alt="" /></td>
</tr>
</tbody>
</table>
Figure 2. Chip package with thermal conduction path to heat sink via TIMs.For high-power applications, the interface thermal resistance becomes an important issue. Direct soldering (e.g., reflow soldering) is often difficult, certainly when copper is used because of the large CTE mismatch between Cu and Si. However, a few promising materials are entering the market. Diamond-filled greases have been tested to have an effective thermal conductivity of over 20 W/mK; however, the vendor claimed 60 W/mK [2]. Even more interesting is a nanostructured foil, which utilizes a very fast exothermic reaction to create a soldered connection virtually at room temperature [3]. Extensive long-term reliability studies are in progress [4].

Heat spreading is a very effective way of mitigating the need for sophisticated high-heat flux cooling options. Of course, to be effective the benefits of decreasing the heat flux density by increasing the area should outweigh the penalty of adding another layer that the heat must be conducted across. This is an optimization problem as discussed below. The options for advanced heat spreading solutions are two-fold:
<ul class="custom_dot list-paddingleft-1">
	<li class="list-dot list-dot-paddingleft">Novel materials such as carbonaceous materials, metal-matrix composites, ceramic matrix composites (e.g., diamond-particle-reinforced silicon carbide), or ScD (Skeleton cemented Diamond), all of them with much higher thermal conductivities than copper, much less weight and tunable CTEs [5].</li>
	<li class="list-dot list-dot-paddingleft">Novel heat spreader technologies such as Novel Concept’s Isoskin [6] and Enerdyne’s Polara [55] that claim effective thermal conductivities that compete with diamond.</li>
</ul>
By applying heat spreaders cooling methods such as loop heat pipes and low-flow liquid cooling may be augmented to accommodate higher heat flux applications. Figure 3 provides a graph showing heat spreading results for a 300 W heat source of 2 cm area as a function of thermal conductivity, thickness and cooling boundary condition (i.e., heat transfer coefficient). Looking at the results it becomes obvious that heat spreading is a complex phenomenon. This is because the conduction and convection effects cannot be separated and the two effects compete: increasing the thickness increases the through-plane resistance but decreases the in-plane thermal resistance. For example, comparing the two upper curves with the two lower curves, their order is changed. The results also show that it is very well possible to use heat spreaders to decrease the required fluid-side heat transfer coefficient to easily manageable values, below 5000 W/mK, which could be fairly easily realized with hydrofluoroether (HFE) cooling fluids. For example, using an 8 x 8 cm heat spreader of some advanced composite with a k of 800 W/mK and a thickness of 4 mm results in a temperature rise of 40°C with a heat transfer coefficient of only 2500 W/mK.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-219" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure03.jpg" width="500" height="284" alt="" /></td>
</tr>
</tbody>
</table>
Figure 3. Example of effect of thickness on heat spreading for various heat source areas, material thermal conductivities, and heat transfer coefficients (A in cm, K in w/mK, h in W/mK).
<h3>Air Cooling</h3>
It is generally acknowledged that traditional air-cooling techniques are about to reach their limit for cooling of high-power applications. With standard fans a maximum heat transfer coefficient of maybe 150 W/mK can be reached with acceptable noise levels, which is about 1 W/cm for a 60°C temperature difference. Using ‘macrojet’ impingement, theoretically we may reach 900 W/mK, but with unacceptable noise levels. Non-standard fans/dedicated heat sink combinations for CPU cooling are expected to have a maximum of about 50 W/cm, which is a factor of 10 higher than expected 15 years ago. However, some new initiatives have emerged to extend the useful range of air-cooling such as piezo fans, ‘synthetic’ jet cooling and ‘nanolightning’.
<h3>Piezo Fans</h3>
Piezoelectric fans are low power, small, relatively low noise, solid-state devices that recently emerged as viable thermal management solutions for a variety of portable electronics applications including laptop computers and cellular phones. Piezoelectric fans utilize piezoceramic patches bonded onto thin, low frequency flexible blades to drive the fan at its resonance frequency. The resonating low frequency blade creates a streaming airflow directed at electronics components. A group at Purdue reports up to a 100% enhancement over natural convection heat transfer [7].
<h3>‘Synthetic’ Jet Cooling</h3>
An approach using periodic microjets coined ‘synthetic jets’ has initially been studied by Georgia Institute of Technology and is being commercialized by Innovative Fluidics. Due to the pulsating nature of the flow, synthetic jets introduce a stronger entrainment than conventional-steady jets of the same Reynolds number and more vigorous mixing between the wall boundary layers and the rest of the flow. One of the test set-ups is shown in Figure 4. A synthetic jet entrains cool air from ambient, impinges on the top hot surface and circulates the heated air back to the ambient through the edges of the plate. A radial counter current flow is created in the gap between the plates with hot air dispersed along the top and ambient air entrained along the bottom surface. The idea was further explored by the development of flow actuators using MEMS technology [8].
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-220" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure04.jpg" width="400" height="663" alt="" /></td>
</tr>
</tbody>
</table>
Figure 4. Flow dynamics of normal jet impingement with an oscillating diaphragm.
<h3>‘Nanolightning’</h3>
An interesting new approach to increasing the heat transfer coefficient called ‘nanolightning’ is being pursued by researchers from Purdue . It is based on ‘micro-scale ion-driven airflow’ using very high electric fields created by nanotubes. As shown in Figure 5, the ionized air molecules are moved by another electric field, thereby inducing secondary airflow [9]. Cooling a heat flux level of 40 W/cm has been reported. The technology is being commercialized through a start-up company (Thorrn).
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-221" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure05.jpg" width="400" height="311" alt="" /></td>
</tr>
</tbody>
</table>
Figure 5. ‘Nanolightning’ sketch.
<h3>Liquid Cooling</h3>
The widely known heat transfer guru John Lienhard [10] once raised the question: “How much heat could possibly be carried away by boiling?” The answer is: 2000 kW/cm (based on water molecules turning into vapor without influencing each other). The highest reported experimental value is over 200 kW/cm, using high velocities and high pressures. Some commercially available microcoolers can handle about 1 kW/cm so there is some room for improvement. Liquid cooling for application to electronics is generally divided into the two main categories of indirect and direct liquid cooling. Indirect liquid cooling is one in which the liquid does not directly contact the components to be cooled. Direct liquid cooling brings the liquid coolant into direct contact with the components to be cooled. The following sections discuss the categories of indirect liquid cooling in the form of heat pipes and cold plates and direct liquid cooling in the form of immersion cooling and jet impingement.
<h3>Heat Pipes</h3>
Heat pipes provide an indirect and passive means of applying liquid cooling. They are sealed and vacuum pumped vessels that are partially filled with a liquid. The internal walls of the pipes are lined with a porous medium (the wick) that acts as a passive capillary pump. When heat is applied to one side of the pipe the liquid starts evaporating. A pressure gradient exists causing the vapor to flow to the cooler regions. The vapor condenses at the cooler regions and is transported back by the wick structure, thereby closing the loop. Heat pipes provide an enhanced means of transporting heat (e.g., under many circumstances much better than copper) from a source to a heat sink where it can be rejected to the cooling medium by natural or forced convection. The effective thermal conductivity of a heat pipe can range from 50,000 to 200,000 W/mK [11], but is often much lower in practice due to additional interface resistances. The performance of heat pipes scales from 10 W/cm to over 300 W/cm. A simple water-copper heat pipe will on average have a heat transfer capacity of 100 W/cm. An example of a typical application of a heat pipe for an electronics cooling application is given in Figure 6.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-222" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure06.jpg" width="400" height="286" alt="" /></td>
</tr>
</tbody>
</table>
Figure 6. Examples of heat pipes used in a notebook application.Although there is virtually no limit to the size of a heat pipe, the effectiveness of a heat pipe decreases with decreasing lengths. For heat pipes with a length less than about 1 cm the performance of a solid piece of metal (e.g., copper) is often comparable. They are very effective as efficient heat conductors to transport heat to locations were more area is available. 2D heat spreaders (otherwise known as vapor chambers) based on the heat pipe principle can achieve much higher effective thermal conductivities than copper. For example, a thin planar heat spreader has been developed that is claimed to have a thermal performance greater than diamond [12].

Besides standard heat pipes, loop heat pipes (LHP) such as those shown in Figure 7 are attracting increased attention. LHPs have the advantage over conventional heat pipes that the vapor and liquid paths are separated enabling much better performance of the liquid return loop. For example, Kim et al. [12] showed the ability to accommodate a heat flux of 625 W/cm.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-223" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure07.jpg" width="400" height="276" alt="" /></td>
</tr>
</tbody>
</table>
Figure 7. Examples of loop heat pipes.
<h3>Cold Plates</h3>
Liquid-cooled cold plates perform a function analogous to air-cooled heat sinks by providing an effective means to transfer heat from a component to a liquid coolant. Unlike heat pipes they may be considered active devices in that liquid is usually forced through them by the action of a pump. For many years water-cooled cold plates were used in mainframe computers to cool high-powered multi-chip processor modules. Vacuum-brazed finstock coldplates are standard practice in defense electronics, and copper-based superalloy structures are used in high-energy lasers. In 1981, in an effort to significantly extend cooling capability, Tuckerman and Pease [13] demonstrated a liquid -cooled microchannel heat sink that removed 790 W/cm with a temperature increase of 71°C for a 600 ml/min flow rate with a pressure drop of 207 kPa. As a result of the continuing increases in heat flux at the chip level, microchannel cold plates are receiving renewed attention.
<h3>Microchannels and Minichannels</h3>
The term ‘micro’ is applied to devices having hydraulic diameters of ten to several hundred micrometers, while ‘mini’ refers to diameters on the order of one to a few millimeters. In many practical cases, the small flow rate within micro-channels produces laminar flow resulting in a heat transfer coefficient inversely proportional to the hydraulic diameter. In other words, the smaller the channel, the higher the heat transfer coefficient. Unfortunately, the pressure drop increases with the inverse of the second power of the channel width, keeping the mass flow constant, and limiting ongoing miniaturization in practice.

Garimella and Sobhan [14] published a very good review of the microchannel literature up to 2000. They concluded, among others, that “Given the diversity in the results in the literature, a reliable prediction of the heat transfer rates and pressure drops in microchannels is not currently possible for design applications such as microchannel heat sinks.” Mudawar [15] reviewed high-heat-flux thermal management schemes, including ultra-high-heat-fluxes in the range of 1000-100,000 W/cm. A recent overview was also provided by Mohapatra and Loikitis [16].

Lee and Vafai [17] compared jet impingement and microchannel cooling for high heat flux applications. One of their conclusions is that microchannel cooling is more effective for areas smaller than 7 x 7 cm. Integrated single and two-phase micro heat sinks are treated by Gillot et al. [18]. They were able to cool about 450 W/cm using both single and two-phase heat transfer. For two-phase flow the pumping power is about ten times lower and the required flow rate is considerably lower. Kandlikar and Upadhye [19] showed enhanced microchannel cooling by using off-set strip fins and a split-flow arrangement. Cooling of over 300 W/cm at 24 kPa is claimed with a flow of 1.5 l/min. A paper devoted to pumping requirements has been written by Singhal et al. [20]. Useful graphs compare the performance of a whole range of pumps that could be considered for microchannel cooling. Colgan et al. [21] at IBM published a practical implementation of a silicon microchannel cooler (as shown in Figure 8) for high-power chips. They argued that it is not practical to form the microchannels directly on the chip given the high cost of high-performance processor chips. Instead, a separate microchannel cold plate is bonded to the back of the chip. This requires a very low interface thermal resistance. If the microcooler is based on silicon, a rigid bonding means that silver-filled epoxies or solder should be used. Power densities in excess of 400 W/cm are reported, for a flow of 1.2 l/min at 30 kPa.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-224" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure08.jpg" width="500" height="166" alt="" /></td>
</tr>
</tbody>
</table>
Figure 8. Pictures from IBM paper showing high-performance liquid cooling technology using microchannels [21].It may be possible to push microchannel heat transfer even further by utilizing boiling. In addition to offering higher heat transfer coefficients, boiling convection in microchannels is promising because it requires less pumping power than single-phase liquid convection to achieve a given heat sink thermal resistance. For the same heat flux the pressure drops by a factor of 20. A review has been published by Bergles et al. [22]. A prototype of a 1000 W/cm cooling system based on boiling heat transfer in microchannel heat sinks using a flow rate of 500 ml/min has been described in [23]. The main practical problem with two-phase flow is its unpredictability. Local heat transfer coefficients may change appreciably over time leading to local temperature changes of 10-15 °C [24]. Also backflow of already heated flow due to expansion of bubbles is observed.

Increasingly, microchannel-like cold plates are becoming commercially available. Mikros [25] claims 1000 W/cmK, 14-21 kPa and 0.05 K/W/cm for its patented technology in which the fluid impinges on the surface to be cooled. ACT (Advanced Cooling Technologies) [26] offers pumped liquid (both single and two-phase) cooling technologies in addition to loop heat pipes for space applications. Their single-phase solution (see Figure 9) incorporates a ‘unique oscillating flow heat transfer’ mechanism, capable of cooling over 1300 W/cm.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-225" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure09.jpg" width="500" height="685" alt="" /></td>
</tr>
</tbody>
</table>
Figure 9. Vendor’s heat spreader and test results.Another company, Cirrus, sells microchannel high heat flux heat sinks, claiming over 100 W/cm heat flux capability and reduced pressure drops. Recently another player, iCurie [27], entered the market. They claim a pumpless microchannel cooling system based on capillary pumping with separate liquid-vapor loops. The layout can be very flexible, only 300 micrometer thick. At least 200 W/cm can be cooled, with the additional advantage of a negligible effect of gravity. It is not a heat pipe because the principle of operation is based on flow boiling, not evaporation. Other companies offering microchannel coolers include Lytron, Novel Concepts, Curamik, Microcooling Concepts (MC), and Koolance.

A completely different way of making microchannels is by using metal foams or metal made porous otherwise. Engineers from Thermacore have described a family of liquid -cooled heat sinks using porous metal. They accommodated a heat flux of 500 W/cm for a 50 K difference at a pressure drop of 115 kPa using water [28].

On June 21, 2005, Georgia Tech [29] announced a novel monolithic technique for fabricating liquid cooling channels onto the backs of high-performance ICs. They also built a system that would allow the on-chip cooling system to be connected to embedded fluidic channels built into a printed circuit board.
<h3>Electrohydrodynamic and Electrowetting Cooling</h3>
As an alternative to a continuous flow set into motion by either temperature differences or by mechanical means, liquid could also be formed and moved in droplets of nano-to-milliliter size (see for example a nice demonstration by Nanolytics [30]) by means of electric fields. Electrowetting on a dielectric film, in which the surface property of a dielectric film can be modified between hydrophobic and hydrophilic states using an electric field, can be used to provide the basis for a direct micropumping system. Electrowetting involves control of the surface tension of a liquid and can cause a droplet of liquid to bead (as shown in Figure 10) or spread out on the surface depending upon its surface state.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-226" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure10.jpg" width="500" height="169" alt="" /></td>
</tr>
</tbody>
</table>
Figure 10. Water forms a nearly perfect ball, as shown in left photo, suspended on the tips of tiny blades of nanograss.One of the possible applications is cooling on a micro scale. The recently published theoretical work of Pamula [31] has shown a possible configuration based on fast moving droplets under a chip. They showed that with 0.4 ml/min it is theoretically possible to cool 90 W/cm. Recently Leuven University in collaboration with Philips Research published two papers on this subject [32, 33]. The Philips approach differs from the Duke approach in that it concerns an oscillating flow. At Bell Labs researchers coupled electrowetting with nanostructured superhydrophobic surfaces (coined ‘nanograss’) to result in dynamically tunable surfaces [34]. One application is the movement of droplets to cool hot spots; however, no further heat transfer data are given.

A recent publication discussed another promising development, the application of electrowetting to liquid metals [35]. The main advantage besides a better heat transfer capability is the much lower voltage required (2 instead of 50 V). However, no experimental data have been presented.

The interesting aspect in combining microfluidics with electric control is that when all sizes scale down to micro scale, the electro/-kinetic/-wetting/-osmotic forces become comparable to pressure drop forces and therefore control of the liquid motion becomes easier. Of course, active cooling of a hot surface is one thing, to remove heat from the heated liquid in a closed loop requires additional heat exchange area.
<h3>Liquid Metal Cooling</h3>
Of special interest is the work ongoing in the field of liquid metal cooling. Apart from heat pipes based on liquid metals, mainly for the high-temperature range, an increasing amount of research is devoted to the use of Ga-Sn-In eutectics that remain liquid down to minus 19°C. In [36, 37] high-performance liquid metal cooling loops are described using magnetofluiddynamic pumps, claiming over 200 W/cm cooling capacity, using a flow of 0.3 l/min at 15 kPa. Examples of liquid cooling loops for electronics cooling application are shown in Figures 11 and 12. Another advantage of liquid metal is its much lower CTE compared to water and the fact that freezing introduces fewer problems. Developments to extend the use in cold environments to -40°C are ongoing.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-227" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure11.jpg" width="500" height="252" alt="" /></td>
</tr>
</tbody>
</table>
Figure 11. Sketch of liquid metal cooling loop.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-228" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure12.jpg" width="400" height="302" alt="" /></td>
</tr>
</tbody>
</table>
Figure 12. Typical configuration of liquid metal cooling loop for mobile applications.
<h3>Immersion Cooling</h3>
Direct liquid or immersion cooling is a well-established method for accommodating high heat flux backed by over thirty years of university and industrial research. With natural convection two-phase flow, generally termed nucleate pool boiling, the critical heat flux using FC-72 is in the range of 5 to 20 W/cm. However, much higher heat fluxes up to 100 W/cm can be accommodated with surface enhancement of the heat source. Figure 13 illustrates a device submerged in a pool of dielectric liquid. The heat dissipated in the device produces vapor bubbles that are driven by buoyancy forces into the upper region of the container, where the vapor condenses and drips back into the liquid pool. One of the disadvantages of this technique is the need for a liquid compatible with the device. Most often, water cannot be used because of its chemical and electrical characteristics.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-229" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure13.jpg" width="400" height="270" alt="" /></td>
</tr>
</tbody>
</table>
Figure 13. Example of pool boiling (thermosyphon) cooling.
<h3>Liquid Jet Impingement</h3>
Wang et al. [38] claim a cooling of 90 W/cm with a 100°C temperature rise using a flow rate of only 8 ml/min. Researchers at Georgia Institute of Technology studied a closed loop impingement jet [39]. Cooling of almost 180 W/cm has been realized using water, using a flow of 0.3 l/min at 300 kPa. The micropump used 7 W to drive it.

At this point it is difficult to say which one is better, microchannels or microjets. Microchannels are easier to fabricate and implement but the temperature nonuniformity is larger and the nucleation is more difficult to control. Microjets achieve better cooling uniformity but more fabrication steps are required and an initial pressure is necessary to form the jet. An example of a commercial concept for liquid cooling is shown in Figure 14 [40].
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-230" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure14.jpg" width="400" height="312" alt="" /></td>
</tr>
</tbody>
</table>
Figure 14. Commercially available multiple jet impingement liquid cooling.
<h3>Spray Cooling</h3>
In recent years spray cooling has received increasing attention as a means of supporting higher heat flux in electronic cooling applications. Spray cooling breaks up the liquid into fine droplets that impinge individually on the heated wall. Cooling of the surface is achieved through a combination of thermal conduction through the liquid in contact with the surface and evaporation at the liquid-vapor interface. The droplet impingement both enhances the spatial uniformity of heat removal and delays the liquid separation on the wall during vigorous boiling.

Spray evaporative cooling with a Fluorinert™ coolant is used to maintain junction temperatures of ASICs on MCMs in the CRAY SV2 system between 70 and 85°C for heat fluxes from 15 to 55 W/cm [41]. In addition to the CRAY cooling application, spray cooling has gained a foothold in the military sector providing for improved thermal management, dense system packaging, and reduced weight [42]. A research group at UCLA discussed chip-level spray cooling for an RF power amplifier and measured a maximum heat flux of over 160 W/cm [43]. Isothermal Systems Research manufactures SprayCool products [44].

Spray cooling and jet impingement (as shown in Figure 15) are often considered competing options for electronic cooling. In general, sprays reduce flow rate requirements but require a higher nozzle pressure drop.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-231" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure15.jpg" width="372" height="432" alt="" /></td>
</tr>
</tbody>
</table>
Figure 15. Illustration of spray and jet impingement cooling.A final method to be mentioned is inkjet-assisted spray cooling. This method uses existing thermal inkjet technology. A critical heat flux of 270 W/cm is reported [45] using only 3ml/min, with a COP of 6, meaning that the inkjet pumping power is a factor of 6 lower than the heat removed.
<h3>Solid-State Cooling</h3>
A thermoelectric or a Peltier cooler (as shown in Figure 16) is a small electronic heat pump that has the advantage of no moving parts and silent operation. Thermoelectric cooling enables cooling below ambient temperature. The coolers operate on direct current and may be used for heating or cooling by reversing the direction of current flow.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-232" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure16.jpg" width="400" height="261" alt="" /></td>
</tr>
</tbody>
</table>
Figure 16. Schematic of simple Peltier cooler.When a positive DC voltage is applied to the n-type thermoelement, electrons pass from the p- to the n- type thermoelement and the cold side temperature decreases as heat is absorbed.

The heat absorption (cooling) is proportional to the current and the number of thermoelectric couples. The main disadvantage is that the heat transferred to the hot side is greater than the amount of heat pumped by a quantity equal to the Joule heating (i.e., IR loss) that takes place in the Peltier elements.

The three most important thermoelectric effects are the Seebeck, Peltier and Thomson effects. For thermoelectric cooling the Thomson effect can be neglected. The Peltier coefficient Π and Seebeck coefficient S are related to each other through Π = S�T. Thermoelectric materials are usually characterized by their figure of merit ZT, defined by:
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-233" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Eq_p34.jpg" width="245" height="45" alt="" /></td>
</tr>
</tbody>
</table>
whereσ= electrical conductivity
λ = thermal conductivity
T = temperature in absolute units

This equation shows why it is difficult to obtain good thermoelectric materials. A good thermoelectric material must achieve low thermal conductivity (to prevent heat losses through heat conduction between the hot and cold side) and a high electrical conductivity (to minimize Joule heating). Due to the dependence of σ and λ (Wiedemann-Franz law), it is almost impossible to optimize this ratio for theelectron contribution to the thermal conductivity. Hence, the approach is to reduce the phonon thermal conductivity without a degradation of the electrical conductivity. The best materials so far are alloys of Bi2Te3 with Sb2Te3 and Bi2Te3 with Bi2Se3. ZT is of the order of 1 at room temperature. This value gives a Coefficient of Performance (COP, a measure for the efficiency) of about 1 (see Figure 17a), which compared to household refrigerators and air conditioners (COP from 2 to 4), makes thermoelectric cooling generally not competitive. The same holds for power generation (see Figure 17b).
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-234" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure17.jpg" width="400" height="631" alt="" /></td>
</tr>
</tbody>
</table>
Figure 17. Comparison of thermoelectric technology with other energy conversion methods for (a) cooling and (b) power generation [46].Despite the low efficiency, the application areas are increasing and include infrared detector cooling, charge coupled devices (CCDs), microprocessors, blood analyzers, portable picnic coolers. Principal applications are still accurate control of temperature and cooling below ambient temperature.

One of the problems with traditional Peltier elements is their limited capability of cooling heat fluxes over 5-10 W/cm. Because the cooling density of a Peltier cooler is inversely proportional to its length, scaling to smaller size is desirable. The material structure produced by conventional crystal growth techniques for producing bismuth telluride thermoelectric materials impose significant limitations on thermoelectric element dimensions due to poor manufacturing yields. This prevents thermoelectric elements from being made very short. Marlow Industries reported new fine-grain micro-alloyed bismuth telluride materials that do not suffer the element geometry limitation and can offer higher performance [47]. Another serious step forward has been realized by Nanocoolers through a proprietary wafer-scale manufacturing process. It concerns a monolithic process with thicknesses about 1-2 micrometers (see Figure 18). They claim a tunable performance of 10 – 1000 W/cm with a single stage Δ T of 50-70 K [48]. MicroPelt, a spin-off company from Fraunhofer and Infineon also sells promising thin film thermoelectrics (see Figure 19). For their near-future products they claim cooling of 160 W/cm.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-235" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure18.jpg" width="400" height="230" alt="" /></td>
</tr>
</tbody>
</table>
Figure 18. Comparison of standard and thin-film Peltier element.

<img class="alignnone size-full wp-image-236" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure19.jpg" width="400" height="290" alt="" />
Figure 19. Thin film Peltier element.A number of other research projects directed at miniaturizing Peltier elements are worth mentioning. In 2004 Biophan Technologies [49] signed an agreement with NASA for characterization and joint development of high-density nanoengineered thermoelectric materials for use with implantable devices. They anticipate a breakthrough in power generation systems. A French/US consortium published a paper [50] on the fabrication and modeling of an in-plane thermoelectric micro-generator. They concluded that a heating power of about 100 mW may be enough to produce 1 mW of useful electrical power in vacuum, using thin film technology. A compact thermoelectric device may be able to produce 60 microwatt with an output voltage of 1.5 V in air. Applied Digital Solutions uses its ThermoLife thermoelectric power generator to power its implantable chips [51]. It generates 3V, has a diameter of 9.3 mm and weighs 230 mg. DTS in Germany uses thin film technology for their Low Power Thermoelectric Generators (LPTGs) [52] that produce a few tens of microwatts in the volt range for a temperature difference of a few degrees C. The generators have a mass of 390 mg. Also in Germany, researchers at Dresden University [53] have found a way to make tiny thermoelectric generators using copper foil as a template. Antimony-Bismuth thermocouples are electro-deposited and after adding an epoxy film the copper is etched away. The result is a cheap, flexible and recycable generator that converts environmental heat into electricity. The growth by pulsed laser deposition of high-quality thermoelectric cobaltate thin films on silicon has been reported by Yu et al. [54]. In addition, TEM characterization revealed nearly perfect crystalline structures of the Ca3Co4O9 film formed on top of an SiOx amorphous layer, suggesting self-assembly might be a viable technique for cobalt oxide-based thermoelectrics.

If the application is limited to temperatures above ambient temperature matters are quite different. Because the heat flow paths of the cooling and the conduction have the same direction, high-thermal conductivity materials are preferred. Enerdyne’s Polara heat spreaders are based on this principle [55]. A factor of five improvement compared to copper is claimed as shown in Figure 20. However, no samples are available as of July 2005.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-237" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure20.jpg" width="400" height="264" alt="" /></td>
</tr>
</tbody>
</table>
Figure 20. Comparison of effective thermal conductances.
<h3>Superlattice and Heterostructure Cooling</h3>
For a number of years now, the strategy to improve thermoelectric cooling has taken a new turn [46] giving hope for the future. On a nano scale level, coherent and incoherent transport plays an important role in the electron and phonon diffusion. Extensive research is going on in this field. For example, Venkatasubramanian [56] at RTI reported ZT values between 2-3 at room temperature obtained with Bi2Te3/Se2Te3 superlattices. Cooling power density is estimated as high as 700 W/cm at 353 K compared to 1.9 W/cm in the bulk material (see Figures 21 and 22).
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-238" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure21.jpg" width="400" height="292" alt="" /></td>
</tr>
</tbody>
</table>
Figure 21. Estimated power density for superlattice devices as a function of current.
<table width="700px">
<tbody>
<tr>
<td align="center" width="680"><img class="alignnone size-full wp-image-239" src="http://www.mekesim.com/wp-content/uploads/2016/03/2005_November_Article2_Figure22.jpg" width="400" height="252" alt="" /></td>
</tr>
</tbody>
</table>
Figure 22. Potential COP as a function of ZT with various technologies. THOT refers to the heat sink temperature.Thin-film related work is also being conducted at the University of California Santa Cruz, based on SiGe/Si. The most recent paper [57] quotes a cooling power density of nearly 600 W/cm for a temperature difference of 4K below ambient for a 40 x 40 micrometer size area. The superlattice efforts of RTI are being commercialized through a spin-off company called Nextreme. Recent information reveals that despite their claimed value of ZT = 2.4, they are not able to manufacture production samples with a ZT larger than 1.4. The focus is to reduce the parasitics and to reduce even further the current 100 micrometer thickness.

However, there is still hope for a serious breakthrough. Very recently, Humphrey and Linke [58] published a paper called ‘Reversible Thermoelectric Materials’. They argue that nanostructured materials with sharply peaked electronic density of states (such as quantum wires) may operate reversibly, challenging the view that thermoelectric devices are inherently irreversible heat engines. In this case, ZT values could reach a value of 10 at room temperature, much above the value of 5 that is required for economical adoption of thermoelectric technology for mainstream refrigeration and power generation.
<h3>Thermionic and Thermotunneling Cooling</h3>
Thermionic cooling is based on the principle that a high-work-function cathode preferentially emits hot electrons [46]. Materials available have a work function of 0.7 eV or higher, which limits the use to the higher temperature ranges (&gt;500 K). Vacuum thermionic devices based on resonant tunnelling have been proposed more recently [59]. Cooling capabilities of 20-30°C with kW/cm cooling power density can be achieved. However, since the operating currents for the device are as high as 10A/cm, effects such as Joule heating at the metal-semiconductor contact resistance and reverse heat conduction have limited the experimental cooling results to &lt;1°C.

Devices based on quantum tunnelling through a small gap are being commercialized [60]. The spacing between the cathode and the anode should be of the order of 10 nm providing quite an engineering challenge. Much larger cooling power than thermoelectric superlattice coolers are predicted by Hishinuma et al. [61] (e.g.10 kW/cm for 50 K cooling at room temperature). Recently a study has been devoted to their potential use as energy scavenging or power conversion devices [62]. Unfortunately, the conclusion is that a gap an order of magnitude lower must be achieved to be of interest for these application fields. Even more worrying is another recent study [63] showing that contrary to the results of Hishinuma only about 16 W/cm can be reached with a Δ T of 40°C, while the maximum COP is only 0.25. More or less the same conclusion can be drawn from a paper presented at THERMINIC 2005, September 27-30 [64]. Herein, some weaknesses in prior studies are discussed and it is clear from the conclusions that nanogap solutions without significant improvements in lower work function materials have no future.
<h3>Phase Change Materials and Heat Accumulators</h3>
Phase change materials are successfully used as heat-storing materials for air conditioning, cool boxes, efficient fire-retarding powders, as functional materials for self-heating insoles for boots and many other industrial applications. Their use for electronics thermal management is limited to applications where time-dependent phenomena play a role. For example, reference [65] discusses the use of phase change materials as compared to copper for use in a power semiconductor unit.

Chemical heat accumulators should also be mentioned. For example, the use of composite materials based on granulated open-porous matrix filled with a hygroscopic substance can be seen as a new approach to accumulate heat [66]. The advantage is a significant increase in the heat that can be stored as compared to sensible heat and latent heat. For example, for a 100°C temperature rise copper absorbs 40 kJ/kg. Evaporation of water is associated with an absorption of 2260 kJ/kg. The enthalpy of a reversible chemical reaction can reach a value of 7000 kJ/kg. A principal advantage of reversible chemical reactions for heat accumulation is their ability to store the accumulated energy for a long time, if the reaction is controlled by the presence of either a catalyst or a reagent. Hence, the major applications are in the field of summer-winter heat storage for buildings, etc. Chemical heat accumulators could potentially be used for outdoor electronic applications when a night-day rhythm is present.
<h3>Conclusions</h3>
A number of approaches show interesting industrial potential for the cooling of high-power electronics. This prospect is attested to by the number of small companies that are entering the market. For example, there are now companies engaged in the development and commercialization of microchannels, spray cooling, synthetic jets, thin film Peltier elements. For heat flux densities up to and maybe even beyond 50 W/cm air-cooling may remain the cooling option of choice. For heat fluxes over 100 W/cm, some form of liquid-cooling appears to be the most viable option. Several papers have demonstrated solutions that may be industrially feasible for application in the range between 500 and 1000 W/cm. Considering the range of efforts underway to extend conventional cooling technologies, as well as develop new ones, the future seems bright for accommodating high-heat flux applications.

(Note: We deemed it instructive to include examples of commercially-available thermal solutions. However, it should be clearly stated that we do not intend to promote any of the mentioned products. Finally, we have tried to cover the state-of-the-art as known to us. However, given the broadness of the field, we may have overlooked some important new developments for which we apologize.)
<h3>References</h3>
<ol class="custom_num list-paddingleft-1">
	<li class="list-num-1-1 list-num-paddingleft-1">Lasance, C., Technical Data column, ElectronicsCooling, January 1997.</li>
	<li class="list-num-1-2 list-num-paddingleft-1">Rogers, P., CALCE, personal communication, April 2005.</li>
	<li class="list-num-1-3 list-num-paddingleft-1"><a href="http://www.reactivenanotechnologies.com/">http://www.reactivenanotechnologies.com/</a>.</li>
	<li class="list-num-1-4 list-num-paddingleft-1">Subramanian, J., et al. “Room Temperature Soldering of Microelectronic Components for Enhanced Thermal Performance,” EuroSimE 2005, pp. 681-686, 2005.</li>
	<li class="list-num-1-5 list-num-paddingleft-1">Zweben, C., “Ultra-High Thermal Conductivity,” Proceedings of 21st SemiTherm Symposium, San Jose, CA, pp. 168-174, 2005.</li>
	<li class="list-num-1-6 list-num-paddingleft-1"><a href="http://novelconceptsinc.com/index.htm">http://novelconceptsinc.com/index.htm</a></li>
	<li class="list-num-1-7 list-num-paddingleft-1">Acikalin, T., Wait, S., Garimella, S., Raman, A., “Experimental Investigation of the Thermal Performance of Piezoelectric Fans,” HeatTransfer Eng., Vol. 25, pp. 4-14, 2004.</li>
	<li class="list-num-1-8 list-num-paddingleft-1">Beratlis, N., and Smith, M., “Optimization of Synthetic Jet Cooling for Micro-electronics Applications,” Proceedings of 19th SemiTherm Symposium, San Jose, CA, pp. 66-73, 2003.</li>
	<li class="list-num-1-9 list-num-paddingleft-1">Peterson, M., Fisher, T., Garimella, S., and Schlitz, D., “Experimental Characterization of Low Voltage Field Emission from Carbon-Based Cathodes in Atmospheric Air,” Proceedings of IMECE’03, Paper #41775, 2003.</li>
	<li class="list-num-1-10 list-num-paddingleft-1">Lienhard, J., “High Heat Flux in Japan,” Egines of Our Ingenuity, No. 448,<a href="http://www.uh.edu/engines/epi448.htm">http://www.uh.edu/engines/epi448.htm</a>.</li>
	<li class="list-num-1-11 list-num-paddingleft-1">Thyrum, G., “Critical Aspects of Modeling Heat Pipe Assisted Heat Sinks,”<a href="http://www.thermacore.com/pdfs/critical.pdf">http://www.thermacore.com/pdfs/critical.pdf</a>.</li>
	<li class="list-num-1-12 list-num-paddingleft-1">Kim, J., and Golliher, E., “Steady State Model of a Micro Loop Heat Pipe,” Proceedings of 18th SemiTherm Symposium, San Jose, CA, pp. 137-144, 2002.</li>
	<li class="list-num-1-13 list-num-paddingleft-1">Tuckerman, D.B., and Pease, R.F., “High Performance Heat Sinking for VLSI,” IEEE Electron Device Letters, EDL-2, 5, pp. 126-129, 1981.</li>
	<li class="list-num-1-14 list-num-paddingleft-1">Garimella, S., and Sobhan, C., “Transport in Microchannels – A Critical Review,” Ann. Rev. Heat Transfer, Vol. 13, pp. 1-50, 2003.</li>
	<li class="list-num-1-15 list-num-paddingleft-1">Mudawar, I., “Assessment of High-Heat-Flux Thermal Management Schemes,” IEEE CPT Trans., Vol. 24, pp. 122-141, 2001.</li>
	<li class="list-num-1-16 list-num-paddingleft-1">Mohapatra, S., and Loikitis, D., “Advances in Liquid Coolant Technologies for Electronics Cooling,” Proceedings of 21st SemiTherm Symposium, San Jose, CA, pp. 354-360, 2005.</li>
	<li class="list-num-1-17 list-num-paddingleft-1">Lee, D.Y., and Vafai, K., “Comparative Analysis of Jet Impingement and Microchannel Cooling for High Heat Flux Applications,” Intl. Jour. of Heat and Mass Transfer, Vol. 42, pp. 1555-1568, 1999.</li>
	<li class="list-num-1-18 list-num-paddingleft-1">Gillot, C., Meysenc, Schaeffer, and Bricard, A., IEEE CPT, Vol. 22, No. 3, pp. 384-389, 1999.</li>
	<li class="list-num-1-19 list-num-paddingleft-1">Kandilikar, S., and Upadhye, H., “Extending the Heat Flux Limit With Enhanced Microchannels in Direct Single-Phase Cooling of Computer Chips,” Proceedings of 21st SemiTherm Symposium, San Jose, CA, pp. 8-15, 2005.</li>
	<li class="list-num-1-20 list-num-paddingleft-1">Singhal, V., et al., “Analysis of Pumping Requirements for Microchannel Cooling Systems,”IPACK’03, Paper # 35237, 2003.</li>
	<li class="list-num-1-21 list-num-paddingleft-1">Colgan, E., et al., “A Practical Implementation of Silicon Microchannel Coolers for High Power Chips,” Proceedings of 21st SemiTherm Symposium, San Jose, CA, pp. 1-7, 2005.</li>
	<li class="list-num-1-22 list-num-paddingleft-1">Bergles, A.E., et al., “Boiling and Evaporation in Small Diameter Channels,” Heat Transfer Engineering, Vol. 24, pp. 18-40, 2003.</li>
	<li class="list-num-1-23 list-num-paddingleft-1">Faulkner, D., Khotan, M., and Shekarriz, R., “Practical Design of 100 W/cm2 Cooling System,” Proceedings of 19th SemiTherm Symposium, San Jose, CA, pp. 223-230, 2003.</li>
	<li class="list-num-1-24 list-num-paddingleft-1">Vadakkan, U., Intel, personal communication, March 2005.<a href="http://www.mikrostechnologies.com/">
</a></li>
	<li class="list-num-1-25 list-num-paddingleft-1"><a href="http://www.mikrostechnologies.com/">http://www.mikrostechnologies.com</a>.</li>
	<li class="list-num-1-26 list-num-paddingleft-1"><a href="http://www.1-act.com/">http://www.1-act.com/</a>.</li>
	<li class="list-num-1-27 list-num-paddingleft-1">Lee, J., “A Macro Cooling Solution With Micro/Nano Technology,” Proceedings of Next-Generation Thermal Management Materials and Systems,” Phoenix, AZ, June 2005.</li>
	<li class="list-num-1-28 list-num-paddingleft-1">North, M., and Cho, W., “High Heat Flux Liquid-Cooled Porous Metal Heat Sink,” Proceedings of IPACK 2003, Maui, HI, Paper # 35320, 2003.</li>
	<li class="list-num-1-29 list-num-paddingleft-1"><a href="http://www.gtresearchnews.gatech.edu/newsrelease/cooling.htm">http://www.gtresearchnews.gatech.edu/newsrelease/cooling.htm</a>.</li>
	<li class="list-num-1-30 list-num-paddingleft-1"><a href="http://www.nanolytics.com/">http://www.nanolytics.com</a>.</li>
	<li class="list-num-1-31 list-num-paddingleft-1">Pamula, V.K., and Chakrabarty, K., “Cooling of Integrated Circuits Using Droplet-Based Microfluidics,” Proceedings ACM Great Lakes Symposium on VLSI, pp. 84-87, 2003.</li>
	<li class="list-num-1-32 list-num-paddingleft-1">Oprins, H., Vandevelde, B., Beyne, E., Borghs, G., and Baelmans, M., “Selective Cooling of Microelectronics Using Electrostatic Actuated Liquid Droplets-Modelling and Experiments, 10th THERMINIC, pp. 207-212, 2004.</li>
	<li class="list-num-1-33 list-num-paddingleft-1">Oprins, H., Nicole, C.C.S., Baret, J.C., Van der Verken, G., Lasance, C., and  Baelmans, M., “On-Chip Liquid Cooling With Integrated Pump Technology,” Proceedings of 21st SemiTherm Symposium, San Jose, CA, pp. 15-17, 2005.</li>
	<li class="list-num-1-34 list-num-paddingleft-1">Krupenkin, T. et al., “From Rolling Ball to Complete Wetting: the Dynamic Tuning of Liquids on Nanostructured Surfaces, Langmuir, 20, pp.3824-3827, 2004.</li>
	<li class="list-num-1-35 list-num-paddingleft-1">Mohseni, K., “Effective Cooling of Integrated Circuits Using Liquid Alloy Electrowetting,” Proceedings of 21st SemiTherm Symposium, San Jose, CA, pp. 20-25, 2005.</li>
	<li class="list-num-1-36 list-num-paddingleft-1">Miner, A., and Ghoshal, U., “Cooling of High-Power Density Microdevices Using Liquid Metal Coolants, Appl. Phys. Lett., Vol.85, 506-508, 2004.</li>
	<li class="list-num-1-37 list-num-paddingleft-1">Ghoshal, U., Grimm, D., Ibrani, S., Johnston, C., and Miner, A., “High-performance Liquid Metal Cooling Loops, Proceedings of 21st SemiTherm Symposium, San Jose, CA, pp. 16-19, 2005.</li>
	<li class="list-num-1-38 list-num-paddingleft-1">Wang, E., et al., Micromachined Jets for Liquid Impingement Cooling of VLSI Chips, J. Microelectromech. Syst., vol.13, pp.833-842, 2004.</li>
	<li class="list-num-1-39 list-num-paddingleft-1">Bintoro, J., et al., “A Closed Loop Impinging Jet Cooling for Computer Chip,” IMECE2003, Washington D.C., Paper # 43865, 2003.</li>
	<li class="list-num-1-40 list-num-paddingleft-1"><a href="http://siliconpower.danfoss.com/Products/PDF/Shower%20Power.pdf">http://siliconpower.danfoss.com/Products/PDF/Shower%20Power.pdf</a>.</li>
	<li class="list-num-1-41 list-num-paddingleft-1">Pautsch, G., and Bar-Cohen, A., “An Overview on the System Packaging of the Cray SV2 Supercomputer,” Ipack 2001 Conference, Kauai, HI, 2001.</li>
	<li class="list-num-1-42 list-num-paddingleft-1">Cader, T., and Tilton, D., “Implementing Spray Cooling Thermal Management in High Heat Flux Applications,” Proceedings of 2004 InterSociety Conference on Thermal Phenomena, pp. 699-701, 2004.</li>
	<li class="list-num-1-43 list-num-paddingleft-1">Cotler, A., et al., “”Chip-Level Spray Cooling of an LD-MOSFET RF Power Amplifier,” IEEE CPT Trans., Vol. 27, pp. 411-416, 2004.</li>
	<li class="list-num-1-44 list-num-paddingleft-1"><a href="http://www.spraycool.com/flash/index.html#home">http://www.spraycool.com/flash/index.html#home</a>.</li>
	<li class="list-num-1-45 list-num-paddingleft-1">Bash, C., et al., “Inkjet Assisted Spray Cooling of Electronics,” IPACK2003, Maui, HI, Paper# 35058, 2003.</li>
	<li class="list-num-1-46 list-num-paddingleft-1">Chen, G., and Shakouri, A., “Heat Transfer in Nanostructures for Solid-State Energy Conversion, J. of Heat Transfer, Vol. 124, p. 242, 2002.</li>
	<li class="list-num-1-47 list-num-paddingleft-1">Bierschenk, J., and Johnson, D.A., “Latest Developments in Thermoelectrically Enhanced Heat Sinks,” ElectronicsCooling, Vol. 11, No. 3, pp. 24-32, August 2005.</li>
	<li class="list-num-1-48 list-num-paddingleft-1">Ghoshal, U., “Advanced Thermoelectric Cooling Systems,” Proceedings of Next-Generation Thermal Management Materials and Systems,” Phoenix, AZ, June 2005.</li>
	<li class="list-num-1-49 list-num-paddingleft-1"><a href="http://www.biophan.com/pr/release_051404.html">http://www.biophan.com/pr/release_051404.html</a>.</li>
	<li class="list-num-1-50 list-num-paddingleft-1">Jacquot, A., Liu, W.L., Chen, G., Fleurial, J.-P., Dauscher, A., and Lenoir, B., “Fabrication and Modeling of an In-Plane Thermoelectric Microgenerator,” Proceedings of Twenty-First International Conference on Thermoelectrics, pp. 561-564, 2002.</li>
	<li class="list-num-1-51 list-num-paddingleft-1"><a href="http://www.adsx.com/content/index.htm">http://www.adsx.com/content/index.htm</a>.</li>
	<li class="list-num-1-52 list-num-paddingleft-1"><a href="http://www.dts-generator.com/main-e.htm">http://www.dts-generator.com/main-e.htm</a>.</li>
	<li class="list-num-1-53 list-num-paddingleft-1">Qu, W., et al., “Microfabrication of Thermoelectric Generators on Flexible Foil Substrates as a Power Source for Autonomous Microsystems,” J. Micromech. Microeng., Vol. 11, pp. 146-152, 2001.</li>
	<li class="list-num-1-54 list-num-paddingleft-1">Yu, H., et al., “In Situ Growth of C-Axis-Oriented Ca3Co4O9 Thin Films on Si (100),” Appl. Phys. Lett., Vol. 86, 082103, 2005.</li>
	<li class="list-num-1-55 list-num-paddingleft-1">http://www.enerdynesolutions.com/tech_polara.html</li>
	<li class="list-num-1-56 list-num-paddingleft-1">Venkatasubramanian, R., Silvola, E., Colpitts, T., O’quinn, B, “Thin-film Thermoelectric Devices With High Room-Temperature Figures of Merit, Nature  413, pp. 597-602, October 2001.</li>
	<li class="list-num-1-57 list-num-paddingleft-1">Zeng, G., et al., “Cooling Power Density of SiGe/Si Superlattice Micro Refrigerators,” Mat. Res. Soc. Symp. Proc., Vol. 793, 2004.</li>
	<li class="list-num-1-58 list-num-paddingleft-1">Humphrey, T., and Linke, H., “Reversible Thermoelectric Materials,” Phys. Rev. Letters, Vol. 94, 096601, 2005.</li>
	<li class="list-num-1-59 list-num-paddingleft-1">Korotkov, N., and Likharev, K.K., “Possible Cooling by Resonant Fowler-Nordheim Emission, Appl. Phys. Lett., Vol.75, p. 2491, 1999.</li>
	<li class="list-num-1-60 list-num-paddingleft-1"><a href="http://www.powerchips.gi/index.shtml">http://www.powerchips.gi/index.shtml</a>.</li>
	<li class="list-num-1-61 list-num-paddingleft-1">Hishinuma, Y., Geballe, T., Moyzhes, B., and Kenny, T., “Refrigeration by Combined Tunneling and Thermionic Emission in Vacuum: Use of Nanometer Scale Design,” Appl. Phys. Lett., Vol. 78, No. 17, pp. 2572-2574, 2001.</li>
	<li class="list-num-1-62 list-num-paddingleft-1">Despesse, G., and Jager, T., “Exploitation of the Thermotunnel Effect for Energy Scavenging,” Appl. Phys. Lett.. Vol. 96, No. 9, pp. 5026-5031, 2004.</li>
	<li class="list-num-1-63 list-num-paddingleft-1">Chua, H., et al., “Thermionic and Tunneling Cooling Thermodynamics,” Appl. Phys. Lett., Vol. 84, pp. 3999-4001, 2004.</li>
	<li class="list-num-1-64 list-num-paddingleft-1">Gerstenmaier, Y. and Wachutka, G., “Thermionic Refrigeration with Planar and Nonplanar Electrodes: Chances and Limits”, Proceedings 11th THERMINIC, September 27-30, Belgirate, Italy, 2005, pp. 270-277</li>
	<li class="list-num-1-65 list-num-paddingleft-1">Krishnan, S., and Garimella, S., “Thermal Management of Transient Power Spikes in Electronics – Phase Change Energy Storage or Copper Heat Sinks?”, IPACK2003, Maui, HI, Ppaper # 35169, 2003.</li>
	<li class="list-num-1-66 list-num-paddingleft-1">Levitskij, E.A., Aristov, Yu. I., Tokarev, V.N., and Parmon, V.N., “Chemical Heat Accumulator,” Solar Energy Material and Solar Cells, 44, pp. 219-235, 1996.</li>
</ol>
&nbsp;