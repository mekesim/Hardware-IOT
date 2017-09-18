---
ID: 246
post_title: >
  Understanding dissipation, thermal
  resistance, and IC temperature (Part 1
  of 2)
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/246
published: true
post_date: 2016-03-03 11:25:06
---
<div class="divsplitter">System designers and board designers have to design their board to handle the heat generated due to power consumption in the ICs. A good understanding of thermal resistance and its implication on power dissipation and heat generation is essential. This knowledge enables designers to determine board layout requirements and system requirement and, as a result, to prevent both overheating of the board and catastrophic IC failure.</div>
<div class="grayshowlinks bigsmall">

This article discusses the relationship between thermal resistance value, power dissipation, and temperature (junction temperature), using the MIC94060 high-side power switch as an example. A method for calculating the thermal resistance of IC will be described, which can be used by system and board designer for calculating the thermal resistance of other ICs on the board.

<b>Thermal resistance of MIC94060</b>

Micrel's MIC94060 is offered in SC70 package and MLF packages. The MIC94060 high-side power switch or load switch is used as a switch to enable or disable power to the load circuit. When the switch is enabled, the load gets powered; when the switch is disabled, the load does not get power. It is placed between a power source and the load circuit. The primary focus here is to characterize the thermal performance of MIC94060 in the SC70 package. A typical application of MIC94060 is shown in<b>Figure 1</b>.

<center><a href="http://m.eet.com/media/1050386/C0230-Figure1.gif"><img src="http://m.eet.com/media/1050386/C0230-Figure1.gif" alt="" width="350" height="190" border="0" /></a>
<i>Figure 1: Typical MIC94060 application </i>
<i>(Click to enlarge image)</i></center>
The MIC94060 has 6 pins in the SC70 package, described in<b>Table 1</b>.

<center><a href="http://m.eet.com/media/1050387/C0230-Table1.gif"><img src="http://m.eet.com/media/1050387/C0230-Table1.gif" alt="" width="350" height="115" border="0" /></a>
<i>Table 1: MIC94060 pin description </i>
<i>(Click to enlarge image)</i></center>
The thermal resistance of an IC package is defined as the amount of heat generated or a rise in temperature when 1 W of power is dissipated in the IC. The thermal resistance of a MIC94060 SC70 package as listed in the datasheet as 240° C/W. This means that when one watt of power is dissipated, the IC's junction temperature would increase by 240 degrees <a href="http://www.planetanalog.com/encyclopedia/defineterm.jhtml?term=C&amp;x=&amp;y=">C</a> over the ambient temperature.

The equation that relates junction temperature T<sub>j</sub> to thermal resistance θ<sub>Ja</sub> is: T<sub>j</sub>=T<sub>a</sub>+ θ<sub>Ja</sub>× Power dissipation

where T<sub>a</sub> is the ambient temperature.

The maximum junction temperature (T<sub>j</sub>) allowed for MIC94060 listed in the datasheet is 125° C. Hence, to prevent the junction temperature from rising above 125°, either the amount of power dissipated in the IC must be controlled, or the maximum ambient temperature must be controlled. For example, for θ<sub>Ja</sub> = 240° C/Watt, maximum T<sub>j</sub> = 125° C and R<sub>ds(on)</sub>=100 mΩ, then <b>Table 2</b>lists the maximum ambient temperature allowed for various amount of power dissipation.

Power dissipation (P<sub>d</sub>)=R<sub>ds(on)</sub>× I<sub>out</sub> × <sub>Iout</sub>
T<sub>j</sub>= T<sub>a</sub> + θ<sub>Ja</sub>× P<sub>d</sub>
125=T<sub>a</sub>+240 × P<sub>d</sub>
T<sub>a</sub>=125 - 240 × P<sub>d</sub>

<center><a href="http://m.eet.com/media/1050388/C0230-Table2.gif"><img src="http://m.eet.com/media/1050388/C0230-Table2.gif" alt="" width="350" height="70" border="0" data-pin-nopin="true" /></a>
<i>Table 2: Maximum ambient temperature versus power dissipation </i>
<i>(Click to enlarge image)</i></center>
From Table 2, it is clear that the MIC94060 would not reliably operate above the ambient temperature of 29° C, when the load current is 2 A. But can this be true? Currently, the MIC94060 is able to pass 2 A without any heating problems on my board. So, what is the explanation for discrepancy between theoretical and real observation? Clearly, the value of thermal resistance of 240° C/W specified in the datasheet cannot be used for my board. The thermal resistance value of 240° C/W is obtained from JEDEC standard,. plus an additional safety number is added. A method for calculating a more accurate thermal resistance for the current board is described in the next subsection.

The higher the θ<sub>Ja</sub> (thermal resistance) of the package, the hotter the IC will become for a given amount of power dissipation (higher junction temperature). <b>Table 3</b> helps to visualize the affect of θ<sub>Ja</sub>on junction temperature T<sub>j</sub> for 400 mW of power dissipation in the IC.

T<sub>j</sub>=T<sub>a</sub> + θ<sub>Ja</sub> × 400 mW

<center><a href="http://m.eet.com/media/1050389/C0230-Table3.gif"><img src="http://m.eet.com/media/1050389/C0230-Table3.gif" alt="" width="350" height="90" border="0" /></a>
<i>Table 3: Thermal Resistance θ<sub>Ja</sub> versus junction temperature T<sub>j</sub> </i>
<i>(Click to enlarge image)</i></center>
Thus, a higher θ<sub>Ja</sub> value leads to higher junction temperature for a given amount of power dissipation.

<b>Power dissipation for the MIC94060</b>

The power dissipation for Micrel's MIC94060 switch is calculated as: R<sub>ds(on)</sub> × I<sub>out</sub>×I<sub>out</sub> where R<sub>ds(on)</sub> is the on-resistance of the switch and I<sub>out</sub> is the load current or output current. The R<sub>ds(on)</sub> of MIC94060 for various values of V<sub>in</sub> and I<sub>out</sub> (load current) is shown in <b>Figure 2</b>. The R<sub>ds(on)</sub> of MIC94060 is typically 77 mΩ. For the purpose of calculating thermal resistance, the R<sub>ds(on)</sub>value of 100 mΩ is used in the next subsection.

<center><a href="http://m.eet.com/media/1050390/C0230-Figure2.gif"><img src="http://m.eet.com/media/1050390/C0230-Figure2.gif" alt="" width="350" height="350" border="0" /></a>
<i>Figure 2: On-resistance R<sub>ds(on)</sub> of the MIC94060 </i>
<i>(Click to enlarge image)</i></center>
<b>Finding the thermal resistance</b>

The thermal resistance is given as θ<sub>Ja</sub> (junction temperature with respect to ambient temperature) or θ<sub>Jc</sub> (junction temperature with respect to case temperature).

The thermal resistance:

θ<sub>Ja</sub> = T<sub>j</sub> - T<sub>a</sub>/(power dissipation).

θ<sub>Jc</sub> = T<sub>j</sub> - T<sub>c</sub>/(power dissipation).

T<sub>j</sub> is the junction temperature, T<sub>a</sub>is the ambient temperature and T<sub>c</sub> is the case temperature.

<b>Characterizing junction temperature</b>

The junction temperature T<sub>j</sub> cannot directly be measured; rather it must be inferred from the characterization data of a temperature dependent parameter of the IC. For the MIC94060, an internal pull-down resistor on the enable pin displays temperature-dependent behavior. Therefore, the internal pull-down resistor's value is the temperature-dependent parameter. The input resistance on the enable pin increases linearly with rise in temperature. So, with a constant voltage applied on the enable pin, the enable input current should decrease linearly with rise in temperature.

A graph of temperature on x-axis and enable pin current on y-axis is created using a setup with a test board (copper board) 60 mm by 35 mm, shown in <b>Figure 3</b> and <b>Figure 4</b>.

<center><a href="http://m.eet.com/media/1050391/C0230-Figure3.gif"><img src="http://m.eet.com/media/1050391/C0230-Figure3.gif" alt="" width="350" height="265" border="0" /></a>
<i>Figure 3: MIC94060 test board. </i>
<i>(Click to enlarge image)</i></center>
<center><a href="http://m.eet.com/media/1050392/C0230-Figure4.gif"><img src="http://m.eet.com/media/1050392/C0230-Figure4.gif" alt="" width="350" height="260" border="0" /></a>
<i>Figure 4: MIC94060 test board. </i>
<i>(Click to enlarge image)</i></center>
The top surface has the V<sub>in</sub> trace, V<sub>out</sub> trace and enable trace. The rest of the top surface and the bottom surface is ground plane. The NIC pin of MIC94060 is left floating and is not soldered on the board. Five tests points, one each for the V<sub>in</sub> pin, V<sub>out</sub> pin, and enable pin, and two for ground pin are also present on the top surface. The test board is placed inside a circular enclosure which protrudes from an elephant temperature system, <b>Figure 5</b>.

<center><a href="http://m.eet.com/media/1050393/C0230-Figure5.gif"><img src="http://m.eet.com/media/1050393/C0230-Figure5.gif" alt="" width="350" height="155" border="0" /></a>
<i>Figure 5: ?Elephant temperature system. </i>
<i>(Click to enlarge image)</i></center>
The elephant temperature system is used to control the temperature inside the circular enclosure and thus the temperature of the test board. Once the temperature is set, the board is left undisturbed for at least half hour to allow the IC and the test board to reach a thermal equilibrium. Once the thermal equilibrium has been reached, the junction temperature of IC (T<sub>j</sub>) will equal to temperature of test board which will then equal to the ambient temperature (T<sub>a</sub>).

Thus ambient temperature (T<sub>a</sub>) = test board temperature

= case temperature (T<sub>c</sub>)

= junction temperature (T<sub>j</sub>)

With 3V applied on the V-enable pin, the current I-enable is measured. A graph of I-enable versus temperature is obtained by changing the temperature setting of the elephant system, <b>Figure 6</b> and <b>Figure 7</b>.

<center><a href="http://m.eet.com/media/1050394/C0230-Figure6.gif"><img src="http://m.eet.com/media/1050394/C0230-Figure6.gif" alt="" width="350" height="260" border="0" /></a>
<i>Figure 6: Enable current versus temperature. </i>
<i>(Click to enlarge image)</i></center>
<center><a href="http://m.eet.com/media/1050395/C0230-Figure7.gif"><img src="http://m.eet.com/media/1050395/C0230-Figure7.gif" alt="" width="350" height="210" border="0" /></a>
<i>Figure 7: Enable current versus temperature. </i>
<i>(Click to enlarge image)</i></center>
<b>(Note: Part 2</b> discusses thermal resistance measurements for θ<sub>Jc</sub>and θ<sub>Ja</sub> as well as conclusions. Click <a href="http://www.planetanalog.com/features/showArticle.jhtml;jsessionid=FORSCMYRYPJHEQSNDLRCKHSCJUNN2JVN?articleID=202102839">here</a> to read Part 2.)

<b>About the author</b>

<b><i>Hardik Patel</i></b> joined <a href="http://www.micrel.com/">Micrel, Inc.</a> in October 2000 as an application engineer. In 2003 he worked at iWatt as a Test Development Engineer, then rejoined Micrel in 2005 and became a Senior Application Engineer. He is currently responsible for new product evaluation, designing customer evaluation boards, and softwareand customer technical support. He handles Micrel's high-side power-distribution switches, current-limiting switches, temperature sensors, voltage supervisors, latch drivers, display drivers, fan controllers, and USB transceivers. He holds a Bachelor of Applied Science from University of Toronto in Electrical Engineering. He also is the author of several technical articles and has one patent pending.

</div>