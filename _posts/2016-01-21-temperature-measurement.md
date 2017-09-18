---
ID: 79
post_title: Temperature measurement
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/79
published: true
post_date: 2016-01-21 07:58:54
---
<h2>Temperature and temperature scales</h2>
Temperature is a measure of how cold or hot something is, expressed in several different scales, such as Celsius, Kelvin or Fahrenheit.

We know three types of temperature scales:
<ol>
	<li>Celsius or centigrade scale which is the most often used scale. For this scale, the freezing point of water is considered to be zero degrees, the boiling point is 100 degrees, and each degree in between is an equal 1/100th of the distance between freezing and boiling.</li>
	<li>Fahrenheit scale is still widely used in the United States. On the Fahrenheit scale, freezing is 32 degrees and boiling is 212 degrees (180 degrees difference).</li>
	<li>Kelvin scale was created to be more scientific. It is the base unit of thermodynamic temperature measurement in the International System (SI) of measurement. It is defined as 1/ 273.16 of the triple point (equilibrium among the solid, liquid, and gaseous phases).</li>
</ol>
Graphical comparison of scales:

<img src="http://www.dewesoft.com/assets/img/pro/uploads/pro_training_farenheit_celsius_scale.svg" alt="" />

<img src="http://www.dewesoft.com/assets/img/pro/uploads/pro_training_celsius_kelvin_scale.svg" alt="" />

Conversion of temperature

<img class="alignnone size-full wp-image-80" src="http://en.mekesim.com/wp-content/uploads/2016/01/equation_temperature_conversion.png" alt="" width="225" height="201" />
<h2 id="panel_33" class="panel panel-default"> Types of temperature sensors</h2>
<h3>1. Thermocouples</h3>
Thermocouples are cheap, interchangeable, have standard connectors and can measure a wide range of temperatures. The main limitation is accuracy. System errors of less than 1°C can be difficult to achieve.

A thermocouple is created when two dissimilar metals touch and the contact point produces a small open-circuit voltage as a function of temperature.

You can choose between different types of thermocouples named by capital letters that show their compositions according to American National Standards Institute conventions. The most common types of thermocouples include B, E, K, N, R, S, and T.

<img class="alignnone size-full wp-image-81" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_temperature_measurement_thermocouple.jpg" alt="" />
<table class="table table-striped table-bordered">
<tbody>
<tr>
<td><strong>ADVANTAGES</strong></td>
<td><strong>DISADVANTAGES</strong></td>
</tr>
<tr>
<td>
<ul>
	<li>Self Powered</li>
	<li>Simple</li>
	<li>Rugged</li>
	<li>Inexpensive</li>
	<li>Wide Variety</li>
	<li>Wide Temp Range</li>
</ul>
</td>
<td>
<ul>
	<li>Non Linear</li>
	<li>Reference Required</li>
	<li>Low Voltage</li>
	<li>Least Stable</li>
	<li>Least Sensitive</li>
</ul>
</td>
</tr>
</tbody>
</table>
<table class="table table-striped table-bordered">
<tbody>
<tr>
<td><img class="alignnone size-full wp-image-82" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_linearisation_curves.png" alt="" /></td>
</tr>
</tbody>
</table>
<h3>2. RTDs</h3>
An RTD is a device made of coils or films of metal (usually platinum). When the RTD is heated, the resistance of the metal increases; when it gets cooled, the resistance decreases. Passing current through an RTD generates a voltage across the RTD. By measuring this voltage, you can determine its resistance and that's how its temperature. The relationship between resistance and temperature is relatively linear. Typically, RTDs have a resistance of 100 Ω at 0 °C and can measure temperatures up to 850 °C.

<img class="alignnone size-full wp-image-83" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_temperature_measurement_rtd.jpg" alt="" />
<table class="table table-striped table-bordered">
<tbody>
<tr>
<td><strong>ADVANTAGES</strong></td>
<td><strong>DISADVANTAGES</strong></td>
</tr>
<tr>
<td>
<ul>
	<li>Most Stable</li>
	<li>Most Accurate</li>
	<li>More Linear than Thermocouple</li>
</ul>
</td>
<td>
<ul>
	<li>Expensive</li>
	<li>Current Source Required</li>
	<li>Small ∆R</li>
	<li>Low absolute Resistance</li>
	<li>Self heating</li>
</ul>
</td>
</tr>
</tbody>
</table>
<table class="table table-striped table-bordered">
<tbody>
<tr>
<td><img class="alignnone size-full wp-image-84" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_pt_rtd_response_curves.png" alt="" /></td>
</tr>
</tbody>
</table>
<h3>3. Thermistors</h3>
NOTE: Thermistors are mostly used in electronics circuits and have little practical use when it comes to measuring with DEWESoft. Thus, we shall only give a small overview of them here and omit them from further discussion.

A thermistor is a piece of semiconductor made of metal oxides that are pressed into a small bead, disk, wafer, or other shape and sintered at high temperatures. Lastly, they are coated with epoxy or glass. As with RTDs, you can pass a current through a thermistor to read the voltage across the thermistor and determine its temperature. However, unlike RTDs, thermistors have a higher resistance (2,000 to 10,000 Ω) and a much higher sensitivity (~200 Ω/°C), allowing them to achieve higher sensitivity within a limited temperature range (up to 300 °)

<img class="alignnone size-full wp-image-85" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_temperature_measurement_thermistor.jpg" alt="" />
<table class="table table-striped table-bordered">
<tbody>
<tr>
<td><strong>ADVANTAGES</strong></td>
<td><strong>DISADVANTAGES</strong></td>
</tr>
<tr>
<td>
<ul>
	<li>High Output</li>
	<li>Fast</li>
	<li>Two wire ohms measurement.</li>
</ul>
</td>
<td>
<ul>
	<li>Non Linear</li>
	<li>Limited Temperature Range.</li>
	<li>Fragile</li>
	<li>Current Source required.</li>
	<li>Self heating</li>
</ul>
</td>
</tr>
</tbody>
</table>
<img class="alignnone size-full wp-image-86" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_thermistor_curve.png" alt="" />
<h2 class="panel-title">How do thermocouples work</h2>
As we already mentioned, thermocouples are the most often used temperature sensors.

Thermocouple is made of at least two metals that are joined together to form two junctions. One is connected to a body whose temperature will be measured; this is the hot or measuring junction. The other junction is connected to a body of known temperature; this is the cold or reference junction. Therefore the thermocouple measures the unknown temperature of the body with reference to the known temperature of the other body, which is in line with the Zeroth law of thermodynamics which states that :“When two bodies are separately in thermal balance with the third body, then the two are also in thermal balance with each other". Because of this, we need to know the temperature at the cold junction if we wish to have an absolute temperature reading. This is done by a technique known as cold junction compensation (CJC).

Typically CJC temperature is sensed by a precision RTD sensor in good thermal contact with the input connectors of the measuring instrument. This second temperature reading, along with the reading from the thermocouple itself is used by the measuring instrument to calculate the true temperature at the thermocouple tip. By combining the signal from this semiconductor with the signal from the thermocouple, the correct reading can be obtained without the need or expense to record two temperatures.

Understanding cold junction compensation is important, since any error in the measurement of the cold junction temperature will lead to the same error in the measured temperature from the thermocouple tip. As well as dealing with the CJC, the measuring instrument must also compensate for the fact that the thermocouple output is non-linear. The relationship between temperature and output voltage is a complex polynomial equation (5th to 9th order depending on thermocouple type). High accuracy instruments such as DEWESoft instruments store thermocouple tables in devices and compensate the results to eliminate this source of error.

Working principle of Thermocouples

Now let's take a look at working principle of every Thermocouple. The working principle is based on the Seebeck, Peltier or Thomson effect.

1. Seebeck effect prescribes that a circuit made from two dissimilar metal, with junctions at different temperature, induces a voltage difference between the junctions.

<img src="http://www.dewesoft.com/assets/img/pro/uploads/pro_training_seebeck_effect_1.svg" alt="" />

2. Peltier effect is the opposite of the Seebeck effect. Instead of using heat to induce a voltage difference, it uses a voltage difference to induce heat.

<img src="http://www.dewesoft.com/assets/img/pro/uploads/pro_training_peltuier_effect.svg" alt="" />

3. Thomson effect states that if an electrical current flows along a single conductor while a temperature difference exist in the conductor, thermal energy is either absorbed or rejected by the conductor, depending on he flow of the current. More specifically heat is liberated if an electric current flows in the same direction as the heat flows; otherwise it is absorbed.

<img src="http://www.dewesoft.com/assets/img/pro/uploads/pro_training_thomson_effect.svg" alt="" />

The circuit of every Thermocouple must be composed of two dissimilar metals, for example, A and B. These two metals are joined together to form two junctions, p, and q, which are maintained at the temperatures T1 and T2 respectively. Let us not forget, that thermocouple cannot be formed if there is just one junction. If the temperature of both the junctions is the same, equal and opposite electromotive force will be generated at both junctions and the net current flowing through the junction is zero. If the junctions are maintained at different temperatures, the electromotive force will not become zero and there will be a net current flowing through the circuit. The total electromotive force flowing through this circuit depends on the metals used in the circuit as well as the temperature of the two junctions. An ammeter is connected in the circuit of the thermocouple. It measures the amount of electromotive force flowing through the circuit due to the two junctions of the two dissimilar metals maintained at different temperatures.
<h2 class="panel-title">Different thermocouple types</h2>
Thermocouples can be made from almost any type of metal, but there are many standard types used because their output voltages and large temperature gradients can be predicted. Each calibration has a different temperature range and the environment, although the maximum temperature varies with the diameter of the wire used in the thermocouple. Although the thermocouple calibration dictates the temperature range, the maximum range is also limited by the diameter of the thermocouple wire. That is, a very thin thermocouple may not reach the full temperature range. The four most common calibrations of Thermocouples are J, K, T and E. There are high-temperature calibrations like R, S, C and GB. If you want to choose the right Thermocouple for your measurement, you need to look at a number of different factors, like what are the maximum and minimum temperatures that the thermocouple will detect, what are the cost limits, what error tolerances are acceptable for certain application, what is the furnace atmosphere, what is the expected life of certain thermocouple type, what is the required time response, will the use of the thermocouple be periodical or continuous, will the thermocouple be exposed to bending or flexing during it's life and what is the immersion depth.

Characteristics of different thermocouples:

<img class="alignnone size-full wp-image-87" src="http://en.mekesim.com/wp-content/uploads/2016/01/different_thermocouples_characteristics.png" alt="" />

Types of thermocouple fabrications
<h3>1. Beaded Wire Thermocouple</h3>
<img class="alignnone size-full wp-image-88" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_temperature_measurement_beaded_wire.jpg" alt="" />

This type of Thermocouples is the simplest from all of the thermocouples. It is made of two pieces of thermocouple wire joined together.

Because of this bead, this type of thermocouples has a lot of limitations. Beaded wire thermocouple mustn't be used with liquids that could corrode or oxidize the thermocouple alloy.

In general, beaded wire thermocouples are the great choice if we measure gas temperature. Since they can be made very small, they also provide very fast response time.

We can actually build these thermocouple types ourselves by buying a thermocouple wire and joining the hot point together. Please note that soldering is not a good option since it adds a third material which will increase inaccuracy. The bigger the junction is, the slower the response of the thermocouple.

Note: This thermocouple type is not electrically isolated, so it is advisable to use isolated amplifiers (such as DEWESoft KRYPTON).
<h3>2. Thermocouple Probe</h3>
<img class="alignnone size-full wp-image-89" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_temperature_measurement_thermocouple_probe.jpg" alt="" />

A thermocouple probe is made of a thermocouple wire that is housed inside a metal tube, which is made of stainless steel or Inconel.

Inconel supports higher temperature ranges than stainless steel, however, stainless steel is often preferred because of its broad chemical compatibility.

The tip of the thermocouple probe can be made in three different styles. Grounded, ungrounded and exposed.

With a grounded tip, the thermocouple is in contact with the sheath wall. A grounded junction provides a fast response time, but it is the most susceptible to electrical ground loops.

In ungrounded junctions, the thermocouple is separated from the sheath wall by a layer of insulation. Response time is slower than the grounded style, but it offers electrical isolation

Exposed junction types have the tip of the thermocouple outside the sheath wall with an exposed junction. They offer the best response time but are limited in use to dry, noncorrosive and non-pressurized applications.

<img class="alignnone size-full wp-image-90" src="http://en.mekesim.com/wp-content/uploads/2016/01/thermocouple_tip_styles.png" alt="" />
<h3>3. Surface Probe</h3>
<img class="alignnone size-full wp-image-91" src="http://en.mekesim.com/wp-content/uploads/2016/01/dewesoft_x_temperature_measurement_surface_probe.jpg" alt="" width="640" height="480" />

These type of thermocouples are great for any surface measurements. Because the thermocouple can be fitted with a rotating mechanism, so we can measure the temperature of a moving surface.