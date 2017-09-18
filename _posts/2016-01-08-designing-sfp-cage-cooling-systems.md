---
ID: 72
post_title: Designing SFP Cage Cooling Systems
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/72
published: true
post_date: 2016-01-08 18:45:19
---
by Herbert Endres, Molex

Sealed small form-factor pluggable (SFP) optical and electrical integrated assemblies play an important role on printed-circuit boards (PCBs) by maximizing valuable space while providing an environmentally rugged interface. Designers currently have two choices when it comes to SFPs. Regular SFP interconnects support 1.125-Gbit/s Fibre Channel and 2.5-Gbit/s Gigabit Ethernet applications, while the more advanced SPF+ interconnects support applications for 8-Gbit/s Fibre Channel and 10-Gbit/s Gigabit Ethernet. Both interconnect types use the same space per port.
<h3>Table Of Contents</h3>
<ol>
	<li>Is Cooling Necessary?</li>
	<li>Dissipated Heat Guidelines</li>
	<li>Heatsink And Baffle Recommendations</li>
</ol>
&nbsp;
<h3>Is Cooling Necessary?</h3>
Featuring a panel feed-through design, SFP assemblies typically incorporate an internally mounted cage and related electrical circuitry. One of the key considerations when it comes to the cage is whether or not cooling is necessary. There is no clear answer to this question, so it’s critical for design engineers to consider several factors.

First, consider the heat dissipation of one SFP insert, which can range from zero (passive copper cable) to approximately 2 W when using twin bi-directional LC inserts. Next, consider the equipment practice. It may be a rack with vertical daughter cards, but it could also be a wide and flat “pizza box” with only a main board or with additional mezzanine cards on top.

Also, consider the number and the density of the ports on the daughter card/mezzanine board. These ports can be single cages with space in between, ganged cages, or stacked and ganged cages. Then, there’s the airflow in the system. It always occurs bottom-to-up in a rack but may be different in a pizza box, such as east-to-west or front-to-rear. Finally, consider the ambient temperature (fan-supported approximately 40°C), the maximum allowed temperature for the insert (typically 70°C), and the airflow speed.
<h3>Dissipated Heat Guidelines</h3>
We have conducted many simulations in our thermal labs to understand the results of these factors. There is no universal clear-cut solution for the problem. But for single cages with spaces in between, engineers are on the safe side if the dissipated heat is below 1 W per insert. When ganging cages, there is still no heat problem, assuming there’s a copper ground plane underneath the inserts that distribute the heat.

If dissipated heat rises above 1 W per insert, care should be taken, especially when ganged SFP cages are preferred or required. A fully SFP-loaded front panel configured with inserts above 1.5-W heat dissipation for each insert requires cooling.

The first hurdle in cooling is finding a good thermal connection between the insert and the heatsink. Only quad small form-factor pluggable (QSFP) inserts have a flat and smooth surface on top for close contact to a heatsink. SFP inserts don’t always have this kind of surface. Even worse, some are manufactured with the label on top, which does not conduct heat well. Engineers can improve the situation with conductive heat cushions, but the thermal contact remains questionable <em>(Fig. 1)</em>.
<div class="captioned-image caption-none"><img class="alignnone size-full wp-image-73" src="http://en.mekesim.com/wp-content/uploads/2016/01/74327_f1-sm.jpg" alt="" width="390" height="178" /></div>
<span class="imagecaption">1. SFP inserts do not always have a flat and smooth surface for close contact to a heatsink. Some are manufactured with the label on top, which does not conduct heat well. Design engineers can improve the situation by installing conductive heat cushions like the one shown above.</span>

Using a defined insert with a defined heat cushion, the second hurdle is selecting the right heatsink in the given environment. One tested arrangement used a rack with vertical daughter cards and 24 ganged SFP ports (four cages for each of the six ports). Given the height of only 15.2 mm above the board, it was clear that a heatsink on top of the SFP cages would block the airflow. This situation is actually worse than using no heatsinks.
<h3>Heatsink And Baffle Recommendations</h3>
Heatsinks should have fingers (no ribs) to create turbulence and generate better thermal conductivity to the air. Testing has shown that “rucksack” heatsinks are a good solution. A lower-profile heatsink with a rucksack is more efficient than a higher heatsink just above the cages.

We tested several heatsink configurations and found the lower-profile, longer rucksack as the best performer. But even with the extended rucksack, we had to apply a baffle to squeeze the airflow onto the rucksack area <em>(Fig. 2)</em>. We then created a heatsink comparison matrix that shows some interesting findings:
<ul>
	<li>Installing heatsinks is sometimes worse than not installing heatsinks.</li>
	<li>Without a baffle, airflow bypasses the heatsink area, so the airflow is in vain.</li>
	<li>Adding more baffles doesn’t improve the cooling effect.</li>
	<li>Most critical is the swelter effect. The lower SFPs heat up the upper SFPs when airflow is not controlled.</li>
</ul>
<div class="captioned-image caption-none"><img class="alignnone size-full wp-image-74" src="http://en.mekesim.com/wp-content/uploads/2016/01/74327_f2-sm.jpg" alt="" width="280" height="569" /></div>
<span class="imagecaption">2. Molex tested heatsinks using no rucksack (a) and a short rucksack (b) but found the lower-profile, longer rucksack to work most effectively (c). Testing revealed that even with an extended rucksack, designers should apply a baffle to squeeze the airflow onto the rucksack area.</span>

We also simulated and verified thermal issues with stacked and ganged configurations of SFP and QSFP, as we foresee a wider usage of cages in the industry—not only with heat dissipation from fiber-optic transceivers, but also with dissipated heat from active copper cables where equalizers are integrated into the cable plugs.

Determining the correct SFP cage cooling system is important because of the many benefits an SFP that functions well can provide when designed properly. For example, SFP transceivers not only can be installed into the front to allow for convenient factory pre-installations, they also can be removed and replaced for easy field upgrades.