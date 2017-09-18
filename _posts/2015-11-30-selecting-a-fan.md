---
ID: 32
post_title: Selecting A Fan
author: admin
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/32
published: true
post_date: 2015-11-30 03:21:58
---
<p class="authorName">By Norm Quesnal - Advanced Thermal Solutions, Inc.</p>
<p class="articleDate">2015-07-22</p>

<div id="article" class="article">
<div id="pagelayout_0_content_0_articlecontent_0_richtextcontent" dir="ltr">

Designing a forced convection cooling system for a chassis or cabinet can be a complicated task. However, it must be done correctly to ensure the performance and reliability of the enclosed electronics. Many different thermal, mechanical and electrical effects must be considered for the successful design of such cooling systems<sup>1</sup>.

The first step is to determine the type of fan that’s needed. This will be based mainly on the chassis design and the allowable space.

There are two major fan types:

1. <a href="http://www.digikey.ca/product-search/en?KeyWords=fans%20axial%20~%20access%20~%20finger">Vane-Axial Fans</a> – Air flow is parallel to the fan’s axis. It provides a high air flow rate with low pressure (Figure 1).

2. <a href="http://www.digikey.ca/product-search/en?KeyWords=fans%20blower%20~%20access">Blower Fans</a> – Air flow from this fan type is perpendicular to its axis. The air flow rate is low and there is high pressure (Figures 2-4).

<img class="alignnone size-full wp-image-43" title="Sanyo Denki vane-axial fan" src="http://en.mekesim.com/wp-content/uploads/2015/12/article-2015july-selecting-a-fan-fig1.jpg" alt="Image of Sanyo Denki vane-axial fan" width="241" height="232" />

<em>Figure 1: Sanyo Denki vane-axial fan.</em>

<em><img class="alignnone size-full wp-image-44" title="Sanyo Denki blower fan" src="http://en.mekesim.com/wp-content/uploads/2015/12/article-2015july-selecting-a-fan-fig2.jpg" alt="Image of Sanyo Denki blower fan" width="239" height="245" />
</em>

<em>Figure 2: Sanyo Denki blower fan.</em>

<em><img class="alignnone size-full wp-image-45" title="Eucania tangenial blowers" src="http://en.mekesim.com/wp-content/uploads/2015/12/article-2015july-selecting-a-fan-fig3.jpg" alt="Image of Eucania tangenial blowers" width="382" height="255" />
</em>

<em>Figure 3: Eucania tangenial blowers.</em>

<em><img class="alignnone size-full wp-image-46" title="Eucania intergrated blower" src="http://en.mekesim.com/wp-content/uploads/2015/12/article-2015july-selecting-a-fan-fig4.jpg" alt="Image of Eucania intergrated blower" width="300" height="262" />
</em>

<em>Figure 4: Eucania intergrated blower.</em>

To select the appropriate fan, we must estimate the system’s air flow requirements. For low power, uniform heat loads we can use a simple, steady-state analysis to balance air flow and temperature rise.

The power dissipation of the chassis, and the desired temperature rise, are used in the following equation to obtain a target flow rate<sup>2</sup>:

<img src="http://www.digikey.com/-/media/Images/Article%20Library/TechZone%20Articles/2015/July/Selecting%20A%20Fan/article-2015july-selecting-a-fan-equation1.jpg?la=en&amp;ts=42c718d0-eeba-41f4-95ec-20c64844f344" alt="Equation 1" width="88" height="28" />

Where:

Q = heat dissipated in enclosure
ṁ = mass flow rate through enclosure
<em>C<sub>P</sub></em> = specific heat of air
Δ<em>T</em> = target temperature rises from intake to exhaust

For high thermal loads with concentrated heat sources, one must design to the worst case component temperature. Spot cooling may be accomplished with internal fans, heatsinks, ducting, and other methods.

Next, the total system thermal impedance curve is needed, or at the very least, you should know the system pressure drop at the desired flow rate.

System resistance is defined as:

<img src="http://www.digikey.com/-/media/Images/Article%20Library/TechZone%20Articles/2015/July/Selecting%20A%20Fan/article-2015july-selecting-a-fan-equation2.jpg?la=en&amp;ts=bb30f130-f421-4fc3-a3dd-0edd185c842f" alt="Equation 2" width="75" height="23" />

Where:

<em>P</em> = system pressure
<em>K</em> = load factor (system dependent)
ρ = air density
<em>Q</em> = air flow rate
<sup><em>n</em></sup> = air flow quality constant; varies between 1 (laminar) and 2 (turbulent)

For practical purposes, the value of <em>K</em> can only be found experimentally or by using computational fluid dynamics. Due to the complex nature of today’s electronic enclosures, an accurate value for <em>K</em> cannot be derived analytically. In a modern enclosure, the air flow is mixed (laminar, turbulent, pulsetile, etc.) and the value of <em>n</em>   can be conservatively chosen as 2.

The calculated flow rate at a specific static pressure can be compared to a specific fan curve. This will determine if the fan will be adequate. An example of a fan curve is shown in Figure 5. Point A is known as the “no flow” point of the curve, where the fan is producing the highest pressure possible. Next is the stall region of the fan, B, which is an unstable operating area and should be avoided. The region from point C to D is the low pressure area of the fan curve. This is a stable region of fan operation and should be the design goal. It is best to select a fan that performs to the higher flow area of this region to improve fan efficiency and compensate for filter clogging.

<img class="alignnone size-full wp-image-47" title="Typical fan and impedance curves" src="http://en.mekesim.com/wp-content/uploads/2015/12/article-2015july-selecting-a-fan-fig5.jpg" alt="Image of typical fan and impedance curves" width="360" height="309" />

<em>Figure 5: Typical fan and impedance curves<sup>3</sup>.</em>

In many systems, a single fan cannot deliver the full volumetric flow rate needed. In these situations multiple fans can be used, configured either in parallel or in series. In order to determine which configuration is more appropriate, the system impedance curve is needed once again (Figure 6). For a high impedance system, two fans in series will produce a higher flow rate than they will in parallel. The opposite behavior can be expected in a low impedance system, where parallel fans are preferred.

An important step to be addressed once the fans have been selected is to configure them in a blow-through or pull-through arrangement. The air flow into a fan can roughly be modeled as laminar, whereas the exit air flow is highly mixed. This phenomenon can be useful in thermal management. An example of this is seen inside a typical telecom sub-rack. Due to the varied resistance that the PCBs impose, and the close proximity of the fans (fan tray) to the cards, the conditioned flow will help provide better velocity distribution in the sub-rack, which also functions as a plenum.

<img class="alignnone size-full wp-image-48" title="The effect of multiple fans on system pressure and flow rate" src="http://en.mekesim.com/wp-content/uploads/2015/12/article-2015july-selecting-a-fan-fig6.jpg" alt="Image of the effect of multiple fans on system pressure and flow rate" width="467" height="235" />

<em>Figure 6: The effect of multiple fans on system pressure and flow rate<sup>4</sup>.</em>

In the blow-through configuration, the turbulent air has a positive effect on the heat transfer coefficient. This can be useful when dealing with concentrated heat sources. The blow-through design allows the fan to push cooler air, which improves its pressure capability and extends the life of the fan. In this arrangement the enclosure is slightly pressurized. This prevents unfiltered air from being drawn through the joints and gaps in the chassis.

<strong>Common Fan Laws</strong>

<img class="alignnone size-full wp-image-49" src="http://en.mekesim.com/wp-content/uploads/2015/12/article-2015july-selecting-a-fan-equation7.jpg" alt="Equations 3-6" width="243" height="141" />

Where:

<em>K</em> = constant for geometrically and dynamically similar operation
<em>G</em> = volumetric flow rate
<em>N</em> = fan speed in RPM
<em>HP</em> = power output
ṁ = mass flow rate
<em>D</em> = fan diameter
ρ = air density

<em>This article first appeared in the <a href="http://www.qats.com/Qpedia-Thermal-eMagazine/">Qpedia Thermal eNewsletter</a> in March, 2007.</em>

<strong>References:</strong>
<ol>
	<li>Ellison, G., Fan Cooled Enclosure Analysis Using a First Order Method, Electronics Cooling, October 1995.</li>
	<li>Turner, M., All You Need to Know About Fans, Electronics Cooling, May 1996.</li>
	<li>Daly, B., Woods Practical Guide to Fan Engineering, Woods of Colchester, Ltd, 1992.</li>
	<li>Comair Rotron, <a href="http://www.digikey.ca/en/pdf/c/comair-rotron/comair-tutorial-establishingcoolingrequirements">Establishing Cooling Requirements: Air Flow vs Pressure</a>, March 12, 2007.</li>
</ol>
</div>
</div>
&nbsp;