---
ID: 733
post_title: Heat Sink transfer principle
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/733
published: true
post_date: 2017-03-13 15:48:44
---
A heat sink transfers thermal energy from a higher temperature device to a lower temperature fluid medium. The fluid medium is frequently air, but can also be water, refrigerants or oil. If the fluid medium is water, the heat sink is frequently called a cold plate. In thermodynamics, a heat sink is a heat reservoir that can absorb an arbitrary amount of heat without significantly changing temperature. Practical heat sinks for electronic devices must have a temperature higher than the surroundings to transfer heat by convection, radiation, and conduction.

To understand the principle of a heat sink, consider Fourier's law of heat conduction. Joseph Fourier was a French mathematician who made important contributions to the analytical treatment of heat conduction.<sup>[2]</sup> Fourier's law of heat conduction, simplified to a one-dimensional form in the <i>x</i>-direction, shows that when there is a temperature gradient in a body, heat will be transferred from the higher temperature region to the lower temperature region. The rate at which heat is transferred by conduction, <img src="http://upload.wikimedia.org/math/5/f/b/5fbe7be0524b8ada04a29fee8d3cf17c.png" alt="q_k" />, is proportional to the product of the temperature gradient and the cross-sectional area through which heat is transferred.
<dl>
 	<dd><img class="alignnone size-full wp-image-734" src="http://en.mekesim.com/wp-content/uploads/2017/03/99a0d8ad110b9340e09c7e9dcbf0b9f6.png" alt="q_k = -k A frac{dT}{dx}" width="112" height="41" /></dd>
</dl>
<img class="alignnone size-full wp-image-735" src="http://en.mekesim.com/wp-content/uploads/2017/03/500px-Heat_sink_control_volume.png" alt="" width="500" height="272" />

Figure 2: Sketch of a heat sink in a duct used to calculate the governing equations from conservation of energy and Newton’s law of cooling.

Consider a heat sink in a duct, where air flows through the duct, as shown in Figure 2. It is assumed that the heat sink base is higher in temperature than the air. Applying the conservation of energy, for steady-state conditions, and Newton’s law of cooling to the temperature nodes shown in Figure 2 gives the following set of equations.
<dl>
 	<dd><img src="http://upload.wikimedia.org/math/e/f/4/ef41f770a4418c64dffae469bea9de1b.png" alt="dot{Q} = dot{m}c_{p,in}(T_{air,out} - T_{air,in})" /> (1)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-736" src="http://en.mekesim.com/wp-content/uploads/2017/03/ee256090bb5280bd737ac2ed149ce802.png" alt="dot{Q} = frac{T_{hs} - T_{air,av}}{R_{hs}}" width="145" height="44" /> (2)</dd>
</dl>
where
<dl>
 	<dd><img class="alignnone size-full wp-image-737" src="http://en.mekesim.com/wp-content/uploads/2017/03/4ae0c93557947a3ebf3d6a36d5fbb273.png" alt="T_{air,av} = frac{T_{air,in} + T_{air,out}}{2}" width="204" height="41" /> (3)</dd>
</dl>
Using the mean air temperature is an assumption that is valid for relatively short heat sinks. When compact heat exchangers are calculated, the logarithmic mean air temperature is used. <img src="http://upload.wikimedia.org/math/2/0/5/2056619d3cf80e2d000509b6110c57ec.png" alt="dot{m}" /> is the air mass flow rate in kg/s.

The above equations show that
<ul>
 	<li>When the air flow through the heat sink decreases, this results in an increase in the average air temperature. This, in turn, increases the heat sink base temperature. And additionally, the thermal resistance of the heat sink will also increase. The net result is a higher heat sink base temperature.
<ul>
 	<li>The increase in heat sink thermal resistance with the decrease in flow rate will be shown in later in this article.</li>
</ul>
</li>
 	<li>The inlet air temperature relates strongly with the heat sink base temperature. For example, if there is recirculation of air in a product, the inlet air temperature is not the ambient air temperature. The inlet air temperature of the heat sink is therefore higher, which also results in a higher heat sink base temperature.</li>
 	<li>If there is no air flow around the heat sink, energy cannot be transferred.</li>
 	<li>A heat sink is not a device with the "magical ability to absorb heat like a sponge and send it off to a parallel universe".<sup>[3]</sup></li>
</ul>
Natural convection requires the free flow of air over the heat sink. If fins are not aligned vertically, or if fins are too close together to allow sufficient air flow between them, the efficiency of the heat sink will decline.
<h2><span class="mw-headline">Design factors</span></h2>
<h3><span class="mw-headline">Thermal resistance</span></h3>
For semiconductor devices used in a variety of consumer and industrial electronics, the idea of <i>thermal resistance</i> simplifies the selection of heat sinks. The heat flow between the semiconductor die and ambient air is modeled as a series of resistances to heat flow; there is a resistance from the die to the device case, from the case to the heat sink, and from the heat sink to the ambient air. The sum of these resistances is the total thermal resistance from the die to the ambient air. Thermal resistance is defined as temperature rise per unit of power, analogous to electrical resistance, and is expressed in units of degrees Celsius per watt (°C/W). If the device dissipation in watts is known, and the total thermal resistance is calculated, the temperature rise of the die over the ambient air can be calculated.

The idea of thermal resistance of a semiconductor heat sink is an approximation. It does not take into account non-uniform distribution of heat over a device or heat sink. It only models a system in thermal equilibrium, and does not take into account the change in temperatures with time. Nor does it reflect the non-linearity of radiation and convection with respect to temperature rise. However, manufacturers tabulate typical values of thermal resistance for heat sinks and semiconductor devices, which allows selection of commercially manufactured heat sinks to be simplified.<sup>[4]</sup>

Commercial extruded aluminum heat sinks have a thermal resistance (heat sink to ambient air) ranging from <span class="nowrap">0.4 °C/W</span> for a large sink meant for TO3 devices, up to as high as <span class="nowrap">85 °C/W</span> for a clip-on heat sink for a TO92 small plastic case.<sup>[4]</sup> The famous, popular, historic and notable 2N3055 power transistor in a TO3 case has an internal thermal resistance from junction to case of <span class="nowrap">1.52 °C/W</span>.<sup>[5]</sup> The contact between the device case and heat sink may have a thermal resistance of between <span class="nowrap">0.5 up to 1.7 °C/W</span>, depending on the case size, and use of grease or insulating mica washer.<sup>[4]</sup>
<h3><span class="mw-headline">Material</span></h3>
The most common heat sink materials are aluminum alloys.<sup>[6]</sup> Aluminum alloy 1050A has one of the higher thermal conductivity values at 229 W/m•K <sup>[7]</sup> but is mechanically soft. Aluminum alloys 6061 and 6063 are commonly used, with thermal conductivity values of 166 and 201 W/m•K, respectively. The values depend on the temper of the alloy.

Copper has excellent heat sink properties in terms of its thermal conductivity, corrosion resistance, biofouling resistance, and antimicrobial resistance <i>(see Main Article: Copper in heat exchangers)</i>. Copper has around twice the thermal conductivity of aluminum and faster, more efficient heat absorption. Its main applications are in industrial facilities, power plants, solar thermal water systems, HVAC systems, gas water heaters, forced air heating and cooling systems, geothermal heating and cooling, and electronic systems.

Copper is three times as dense<sup>[6]</sup> and more expensive than aluminum.<sup>[6]</sup> Copper heat sinks are machined and skived. Another method of manufacture is to solder the fins into the heat sink base. Aluminum can be extruded, but copper can not.

Diamond is another heat sink material, and its thermal conductivity of 2000 W/m•K exceeds copper five-fold.<sup>[8]</sup><sup>[<i>unreliable source?</i>]</sup>In contrast to metals, where heat is conducted by delocalized electrons, lattice vibrations are responsible for diamond's very high thermal conductivity. For thermal management applications, the outstanding thermal conductivity and diffusivity of diamond is an essential. Nowadays synthetic diamond is used as submounts for high-power integrated circuits and laser diodes.

Composite materials can be used. Examples are a copper-tungsten pseudoalloy, AlSiC (silicon carbide in aluminium matrix), Dymalloy (diamond in copper-silver alloy matrix), and E-Material (beryllium oxide in beryllium matrix). Such materials are often used as substrates for chips, as their thermal expansion coefficient can be matched to ceramics and semiconductors.
<h4><span class="mw-headline">Fin efficiency</span></h4>
Fin efficiency is one of the parameters which makes a higher thermal conductivity material important. A fin of a heat sink may be considered to be a flat plate with heat flowing in one end and being dissipated into the surrounding fluid as it travels to the other.<sup>[9]</sup>As heat flows through the fin, the combination of the thermal resistance of the heat sink impeding the flow and the heat lost due to convection, the temperature of the fin and, therefore, the heat transfer to the fluid, will decrease from the base to the end of the fin. Fin efficiency is defined as the actual heat transferred by the fin, divided by the heat transfer were the fin to be isothermal (hypothetically the fin having infinite thermal conductivity). Equations 6 and 7 are applicable for straight fins.
<dl>
 	<dd><img class="alignnone size-full wp-image-738" src="http://en.mekesim.com/wp-content/uploads/2017/03/f15ad59e6188e69896d571b446f6eca5.png" alt="eta_f = frac{tanh(mL_c)}{mL_c}" width="139" height="46" /><sup>[10]</sup> (6)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-739" src="http://en.mekesim.com/wp-content/uploads/2017/03/6ba4783e423761938850a92d51a7d9e9.png" alt="mL_c = sqrt{frac{2h_f}{k t_f}}L_f" width="136" height="60" /><sup>[10]</sup> (7)</dd>
</dl>
Where:
<ul>
 	<li>h<sub>f</sub> is the convection coefficient of the fin
<ul>
 	<li>Air: 10 to 100 W/(m<sup>2</sup>K)</li>
 	<li>Water: 500 to 10,000 W/(m<sup>2</sup>K)</li>
</ul>
</li>
 	<li>k is the thermal conductivity of the fin material
<ul>
 	<li>Aluminum: 120 to 240 W/(m·K)</li>
</ul>
</li>
 	<li>L<sub>f</sub> is the fin height (m)</li>
 	<li>t<sub>f</sub> is the fin thickness (m)</li>
</ul>
Fin efficiency is increased by decreasing the fin aspect ratio (making them thicker or shorter), or by using more conductive material (copper instead of aluminum, for example).
<h4><span class="mw-headline">Spreading resistance</span></h4>
Another parameter that concerns the thermal conductivity of the heat sink material is spreading resistance. Spreading resistance occurs when thermal energy is transferred from a small area to a larger area in a substance with finite thermal conductivity. In a heat sink, this means that heat does not distribute uniformly through the heat sink base. The spreading resistance phenomenon is shown by how the heat travels from the heat source location and causes a large temperature gradient between the heat source and the edges of the heat sink. This means that some fins are at a lower temperature than if the heat source were uniform across the base of the heat sink. This nonuniformity increases the heat sink's effective thermal resistance.

To decrease the spreading resistance in the base of a heat sink:
<ul>
 	<li>Increase the base thickness</li>
 	<li>Choose a different material with better thermal conductivity</li>
 	<li>Use a vapor chamber or heat pipe in the heat sink base.</li>
</ul>
<h3><span class="mw-headline">Fin arrangements</span></h3>
<div class="rellink relarticle mainarticle">Main article: Fin (extended surface)</div>
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-741" src="http://en.mekesim.com/wp-content/uploads/2017/03/500px-Pin_fin_straight_fin_and_flared_heat_sinks.png" alt="" width="500" height="125" />
<div class="thumbcaption">
<div class="magnify">Figure 5: A pin-, straight- and flared fin heat sink types</div>
</div>
</div>
</div>
A pin fin heat sink is a heat sink that has pins that extend from its base. The pins can be cylindrical, elliptical or square. A pin is by far one of the more common heat sink types available on the market. The second type of heat sink fin arrangement is the straight fin. These run the entire length of the heat sink. A variation on the straight fin heat sink is a cross-cut heat sink. A straight fin heat sink is cut at regular intervals.

In general, the more surface area a heat sink has, the better it works.<sup>[3]</sup> However, this is not always true. The concept of a pin fin heat sink is to try to pack as much surface area into a given volume as possible.<sup>[3]</sup> As well, it works well in any orientation. Kordyban<sup>[3]</sup> has compared the performance of a pin fin and a straight fin heat sink of similar dimensions. Although the pin fin has 194 cm<sup>2</sup> surface area while the straight fin has 58 cm<sup>2</sup>, the temperature difference between the heat sink base and the ambient air for the pin fin is <span class="nowrap">50 °C</span>. For the straight fin it was 44 °C or 6 °C better than the pin fin. Pin fin heat sink performance is significantly better than straight fins when used in their intended application where the fluid flows axially along the pins (see figure 17) rather than only tangentially across the pins.

Comparison of a pin fin and straight fin heat sink of similar dimensions. Adapted from data of<sup>[3]</sup>
<table border="1" align="center">
<tbody>
<tr>
<td align="center"><b>Heat sink fin type</b></td>
<td align="center" width="50"><b>Width [cm]</b></td>
<td align="center" width="50"><b>Length [cm]</b></td>
<td align="center" width="50"><b>Height [cm]</b></td>
<td align="center" width="50"><b>Surface area [cm²]</b></td>
<td align="center" width="50"><b>Volume [cm³]</b></td>
<td align="center" width="100"><b>Temperature difference, T<sub>case</sub>−T<sub>air</sub> [°C]</b></td>
</tr>
<tr>
<td align="center">Straight</td>
<td align="center">2.5</td>
<td align="center">2.5</td>
<td align="center">3.2</td>
<td align="center">58</td>
<td align="center">20</td>
<td align="center">44</td>
</tr>
<tr>
<td align="center">Pin</td>
<td align="center">3.8</td>
<td align="center">3.8</td>
<td align="center">1.7</td>
<td align="center">194</td>
<td align="center">24</td>
<td align="center">51</td>
</tr>
</tbody>
</table>
Another configuration is the flared fin heat sink; its fins are not parallel to each other, as shown in figure 5. Flaring the fins decreases flow resistance and makes more air go through the heat sink fin channel; otherwise, more air would bypass the fins. Slanting them keeps the overall dimensions the same, but offers longer fins. Forghan, et al.<sup>[11]</sup> have published data on tests conducted on pin fin, straight fin and flared fin heat sinks. They found that for low approach air velocity, typically around 1 m/s, the thermal performance is at least 20% better than straight fin heat sinks. Lasance and Eggink<sup>[12]</sup> also found that for the bypass configurations that they tested, the flared heat sink performed better than the other heat sinks tested.
<h3><span class="mw-headline">Surface color</span></h3>
The heat transfer from the heatsink occurs by convection of the surrounding air, conduction through the air, and radiation.

Heat transfer by radiation is a function of both the heat sink temperature, and the temperature of the surroundings that the heat sink is optically coupled with. When both of these temperatures are on the order of 0 °C to 100 °C, the contribution of radiation compared to convection is generally small, and this factor is often neglected. In this case, finned heat sinks operating in either natural-convection or forced-flow will not be affected significantly by surface emissivity.

In situations where convection is low, such as a flat non-finned panel with low airflow, radiative cooling can be a significant factor. Here the surface properties may be an important design factor. Matte-black surfaces will radiate much more efficiently than shiny bare metal in the visible spectrum.<sup>[13]</sup><sup>[<i>unreliable source?</i>]</sup> A shiny metal surface has low effective emissivity due to its low surface area. While the emissivity of a material is tremendously energy (frequency) dependent, the noble metals demonstrate very low emissivity in the Near-Infrared spectrum. The emissivity in the visible spectrum is closely related to color. For most materials, the emissivity in the visible spectrum is similar to the emissivity in the infrared spectrum; however there are exceptions, notably certain metal oxides that are used as "selective surfaces".

In a vacuum or in outer space, there is no convective heat transfer, thus in these environments, radiation is the only factor governing heat flow between the heat sink and the environment. For a satellite in space, a 100 °C (373 Kelvin) surface facing the sun will absorb a lot of radiant heat, since the sun's surface temperature is nearly 6000 Kelvin, whereas the same surface facing deep-space will radiate a lot of heat, since deep-space has an effective temperature of only a few Kelvin.
<h2><span class="mw-headline">Engineering applications</span></h2>
<h3><span class="mw-headline">Microprocessor cooling</span></h3>
Heat dissipation is an unavoidable by-product of electronic devices and circuits.<sup>[9]</sup> In general, the temperature of the device or component will depend on the thermal resistance from the component to the environment, and the heat dissipated by the component. To ensure that the component temperature does not overheat, a thermal engineer seeks to find an efficient heat transfer path from the device to the environment. The heat transfer path may be from the component to a printed circuit board (PCB), to a heat sink, to air flow provided by a fan, but in all instances, eventually to the environment.

Two additional design factors also influence the thermal/mechanical performance of the thermal design:
<ol>
 	<li>The method by which the heat sink is mounted on a component or processor. This will be discussed under the section <i>attachment methods</i>.</li>
 	<li>For each interface between two objects in contact with each other, there will be a temperature drop across the interface. For such composite systems, the temperature drop across the interface may be appreciable.<sup>[10]</sup> This temperature change may be attributed to what is known as the thermal contact resistance.<sup>[10]</sup> <i>Thermal interface materials</i> (TIM) decrease the thermal contact resistance.</li>
</ol>
<h4><span class="mw-headline">Attachment methods</span></h4>
As power dissipation of components increases and component package size decreases, thermal engineers must innovate to ensure components won't overheat. Devices that run cooler last longer. A heat sink design must fulfill both its thermal as well as its mechanical requirements. Concerning the latter, the component must remain in thermal contact with its heat sink with reasonable shock and vibration. The heat sink could be the copper foil of a circuit board, or else a separate heat sink mounted onto the component or circuit board. Attachment methods include thermally conductive tape or epoxy, wire-form z clips, flat spring clips, standoff spacers, and push pins with ends that expand after installing.
<dl>
 	<dt>Thermally conductive tape</dt>
</dl>
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-742" src="http://en.mekesim.com/wp-content/uploads/2017/03/300px-Thermally_conductive_tape.png" alt="" width="300" height="243" />
<div class="thumbcaption">
<div class="magnify">Figure 6: Roll of thermally conductive tape.</div>
</div>
</div>
</div>
Thermally conductive tape is one of the most cost-effective heat sink attachment materials.<sup>[14]</sup> It is suitable for low-mass heat sinks and for components with low power dissipation. It consists of a thermally conductive carrier material with a pressure-sensitive adhesive on each side.

This tape is applied to the base of the heat sink, which is then attached to the component. Following are factors that influence the performance of thermal tape:<sup>[14]</sup>
<ol>
 	<li>Surfaces of both the component and heat sink must be clean, with no residue such as a film of silicone grease.</li>
 	<li>Preload pressure is essential to ensure good contact. Insufficient pressure results in areas of non-contact with trapped air, and results in higher-than-expected interface thermal resistance.</li>
 	<li>Thicker tapes tend to provide better "wettability" with uneven component surfaces. "Wettability" is the percentage area of contact of a tape on a component. Thicker tapes, however, have a higher thermal resistance than thinner tapes. From a design standpoint, it is best to strike a balance by selecting a tape thickness that provides maximum "wettablilty" with minimum thermal resistance.</li>
</ol>
<dl>
 	<dt>Epoxy</dt>
</dl>
Epoxy is more expensive than tape, but provides a greater mechanical bond between the heat sink and component, as well as improved thermal conductivity.<sup>[14]</sup> The epoxy chosen must be formulated for this purpose. Most epoxies are two-part liquid formulations that must be thoroughly mixed before being applied to the heat sink, and before the heat sink is placed on the component. The epoxy is then cured for a specified time, which can vary from 2 hours to 48 hours. Faster cure time can be achieved at higher temperatures. The surfaces to which the epoxy is applied must be clean and free of any residue.

The epoxy bond between the heat sink and component is semi-permanent/permanent.<sup>[14]</sup> This makes re-work very difficult and at times impossible. The most typical damage caused by rework is the separation of the component die heat spreader from its package.
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-743" src="http://en.mekesim.com/wp-content/uploads/2017/03/300px-Pin_fin_heat_sink_with_a_z-clip.png" alt="" width="300" height="236" />
<div class="thumbcaption">
<div class="magnify">Figure 7: A pin fin heat sink with a z-clip retainer.</div>
</div>
</div>
</div>
<dl>
 	<dt>Wire form Z-clips</dt>
</dl>
More expensive than tape and epoxy, wire form z-clips attach heat sinks mechanically. To use the z-clips, the printed circuit board must have anchors. Anchors can be either soldered onto the board, or pushed through. Either type requires holes to be designed into the board. The use of RoHS solder must be allowed for because such solder is mechanically weaker than traditional Pb/Sn solder.

To assemble with a z-clip, attach one side of it to one of the anchors. Deflect the spring until the other side of the clip can be placed in the other anchor. The deflection develops a spring load on the component, which maintains very good contact. In addition to the mechanical attachment that the z-clip provides, it also permits using higher-performance thermal interface materials, such as phase change types.<sup>[14]</sup>
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-744" src="http://en.mekesim.com/wp-content/uploads/2017/03/500px-MaxiGRIP_and_Talon_Clip_heat_sink_attachment_methods.png" alt="" width="500" height="175" />
<div class="thumbcaption">
<div class="magnify">Figure 8: Two heat sink attachment methods, namely the maxiGRIP (left) and Talon Clip</div>
</div>
</div>
</div>
<dl>
 	<dt>Clips</dt>
</dl>
Available for processors and ball grid array (BGA) components, clips allow the attachment of a BGA heat sink directly to the component. The clips make use of the gap created by the ball grid array (BGA) between the component underside and PCB top surface. The clips therefore require no holes in the PCB. They also allow for easy rework of components. Examples of commercially available clips are the maxiGRIP<sup>TM</sup> and superGRIP<sup>TM</sup> range from Advanced Thermal Solutions (ATS) and the Talon Clip<sup>TM</sup> from Malico. The three aforementioned clipping methods use plastic frames for the clips, but the ATS designs uses metal spring clips to provide the compression force. The Malico design uses the plastic "arm" to provide a mechanical load on the component. Depending on the product requirement, the clipping methods will have to meet shock and vibration standards, such as Telecordia GR-63-CORE, ETSI 300 019 and MIL-STD-810.
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-745" src="http://en.mekesim.com/wp-content/uploads/2017/03/300px-Pushpins.png" alt="" width="300" height="228" />
<div class="thumbcaption">
<div class="magnify">Figure 9: Push pins.</div>
</div>
</div>
</div>
<dl>
 	<dt>Push pins with compression springs</dt>
</dl>
For larger heat sinks and higher preloads, push pins with compression springs are very effective.<sup>[14]</sup> The push pins, typically made of brass or plastic, have a flexible barb at the end that engages with a hole in the PCB; once installed, the barb retains the pin. The compression spring holds the assembly together and maintains contact between the heat sink and component. Care is needed in selection of push pin size. Too great an insertion force can result in the die cracking and consequent component failure.
<dl>
 	<dt>Threaded standoffs with compression springs</dt>
</dl>
For very large heat sinks, there is no substitute for the threaded standoff and compression spring attachment method.<sup>[14]</sup> A threaded standoff is essentially a hollow metal tube with internal threads. One end is secured with a screw through a hole in the PCB. The other end accepts a screw which compresses the spring, completing the assembly. A typical heat sink assembly uses two to four standoffs, which tends to make this the most costly heat sink attachment design. Another disadvantage is the need for holes in the PCB.

Summary of heat sink attachment methods
<sup>[14]</sup>
<table border="1" align="center">
<tbody>
<tr>
<td align="center"><b>Method</b></td>
<td align="center"><b>Pros</b></td>
<td align="center"><b>Cons</b></td>
<td align="center"><b>Cost</b></td>
</tr>
<tr>
<td>Thermal tape</td>
<td>Easy to attach. Inexpensive.</td>
<td>Cannot provide mechanical attachment for heavier heat sinks or for high vibration environments. Surface must be cleaned for optimal adhesion. Moderate to low thermal conductivity.</td>
<td>Very low</td>
</tr>
<tr>
<td>Epoxy</td>
<td>Strong mechanical adhesion. Relatively inexpensive.</td>
<td>Makes board rework difficult since it can damage component. Surface must be cleaned for optimal adhesion.</td>
<td>Very low</td>
</tr>
<tr>
<td>Wire form Z-clips</td>
<td>Strong mechanical attachment. Easy removal/rework. Applies a preload to the thermal interface material, improving thermal performance.</td>
<td>Requires holes in the board or solder anchors. More expensive than tape or epoxy. Custom designs.</td>
<td>Low</td>
</tr>
<tr>
<td>Clip-on</td>
<td>Applies a preload to the thermal interface material, improving thermal performance. Requires no holes or anchors. Easy removal/rework.</td>
<td>Must have "keep out" zone around the BGA for the clip. Extra assembly steps.</td>
<td>Low</td>
</tr>
<tr>
<td>Push pin with compression springs</td>
<td>Strong mechanical attachment. Highest thermal interface material preload. Easy removal and installation.</td>
<td>Requires holes in the board which increases complexity of traces in PCB.</td>
<td>Moderate</td>
</tr>
<tr>
<td>Stand-offs with compression springs</td>
<td>Strongest mechanical attachment. Highest preload for the thermal interface material. Ideal for large heat sinks.</td>
<td>Requires holes in the board which increases complexity of trace layout. Complicated assembly.</td>
<td>High</td>
</tr>
</tbody>
</table>
<h4><span class="mw-headline">Thermal interface materials</span><span class="mw-editsection"><span class="mw-editsection-bracket">[</span>edit<span class="mw-editsection-bracket">]</span></span></h4>
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-746" src="http://en.mekesim.com/wp-content/uploads/2017/03/400px-Difference_between_thermal_conductivity_of_thermal_interface_materials_and_thermal_contact_resistance.png" alt="" width="400" height="203" />
<div class="thumbcaption">
<div class="magnify">Figure 10: Thermal conductivity and the interface resistance form part of the thermal interface resistance of a thermal interface material.</div>
</div>
</div>
</div>
Thermal contact resistance occurs due to the voids created by surface roughness effects, defects and misalignment of the interface. The voids present in the interface are filled with air. Heat transfer is therefore due to conduction across the actual contact area and to conduction (or natural convection) and radiation across the gaps.<sup>[10]</sup> If the contact area is small, as it is for rough surfaces, the major contribution to the resistance is made by the gaps.<sup>[10]</sup> To decrease the thermal contact resistance, the surface roughness can be decreased while the interface pressure is increased. However, these improving methods are not always practical or possible for electronic equipment. Thermal interface materials (TIM) are a common way to overcome these limitations,

Properly applied thermal interface materials displace the air that is present in the gaps between the two objects with a material that has a much-higher thermal conductivity. Air has a thermal conductivity of 0.022 W/m•K<sup>[15]</sup> while TIMs have conductivities of 0.3 W/m•K<sup>[16]</sup> and higher.

When selecting a TIM, care must be taken with the values supplied by the manufacturer. Most manufacturers give a value for the thermal conductivity of a material. However, the thermal conductivity does not take into account the interface resistances. Therefore, if a TIM has a high thermal conductivity, it does not necessarily mean that the interface resistance will be low.

Selection of a TIM is based on three parameters: the interface gap which the TIM must fill, the contact pressure, and the electrical resistivity of the TIM. The contact pressure is the pressure applied to the interface between the two materials. The selection does not include the cost of the material. Electrical resistivity may, or may not, be important, depending upon electrical design details.

Selection Based on Interface Gap
<sup>[16]</sup>
<table border="1" align="center">
<tbody>
<tr>
<td colspan="2" align="center"><b>Interface gap values</b></td>
<td align="center"><b>Products types available</b></td>
</tr>
<tr>
<td align="right">&lt; 0.05 mm</td>
<td align="right">&lt; 2 mil</td>
<td>Thermal grease, epoxy, phase change materials</td>
</tr>
<tr>
<td align="right">0.05 – 0.1 mm</td>
<td align="right">2 – 5 mil</td>
<td>Phase change materials, polyimide, graphite or aluminium tapes</td>
</tr>
<tr>
<td align="right">0.1 - 0,5 mm</td>
<td align="right">5 – 18 mil</td>
<td>Silicone-coated fabrics</td>
</tr>
<tr>
<td align="right">&gt; 0.5 mm</td>
<td align="right">&gt; 18 mil</td>
<td>Gap fillers</td>
</tr>
</tbody>
</table>
Selection Based on Contact Pressure
<sup>[16]</sup>
<table border="1" align="center">
<tbody>
<tr>
<td align="center"><b>Contact pressure scale</b></td>
<td align="center"><b>Typical pressure ranges</b></td>
<td align="center"><b>Product types available</b></td>
</tr>
<tr>
<td>Very low</td>
<td>&lt; 70 kPa</td>
<td>Gap fillers</td>
</tr>
<tr>
<td>Low</td>
<td>&lt; 140 kPa</td>
<td>Thermal grease, epoxy, polyimide, graphite or aluminium tapes</td>
</tr>
<tr>
<td>High</td>
<td>2 MPa</td>
<td>Silicone-coated fabrics</td>
</tr>
</tbody>
</table>
Selection Based on Dielectric Strength
<sup>[16]</sup>
<table border="1" align="center">
<tbody>
<tr>
<td align="center"><b>Electrical insulation</b></td>
<td align="center"><b>Dielectric strength</b></td>
<td colspan="2" align="center"><b>Typical values</b></td>
<td align="center"><b>Product types available</b></td>
</tr>
<tr>
<td>Not required</td>
<td>N/A</td>
<td align="right">N/A</td>
<td align="right">N/A</td>
<td>Thermal grease, epoxy, phase change materials, graphite or aluminium tapes.</td>
</tr>
<tr>
<td>Required</td>
<td>Low</td>
<td align="right"><span class="nowrap">10 kV/mm</span></td>
<td align="right"><span class="nowrap">&lt; 300 V/mil</span></td>
<td>Silicone coated fabrics, gap fillers</td>
</tr>
<tr>
<td>Required</td>
<td>High</td>
<td align="right"><span class="nowrap">60 kV/mm</span></td>
<td align="right"><span class="nowrap">&gt; 1500 V/mil</span></td>
<td>Polyimide tape</td>
</tr>
</tbody>
</table>
TIM Application Notes Based on Product Type
<table border="1" align="center">
<tbody>
<tr>
<td align="center"><b>Product type</b></td>
<td align="center"><b>Application notes</b></td>
<td align="center"><b>Thermal performance</b></td>
</tr>
<tr>
<td>Thermal paste</td>
<td>Messy. Labor intensive. Relatively long assembly time.</td>
<td>++++</td>
</tr>
<tr>
<td>Epoxy</td>
<td>Creates "permanent" interface bond.</td>
<td>++++</td>
</tr>
<tr>
<td>Phase change</td>
<td>Allows for pre-attachment. Softens and conforms to interface defects at operational temperatures. Can be repositioned in field.</td>
<td>++++</td>
</tr>
<tr>
<td>Thermal tapes, including graphite, polyimide, and aluminium tapes</td>
<td>Easy to apply. Some mechanical strength.</td>
<td>+++</td>
</tr>
<tr>
<td>Silicone coated fabrics</td>
<td>Provide cushioning and sealing while still allowing heat transfer.</td>
<td>+</td>
</tr>
<tr>
<td>Gap filler</td>
<td>Can be used to thermally couple differing-height components to a heat spreader or heat sink. Naturally tacky.</td>
<td>++</td>
</tr>
</tbody>
</table>
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-747" src="http://en.mekesim.com/wp-content/uploads/2017/03/220px-2007-07-24_High-power_light_emiting_diodes_Luxeon_Lumiled.jpg" alt="" width="220" height="165" />
<div class="thumbcaption">
<div class="magnify">Figure 11: High power LEDs from Philips Lumileds Lighting Company mounted on 21 mm star shaped aluminium-core PCBs</div>
</div>
</div>
</div>
<h3><span class="mw-headline">Light-emitting diode lamps</span></h3>
Light-emitting diode (LED) performance and lifetime are strong functions of their temperature.<sup>[17]</sup> Effective cooling is therefore essential. A case study of a LED based downlighter shows an example of the calculations done in order to calculate the required heat sink necessary for the effective cooling of lighting system.<sup>[18]</sup> The article also shows that in order to get confidence in the results, multiple independent solutions are required that give similar results. Specifically, results of the experimental, numerical and theoretical methods should all be within 10% of each other to give high confidence in the results.
<h3><span class="mw-headline">In soldering</span></h3>
Temporary heat sinks were sometimes used while soldering circuit boards, preventing excessive heat from damaging sensitive nearby electronics. In the simplest case, this means partially gripping a component using a heavy metal crocodile clip, hemostat or similar clamp. Modern semiconductor devices, which are designed to be assembled by reflow soldering, can usually tolerate soldering temperatures without damage. On the other hand, electrical components such as magnetic reed switches can malfunction if exposed to hotter soldering irons, so this practice is still very much in use.<sup>[19]</sup>
<h2><span class="mw-headline">Methods to determine performance</span></h2>
In general, a heat sink performance is a function of material thermal conductivity, dimensions, fin type, heat transfer coefficient, air flow rate, and duct size. To determine the thermal performance of a heat sink, a theoretical model can be made. Alternatively, the thermal performance can be measured experimentally. Due to the complex nature of the highly 3D flow in present in applications, numerical methods or computational fluid dynamics (CFD) can also be used. This section will discuss the aforementioned methods for the determination of the heat sink thermal performance.
<h3><span class="mw-headline">A heat transfer theoretical model</span><span class="mw-editsection"><span class="mw-editsection-bracket">[</span>edit<span class="mw-editsection-bracket">]</span></span></h3>
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-748" src="http://en.mekesim.com/wp-content/uploads/2017/03/500px-Heat_sink_thermal_resistances.png" alt="" width="500" height="519" />
<div class="thumbcaption">
<div class="magnify">Figure 13: Sketch of a heat sink with equivalent thermal resistances.</div>
</div>
</div>
</div>
<div class="thumb tright">
<div class="thumbinner">

<img class="alignnone size-full wp-image-749" src="http://en.mekesim.com/wp-content/uploads/2017/03/300px-Thermal_resistance_and_heat_transfer_coefficient_plotted_against_flow_rate_for_specific_heat_sink_design.png" alt="" width="300" height="205" />
<div class="thumbcaption">
<div class="magnify">Figure 14: Thermal resistance and heat transfer coefficient plotted against flow rate for the specific heat sink design used in.<sup>[20]</sup>The data was generated using the equations provided in the article. The data shows that for an increasing air flow rate, the thermal resistance of the heat sink decreases.</div>
</div>
</div>
</div>
One of the methods to determine the performance of a heat sink is to use heat transfer and fluid dynamics theory. One such method has been published by Jeggels, et al.,<sup>[20]</sup> though this work is limited to ducted flow. Ducted flow is where the air is forced to flow through a channel which fits tightly over the heat sink. This makes sure that all the air goes through the channels formed by the fins of the heat sink. When the air flow is not ducted, a certain percentage of air flow will bypass the heat sink. Flow bypass was found to increase with increasing fin density and clearance, while remaining relatively insensitive to inlet duct velocity.<sup>[21]</sup>

The heat sink thermal resistance model consists of two resistances, namely the resistance in the heat sink base, <img src="http://upload.wikimedia.org/math/0/1/9/0192ff26b1834264029b67ae77d9e1c2.png" alt="R_{b}" />, and the resistance in the fins, <img src="http://upload.wikimedia.org/math/0/0/f/00f5dde98850ed1019e10a8019173da2.png" alt="R_{f}" />. The heat sink base thermal resistance, <img src="http://upload.wikimedia.org/math/0/1/9/0192ff26b1834264029b67ae77d9e1c2.png" alt="R_{b}" />, can be written as follows if the source is a uniformly applied the heat sink base. If it is not, then the base resistance is primarily spreading resistance:
<dl>
 	<dd><img class="alignnone size-full wp-image-750" src="http://en.mekesim.com/wp-content/uploads/2017/03/6f9f3f34c45335982f764605e863ffb1.png" alt="R_b = frac{t_b}{kA_b}" width="83" height="43" /> (4)</dd>
</dl>
where <img src="http://upload.wikimedia.org/math/4/d/9/4d9ecb3216b52cc64e016e583ca1a3b2.png" alt="t_b" /> is the heat sink base thickness, <img src="http://upload.wikimedia.org/math/8/c/e/8ce4b16b22b58894aa86c421e8759df3.png" alt="k" /> is the heat sink material thermal conductivity and <img src="http://upload.wikimedia.org/math/6/7/2/672200b585b9a8f4288d2539ba22c762.png" alt="A_b" /> is the area of the heat sink base.

The thermal resistance from the base of the fins to the air, <img src="http://upload.wikimedia.org/math/0/0/f/00f5dde98850ed1019e10a8019173da2.png" alt="R_{f}" />, can be calculated by the following formulas.
<dl>
 	<dd><img class="alignnone size-full wp-image-751" src="http://en.mekesim.com/wp-content/uploads/2017/03/b432a68fbecb86769d843ebba7eb5755.png" alt="R_f = frac{1}{n h_f W_f left ( t_f + 2eta_f L_f right)}" width="221" height="47" /> (5)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-752" src="http://en.mekesim.com/wp-content/uploads/2017/03/aa333f1fdfe8546bc8423cb37bf1461e.png" alt="eta_f = frac{tanh{mL_c}}{mL_c}" width="127" height="44" /><sup>[10]</sup> (6)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-739" src="http://en.mekesim.com/wp-content/uploads/2017/03/6ba4783e423761938850a92d51a7d9e9.png" alt="mL_c = sqrt{frac{2h_f}{k t_f}}L_f" width="136" height="60" /><sup>[10]</sup> (7)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-754" src="http://en.mekesim.com/wp-content/uploads/2017/03/70be775fba0df2fe54bef39163a03687.png" alt="D_h = frac{4A_{ch}}{P_{ch}}" width="94" height="44" /> (8)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-755" src="http://en.mekesim.com/wp-content/uploads/2017/03/c363cb19139af019ae0e803b53b7ac2e.png" alt="Re = frac{4 dot{G} rho}{n pi D_h mu}" width="114" height="51" /> (9)</dd>
</dl>
<dl>
 	<dd><img src="http://upload.wikimedia.org/math/1/2/8/12899b6d885703cbc36d73e18f6eb170.png" alt="f = (0.79 ln Re - 1.64)^{-2}" /><sup>[22]</sup> (10)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-756" src="http://en.mekesim.com/wp-content/uploads/2017/03/655d4721a76d3cbc83e7f37101eb3635.png" alt="Nu = frac{(f/8)(Re - 1000)Pr}{1+12.7(f/8)^{0.5}(Pr^{frac{2}{3}}-1)}" width="276" height="51" /><sup>[22]</sup> (11)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-757" src="http://en.mekesim.com/wp-content/uploads/2017/03/b25ca5410d25813841281c9ce828bc8a.png" alt="h_f = frac{Nu k_{air}}{D_h}" width="106" height="44" /> (12)</dd>
</dl>
<dl>
 	<dd><img class="alignnone size-full wp-image-758" src="http://en.mekesim.com/wp-content/uploads/2017/03/b375124c145bf610a0554286f955e20b.png" alt="rho = frac{P_{atm}}{R_aT_{in}}" width="87" height="44" /> (13)</dd>
</dl>
The flow rate can be determined by the intersection of the heat sink system curve and the fan curve. The heat sink system curve can be calculated by the flow resistance of the channels and inlet and outlet losses as done in standard fluid mechanics text books, such as Potter, et al.<sup>[23]</sup> and White.<sup>[24]</sup>

Once the heat sink base and fin resistances are known, then the heat sink thermal resistance, <img src="http://upload.wikimedia.org/math/5/8/1/581ad40c37184b8c075eeb3e035b8b78.png" alt="R_{hs}" /> can be calculated as: <img src="http://upload.wikimedia.org/math/7/5/7/757af68e88d768996ee04b53b12147a2.png" alt="R_{hs}=R_{b} + R_{f}" /> (14)

Using the equations 5 to 13 and the dimensional data in,<sup>[20]</sup> the thermal resistance for the fins was calculated for various air flow rates. The data for the thermal resistance and heat transfer coefficient are shown in Figure 14. It shows that for an increasing air flow rate, the thermal resistance of the heat sink decreases.