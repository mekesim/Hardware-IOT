---
ID: 295
post_title: >
  Thermal Analysis of a Low Noise
  Amplifier
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/295
published: true
post_date: 2016-03-16 10:35:58
---
LNA Design Series - part 13

From RF Design HQ

It is time to make sure that all transistors are going to operate reliably at maximum temperatures.  For this analysis you can use Avago's <a href="http://www.avagotech.com/pages/appcad" target="_blank" rel="nofollow">AppCAD Design Assistant</a>.  We used this tool <a href="http://www.rfdesignhq.com/2013/03/low-noise-amplifier-design-tutorial.html" target="_blank">early in this series</a> to plot some gain, Noise Figure and circuit stability circles.  This time we will showcase its Device Thermal Calculator tool.

To remain informed about this project I encourage you to sign up to <a href="http://eepurl.com/wMpsv">my mailing list</a>.
<h2>1. Thermal Analysis of the ATF-34143</h2>
<img class="alignnone size-full wp-image-296" title="Thermal Analysis of the ATF-34143" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-03_07_2013-12_03_20-AM.png" alt="Thermal Analysis of the ATF-34143" width="640" height="457" />
<h3>Operating Temperature</h3>
In the previous Thermal Analysis screenshot I've plugged in the numbers for the Bias Voltage (Vin), Bias Current (Iin), Input Power (Pin), Output Power (Pout), PCB Thermal Resistance (Θca), Junction or Channel Resistance (Θjc), and Ambient Temperature (Ta).

<img class="alignnone size-full wp-image-297" title="Device Max Temperature Warning" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-02_07_2013-11_36_17-PM.png" alt="Device Max Temperature Warning" width="482" height="341" />

Figure: Device Max Temperature Warning

Hidden deep in the preferences menu is an option to enter a Device Maximum Temperature Warning.  For the ATF-34143 it is 160°C as entered.  In reality we should enter a much lower number depending on the reliability targets of the design.  For reference, below is an excerpt from the <a href="https://docs.google.com/file/d/0B6ji9f7ejcKyb09zekd6Z2M3bzg/edit?usp=sharing" target="_blank">AD-A153 744 "Reliability Derating Procedures"</a> specific to GaAs for example.

<img class="alignnone size-full wp-image-298" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-03_07_2013-12_12_35-AM.png" alt="" width="568" height="357" />

Figure: GaAs Fet Device Derating Levels

<img class="alignnone size-full wp-image-299" title="ATF-34143 Absolute Maximum Ratings" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-02_07_2013-11_18_16-PM.png" alt="ATF-34143 Absolute Maximum Ratings" width="640" height="228" />

Figure: ATF-34143 Absolute Maximum Ratings

So far everything looks to be well within the maximum operating conditions in regards to Channel Temperature with a Channel Temperature of 87°C vs. a maximum of 160°C.
<h3>Total Power Dissipation</h3>
If you read Note 4 in the Absolute Ratings listed above we should take into account a reduction in Power Dissipation capability due to the Source leads at temperatures above 40°C. To be safe, we will use the Case Temperature (Tcase) of 72°C that was calculated with the Device Thermal Calculator.  This results in a 192mW((72-40)/6=192) degradation in Total Power Dissipation capabilities of the ATF-34143.  This results in a Total Power Dissipation maximum of 533mW.  Our previous analysis calculated this value to be a worst case of 89mW at an ambient temperature of 70°C.  This means the device will be operating safely below it's absolute maximum temperatures.
<h2>2. MGA-53543 Operating Temperature and Power Dissipation</h2>
Listed below are the Maximum Ratings we need to perform the analysis for the MGA-53543.

<img class="alignnone size-full wp-image-300" title="MGA-53543 Absolute Maximum Ratings" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-03_07_2013-12_36_44-AM.png" alt="MGA-53543 Absolute Maximum Ratings" width="640" height="186" />

Figure: MGA-53543 Absolute Maximum Ratings
<h3>Lead Temperature of the MGA-53543</h3>
When we consider Device Lead Temperature as specified in note 2 of the Absolute Maximum Ratings sections of the data sheet.  We only need to derate the Power Dissipation capability if we exceed a lead temperature of 96°C.  The analysis presented below shows that the case temperature will not exceed 77°C making the derating of the Power Dissipation unnecessary.

<img class="alignnone size-full wp-image-301" title="Thermal Analysis of the MGA-53543" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-03_07_2013-12_42_50-AM.png" alt="Thermal Analysis of the MGA-53543" width="640" height="457" />
<div>

Thermal Analysis of the MGA-53543
<h3>Thermal Results for the MGA-53543</h3>
<ul>
	<li>The Maximum Junction Temperature remains below 150°C at 130°C.</li>
	<li>The Total Power Dissipated at heat is 335mW with a maximum allowed of 400mW.</li>
</ul>
<h2>3. ATF-50189 Operating Temperature and Power Dissipation</h2>
If you remember in <a href="http://www.rfdesignhq.com/2013/06/atf-50189-high-linearity-balanced.html" target="_blank">Part-11</a> during the board layout of the ATF-50189, we went through great lengths to ensure good placement of large headed screws.  This was to achieve a strong contact to the case for improved heat dissipation.  Since this is the most power hungry of the devices in this amplifier design, it will help make this amplifier reliable under stressful conditions.
<img class="alignnone size-full wp-image-302" title="ATF-50189 Absolute Maximum Ratings" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-03_07_2013-12_58_02-AM.png" alt="ATF-50189 Absolute Maximum Ratings" width="640" height="255" />

ATF-50189 Absolute Maximum Ratings

The ATF-50189 is in a SOT-89 package and is best suited for high linearity amplifiers because of their low Thermal Resistance.  This device achieves a Channel Resistance of 29°C/W which makes achieving reliable performance possible.

<img class="alignnone size-full wp-image-303" title="ATF-50189 Thermal Analysis" src="http://www.mekesim.com/wp-content/uploads/2016/03/Screenshot-03_07_2013-1_05_14-AM.png" alt="ATF-50189 Thermal Analysis" width="640" height="457" />

ATF-50189 Thermal Analysis

In this analysis you may have noted that we also depend upon an improved PCB Thermal Resistance.  This is due to the large Screws that are placed near the SOT-89 package.  If we really need to improve upon the heat transfer we can always opt for some brass screws.  That will certain shunt the heat more effectively than stainless steel.

ATF-50189 Analysis Results

Power Dissipation = 914mW  (Max 2250mW)
Channel Temperature = 111°C (Max 150°C)
<h2>Summary</h2>
This analysis shows that all of the devices are well suited to meet the rugged reliability requirements needed of this design specification as outlined in <a href="http://www.rfdesignhq.com/2013/03/low-noise-amplifier-design-series-part-i.html?view=magazine" target="_blank">part-1</a>.  In this analysis we entered the parameters and examined the results against the Absolute Maximums.  You can also use the AppCAD design tool to determine the target case temperature to achieve channel temperatures that will provide the desired reliability/deratings a given application may require.  Making this a good heat sink design specification tool as well.

This concludes the thermal analysis of the Low Noise Microwave Amplifier design.

</div>