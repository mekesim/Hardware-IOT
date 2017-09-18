---
ID: 201
post_title: >
  Tablet Natural Convection Cooling
  Efficiency
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/201
published: true
post_date: 2016-02-02 10:56:59
---
<h3>By Guy R. Wagner and William Maltz</h3>
<h2><em><strong>Abstract</strong></em></h2>
<em>This study explores the limits of natural convection cooling for handheld devices based on both testing and simulation under various conditions and proposes a figure of merit for the efficiency of heat dissipation. The factors affecting the maximum possible power dissipation are the available surface area and surface finishes, selection of the outer shell materials, thermal interface materials, heat spreaders and air gaps. In most cases, the limiting factor in the thermal design of these devices is not the temperatures of the internal components but the temperature of the external surfaces since these are in direct contact with the skin of the user. There have been studies that address the maximum allowable comfortable touch temperature of a handheld device. This study presents a method for analyzing the quality of the thermal design of these devices. <span id="more-14"></span></em>

<strong>1. Introduction</strong>

With the rapidly increasing performance in tablets and smart phones, the result is increased power consumption leading to devices that are uncomfortably hot to hold. This is especially true since watching video or playing games on these devices has become very popular. These types of operations are both CPU and graphics intensive which involves much higher power dissipation than viewing a relatively static screen. The thermal design of the next generation handheld tablet device and smart phone will need to address both a comfortable surface touch temperature and maximum temperature limitations of critical internal components while also meeting aggressive industrial design requirements.

Users are rapidly switching from desktop computers and laptop computers to tablets and smart phones for their computing, gaming and communication needs. These handheld devices are increasingly capable of running applications that used to require their more powerful predecessors. With a smaller form factor, this presents significant challenges, especially when one considers that passive cooling is almost a requirement.

The limits of cooling for handheld devices explored in this study are based on both testing and simulation under various conditions and provides a method for evaluating the quality of the cooling solution for these devices. Factors affecting the maximum possible power dissipation are surface area and emissivity, outer shell materials, thermal interface materials, heat spreader properties and air gaps. The limiting factor in the thermal design of these devices is generally the touch temperature of external surfaces. There have been studies that address the maximum allowable comfortable touch temperature of a handheld device. This study discusses the effect of maximizing the heat spreading within these devices which aids in keeping the touch temperatures of these devices within comfortable limits.

<strong>2. Performance Expectations</strong>

With the switch from desktop computers to laptops and now tablets, these handheld devices are increasingly capable of running applications that used to require their more powerful predecessors. The user expects that these devices provide similar performance to that which they had become accustom to in previous computers. This presents significant challenges, especially when one considers that passive cooling is almost a requirement in these small form factor devices. Several studies have focused on the cooling challenges of hand-held devices; Brown et al [2], Lee et al [5], Mongia et al [6], Huh et al [4], and Gurrum et al [3].

<strong>3. Maximum Power Dissipation</strong>
<img class="alignnone size-full wp-image-202" src="http://www.mekesim.com/wp-content/uploads/2016/02/1.png" width="244" height="300" alt="FloTHERM® CFD Model of a 10 Inch Tablet in a Vertical Orientation" />
<p class="wp-caption-text">FloTHERM® CFD Model of a 10 Inch Tablet in a Vertical Orientation</p>
The maximum possible power dissipation by natural convection and radiation has been calculated for this study using FloTHERM® CFD simulations is shown in Figure 1. In a 25°C ambient condition, the maximum total power dissipation is calculated with a requirement that the surface temperature does not exceed a touch temperature of 41°C. This is the maximum aluminum enclosure comfort touch temperature as presented by Berhe [1].

It can be seen that the theoretical maximum total power dissipation is 17.1 watts when a 10 inch tablet is suspended vertically in midair with conduction and radiation occurring from all surfaces. When the device is placed on a horizontal adiabatic surface, heat transfer is occurring from the sides and front surface only. These values establish bounds for the maximum amount of heat that can be dissipated by the device for different orientations in still air.

<img class="alignnone size-full wp-image-203" src="http://www.mekesim.com/wp-content/uploads/2016/02/2.png" width="300" height="241" alt="Figure 2. Temperature Rise Above Ambient as a Function of Tablet Power" />
<p class="wp-caption-text">Figure 2. Temperature Rise Above Ambient as a Function of Tablet Power</p>
In order to calculate the total power dissipation for a full-size tablet, the following assumptions were made as inputs to the FloTHERM<sup>®</sup> model with 610k elements: a typical 10 inch tablet size of 180 mm by 240 mm by 10 mm and an ideal condition of uniform surface temperature. The tablet was simulated as a very high thermal conductivity block (k = 10000 W/mK) with uniform internal heat generation to yield an essentially isothermal surface. With an ideal surface emissivity of 1.0, the radiant heat transfer component accounts for a surprising 9.9 watts of the 17.1 watts total power while the convective heat transfer component is 7.2 watts. Since radiation can account for more than half of the total power dissipation at an ambient temperature of 25°C, the use of high emissivity surfaces finishes is very important.

In order to achieve maximum power dissipation, design parameters need to be considered carefully. It is important to design the device to be as isothermal as possible to maximize the amount of heat transfer from all surfaces to the surroundings. The reason for this is so that all surface areas of the device are as far above ambient temperature as possible to maximize heat transfer without exceeding the maximum allowable touch temperature. When a surface is no longer available for heat transfer, such as when the device is placed on a blanket, the amount of power that can be dissipated is almost cut in half.

<img class="alignnone size-full wp-image-204" src="http://www.mekesim.com/wp-content/uploads/2016/02/3.png" width="300" height="244" alt="Figure 3. Power Dissipation vs Surface Area for a Device with a 41C Skin Temperature" />
<p class="wp-caption-text">Figure 3. Power Dissipation vs Surface Area for a Device with a 41C Skin Temperature</p>
If the power dissipation at 41C maximum touch temperature is calculated using CFD for three devices ranging from smart phone size through mini tablet size and a full-size tablet, the power dissipation versus surface area is shown in Figure 3 for the device in both the vertical position and the horizontal position with an adiabatic lower surface. There is a high probability that the tablet will be used in the horizontal position with a near-adiabatic lower surface while the smart phone will rarely be run in this orientation. From the power and temperature rise computations, it is now possible to calculate the thermal resistance of a vertical, isothermal tablet as a function of the exposed surface area as shown in figure 4.

<img class="alignnone size-full wp-image-205" src="http://www.mekesim.com/wp-content/uploads/2016/02/4.png" width="300" height="247" alt="Figure 4. Thernal Resistance vs Surface Area for a Vertical Isothermal Device with a 41C Skin Temperature" />
<p class="wp-caption-text">Figure 4. Thernal Resistance vs Surface Area for a Vertical Isothermal Device with a 41C Skin Temperature</p>
<strong>4. Numerical Models</strong>

In order to analyze the impact of different thermal management techniques, a detailed computational fluid dynamics (CFD) thermal model is constructed using FloTHERM XT<sup>®</sup>. Since the thermal characterization data of the main processor in the tablet may not be known, the thermal characteristics of the actual processor can be measured with a high degree of accuracy using a Mentor Graphics T3Ster<sup>®</sup> to determine the thermal resistance from the processor IC to the case and the PCB; Wagner et al [7].

<img class="alignnone size-full wp-image-206" src="http://www.mekesim.com/wp-content/uploads/2016/02/5.png" width="300" height="237" alt="Figure 5. Flotherm XT Model of the Internal Component Temperatures of a Tablet" />
<p class="wp-caption-text">Figure 5. Flotherm XT Model of the Internal Component Temperatures of a Tablet</p>
<img class="alignnone size-full wp-image-207" src="http://www.mekesim.com/wp-content/uploads/2016/02/6.png" width="230" height="299" alt="Figure 6. Flotherm XT Model Showing the Hot Spot and the Natural Convection Airflow around the Back of a Tablet" />
<p class="wp-caption-text">Figure 6. Flotherm XT Model Showing the Hot Spot and the Natural Convection Airflow around the Back of a Tablet</p>
This allows accurate capture of heat flow from the top and bottom of the processor. The thermal model of the processor can be directly dropped into the tablet CFD model. The adaptive mesh in FloTHERM XT<sup>®</sup> allows the fine features of the internal components of the tablet to be included in the model while keeping the mesh count to a reasonable size as shown in figures 5 and 6.

With the CFD thermal model, the following questions can be addressed:
<ol>
	<li>How much do high-conductivity heat spreaders improve heat dissipation while reducing the touch temperature?</li>
	<li>What is the best way to move the heat from the heat-producing components to the surfaces of the tablet where it can be safely dissipated?</li>
	<li>How are air gaps strategically used in the thermal management process?</li>
	<li>How important it is to account for radiation in addition to convection?</li>
	<li>Should the dissipated power be spread at the source or at the surface?</li>
	<li>How does designing the tablet with a plastic case compare to an aluminum or magnesium case?</li>
</ol>
Since we have a goal of keeping touch temperature at or below 41°C, answering question #1 will have a large impact on the design.

Temperature uniformity can be achieved by either providing a high conductivity heat spreader inside the case of the tablet or by making the case itself out of a high conductivity material; Wagner et al [8]. One must keep in mind that the maximum touch temperature is a strong function of the conductivity of the heat spreader or case.

Keep in mind that as the conductivity of the case goes down the maximum comfortable touch temperature increases. For example, if the case is made of plastic with a thermal conductivity in the range of 0.2 W/mK, the case temperature that the user senses feels cooler since the low thermal conductivity of the plastic results in less heat being conducted to the user’s skin. The apparent touch temperature decreases as the product of thermal conductivity * density * specific heat of the case material decreases. When this product is low, the touch temperature may be increased by approximately 5C over that of a solid metal case. Since the surface area of the case is large in relation to the thickness of the plastic, heat transfer to the air is not reduced significantly over that of an aluminum case. This of course assumes that the heat is spread on the inside of the plastic case using a high-conductivity aluminium plate or graphite sheet.

<strong>5. Infrared Images</strong>

When evaluating the effectiveness of heat spreaders, whether internal or through the use of high conductivity case material, it is very useful to take infrared images of the units under test while they are performing at their maximum computation levels. It has been found that graphics intensive procedures, also requiring considerable computation, will exercise the tablet at maximum power. In general, it takes a minimum of 30 minutes for the tablet to reach a steady state temperature.  Figure 7 shows three tablets running Riptide GP during thermal testing.

<img class="alignnone size-full wp-image-208" src="http://www.mekesim.com/wp-content/uploads/2016/02/7.png" width="300" height="128" alt="Figure 7. Images of three Different Tables Running Riptide GP while Temperatures are being Monitored with Thermocouples." />
<p class="wp-caption-text">Figure 7. Images of three Different Tables Running Riptide GP while Temperatures are being Monitored with Thermocouples.</p>
Since the emissivities of the tablet surfaces are not always known, thermocouples are placed at various locations on the front and back of the tablet to read the temperatures at selected locations. The emissivity setting of the image from the IR camera is adjusted until the difference between the thermocouple readings and the IR image is minimized.

Figure 8 consists of infrared images of the back side of four different models of tablet. The tablets were running a game called Riptide GP which measures the graphics and computational capabilities of mobile devices. Ambient air temperature at the time of the test was recorded for each tablet to determine the temperature rise of the hot spot. The dark area running up the center of tablet A is from the support that was holding that tablet in the vertical position.

<img class="alignnone size-full wp-image-209" src="http://www.mekesim.com/wp-content/uploads/2016/02/8.jpg" width="300" height="214" alt="#8" />
<p class="wp-caption-text">Figure 8. Infrared Images of the Back Side of Four Different Tables Running Riptide GP</p>
Note how the location of the hot components inside “print through” the case forming a hot spot.

<strong>6. Figure of Merit for the Quality of the Thermal Solution</strong>

Since heat spreading is the most important factor in dissipating heat from the outer surface of the tablet and reducing the temperature of the hot spot, the authors propose the following figure of merit to determine the effectiveness of the thermal design of the tablet. The thermal heat spreading efficiency of the tablet can be defined as the ratio of the ideal thermal resistance of an isothermal tablet divided by the measured or simulated thermal resistance of the actual tablet. The thermal resistance of an isothermal tablet with emissivity equal to 1.0 is the very best that can be achieved on a theoretical basis. The isothermal thermal resistance is calculated by dividing the temperature rise above ambient by the dissipated tablet power for an isothermal tablet. The actual thermal resistance is calculated by dividing the temperature rise of the hot spot above ambient by the dissipated tablet power.

<strong>Heat Spreading Efficiency = R<sub>i</sub>/R<sub>a</sub></strong>

R<sub>i</sub>=∆T<sub>i</sub>/Q<sub>i</sub>   Thermal resistance of an ideal isothermal tablet

R<sub>a</sub>=∆T<sub>a</sub>/Q<sub>a</sub>   Thermal resistance of an actual tablet

Where

∆T<sub>i </sub>= Temperature rise above ambient for an ideal isothermal tablet with emissivity = 1.0

Q<sub>i</sub> = Power dissipation of the ideal isothermal tablet

∆T<sub>a</sub> = Temperature rise of the hot spot above ambient for the actual tablet

Q<sub>a</sub> = Power dissipation of the actual tablet

The following table summarizes the results of the testing for the four tablets and calculates the heat spreading efficiency of the thermal design for each tablet.

<img class="alignnone size-full wp-image-210" src="http://www.mekesim.com/wp-content/uploads/2016/02/9.png" width="660" height="274" alt="#9" />

<strong>7. Summary</strong>

In summary, building an accurate thermal model of the tablet allows the designer to rapidly test the effect of design and material changes without incurring the cost and schedule delays of testing prototypes. This speeds time to market and lowers development costs.

The maximum power dissipation of the internal components is not only governed by the size of the tablet but is a strong function of how well that heat is spread internally to reduce hot-spot temperatures. Few engineers realize the importance played by radiation in dissipating the heat from the exposed surfaces of a tablet. It is not until precise calculations are made that the importance of radiation is realized in the thermal design of the tablet. If the emissivities of the various surfaces are high, over half of the heat transfer is due to radiation.

Introduced is the <em>Heat Spreading Efficiency</em> figure of merit which measures the actual cooling efficiency of a tablet against the theoretical maximum cooling efficiency. The perfect thermal design for a tablet cooled under natural convection would have a Heat Spreading Efficiency of 1.0. However, tablet thickness and weight have to be traded off against efficiency.

<em>FloTHERM<sup>®</sup> and T3Ster<sup>®</sup> are register trademarks of Mentor Graphics Corporation.</em>

<strong>Literature</strong>
<ul>
	<li>Berhe, M.K., Ergonomic Temperature Limits for Handheld Electronic Devices, Proceedings of ASME InterPACK’07, Paper No. IPACK2007-33873</li>
	<li>Brown, L., Seshadri, H., Cool Hand Linux® – Handheld Thermal Extensions, Proceedings of the Linux Symposium, Vol. 1, pp 75 – 80, 2007</li>
	<li>Gurrum, S.P., Edwards, D.R., Marchand-Golder, T., Akiyama, J., Yokoya, S., Drouard, J.F., Dahan, F., Generic Thermal Analysis for Phone and Tablet Systems, Proceedings of IEEE Electronic Components and Technology Conference, 2012</li>
	<li>Huh, Y., Future Direction of Power Management in Mobile Devices, IEEE Asian Solid-State Circuits Conference, 2011.</li>
	<li>Lee, J., Gerlach, D.W., Joshi, Y.K., Parametric Thermal Modeling of Heat Transfer in Handheld Electronic Devices, Proceedings of the 11th IEEE Intersociety Conference on Thermal and Thermomechanical Phenomena in Electronic Systems, I-THERM, pp 604-609, 2008</li>
	<li>Mongia, R., Bhattacharya, A., Pokharna, H., Skin Cooling and Other Challenges in Future Mobile Form Factor Computing Devices, Microelectronics Journal, Vol. 39, pp 992 – 1000, 2008</li>
	<li>Wagner, G.R., Maltz, W., Thermal Management Challenges in the Passive Cooling of Handheld Devices, Proceedings of Therminic 2013, pp 135-140.</li>
	<li>Wagner, G.R., Maltz, W., On the Thermal Management Challenges in Next Generation Handheld Devices, Proceedings of the ASME InterPACK 2013, Paper No. InterPACK2013-73237</li>
</ul>