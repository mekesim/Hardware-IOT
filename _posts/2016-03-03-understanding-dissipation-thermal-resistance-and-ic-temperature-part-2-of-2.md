---
ID: 248
post_title: >
  Understanding dissipation, thermal
  resistance, and IC temperature (Part 2
  of 2)
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/248
published: true
post_date: 2016-03-03 11:28:57
---
<b>Thermal resistance: θ<sub>Jc</sub> measurement</b>

The test board is placed in the circular enclosure protruding from the elephant system. The temperature of the elephant system is set at 25° C, thus the ambient temperature equals to case temperature T<sub>c</sub> = 25° C. Voltage is applied on V<sub>in</sub> pin and the switch is enabled. Load current I<sub>ou</sub>t is drawn. So with V<sub>in</sub> = 5 V, V<sub>en</sub> = 3 V, load current I<sub>out</sub> = 1 A; the enable current I<sub>enable</sub> and output voltage V<sub>out</sub> are measured.

Since current is drawn by the load, the chip will become hot due to power dissipation. The junction temperature T<sub>j</sub> will differ from the ambient temperature or case temperature. The junction temperature T<sub>j</sub> can be related to power dissipated in the chip using the equation:

T<sub>j</sub> = T<sub>c</sub> + (θ<sub>Jc</sub> × power dissipation)

The junction temperature T<sub>j</sub> can be found by relating the measured enable current to junction temperature graph, which was shown in the previous subsection. Since T<sub>j</sub>, T<sub>c</sub> and power dissipation is known, θ<sub>Jc</sub> can be calculated.

For example, when V<sub>in</sub> = 5 V, V<sub>en</sub> = 3 V and Iout = 1.205 A, the measured I-enable current =1.4056 μAs. The I-enable current can be related to the junction temperature using the graph in previous section. For enable current of 1.4056 μA, T<sub>j</sub> = 36.33° C.

Power dissipation can be calculated as I<sub>out</sub> × (V<sub>out</sub> - V<sub>in</sub>). V<sub>out</sub> was measured as 4.71 V. Power dissipation was calculated as 0.35 W.

θ<sub>Jc</sub> = T<sub>j</sub> - T<sub>c</sub>/(power dissipation) = 36.33 - 25/(0.351) = 32.27° C/ W

Since the board was not set up for performing a Kelvin measurement, the additional voltage drop due to the resistance in the cable and test point turret would increase the measured V<sub>out</sub>and V<sub>in</sub> reading. The power-dissipation calculation would therefore not be accurate.

A better way for finding power dissipation is to use the value of R<sub>ds(on)</sub> of MIC94060. So, power dissipation equals R<sub>ds(on)</sub> × I<sub>out</sub> × I<sub>out</sub>.

Power dissipation =100 mΩ × 1.205 × 1.205 = 0.145 W

and θ<sub>Ja</sub> = 36.33 - 25/(0.14520) = 78.05° C/Watt

<b>Table 4</b> shows the thermal resistance θ<sub>Ja</sub> result taken for board size of 60 mm by 35 mm:

<center><img src="http://m.eet.com/media/1050396/C0230-Table4.gif" alt="" width="350" height="145" border="0" />
<i>Table 4: Thermal resistance θ<sub>Jc</sub> results. </i>
<i>(Click to enlarge image)</i></center>&nbsp;

The result is thermal resistance θ<sub>Jc</sub> between 56° C/W and 80° C/W for different amounts of load current I<sub>out</sub>.

<b>Thermal resistance: θ<sub>Ja</sub> measurement</b>

To perform this measurement, the test board is placed on the lab bench. The elephant temperature system is not used during this test. Room temperature is measured to determine ambient temperature T<sub>a</sub>.

Power is applied to the chip. The chip will get hot and the junction temperature T<sub>j</sub> will be different from the ambient temperature T<sub>a</sub>. The junction temperature T<sub>j</sub> can be related to power dissipated in the chip by:

T<sub>j</sub> = T<sub>a</sub> + (θ<sub>Ja</sub> × power dissipation)

The junction temperature T<sub>j</sub> can be found by relating the measured enable current to junction temperature graph, which was shown in the previous subsection.

As an example, power is applied to the chip. V<sub>in</sub> = 5 V, V<sub>en</sub> = 3 V and I<sub>out</sub> = 1.2052 A; the measured I-enable current = 1.4065 μA. By relating the I-enable current to the junction temperature using the "Enable current versus temperature" graph, the junction temperature T<sub>j</sub> = 36.033° C is found. The power dissipation based upon R<sub>ds(on)</sub> =100 mΩ is R<sub>ds(on)</sub> × Iout × Iout =0.1452. Therefore

θ<sub>Ja</sub> = T<sub>j</sub> - T<sub>a</sub>/(power dissipation) = 36.033-19/(0.1452) = 117.3° C/W

<b>Table 5</b> shows thermal resistance θ<sub>Ja</sub> results taken for board size of 60 mm by 35 mm:

<center><img src="http://m.eet.com/media/1050397/C0230-Table5.gif" alt="" width="350" height="170" border="0" />
<i>Table 5: Thermal resistance θ<sub>Ja</sub> results. </i>
<i>(Click to enlarge image)</i></center>&nbsp;

The result is a thermal resistance θ<sub>Ja</sub> between 90° C/W and 120° C/W for different values of load current I<sub>out</sub>. These values are more accurate representation of thermal behavior for the current board. These values are lower than 240° C/W specified in the datasheet. Observe also that θ<sub>Jc</sub> value is lower than θ<sub>Ja</sub>. This is because during θ<sub>Ja</sub> measurement, the chip is placed in the elephant system which blows air on top of the chip, helping in power dissipation, and in turn, reducing junction temperature.

<b>Further tests for θ<sub>Ja</sub> measurement</b>

When the size of the board was reduced to 30 mm by 30 mm, the results of <b>Table 6</b> were obtained:

<center><img src="http://m.eet.com/media/1050398/C0230-Table6.gif" alt="" width="350" height="55" border="0" />
<i>Table 6: Thermal resistance θ<sub>Ja</sub> of smaller board. </i>
<i>(Click to enlarge image)</i></center>&nbsp;

. The thermal resistance increases to 133.24° C/W. The above result shows that the size of the test board impacts the θ<sub>Ja</sub> result. The smaller the size of the board, the higher the θ<sub>Ja</sub> result. Thus, designers must keep in mind that their board size will impact the thermal resistance of the ICs present on their board.

A plastic bag was placed on top of the test board to prevent air circulation. The results are shown in <b>Table 7</b>:

<center><img src="http://m.eet.com/media/1050399/C0230-Table7.gif" alt="" width="350" height="55" border="0" />
<i>Table 7: Thermal resistance θ<sub>Ja</sub> of smaller covered board. </i>
<i>(Click to enlarge image)</i></center>&nbsp;

The thermal resistance is observed to increase to 152.08° C/W. Thus, the amount of air flow on top of test board impacts the θ<sub>Ja</sub>result. The less the air flow over the board, the higher the θ<sub>Ja</sub>result. Thus, designers must keep in mind that the amount of airflow over the board will impact the thermal resistance of the ICs present on the board.

The thermal resistance number published in datasheets is often based on JEDEC standard. However, this value may not accurately represent the thermal performance on the customer's board and should only be used as a reference. The actual thermal performance on the customer board would depend upon the size of the board, the amount of copper underneath the pins, the air flow in the system and the use of fans in the system.

For Micrel's MIC94060, the thermal resistance of SC70 package is much better than the numbers specified in the datasheet. From the measured data, the maximum θ<sub>Ja</sub> is 100° C/W for 65 mm by 40 mm board, and the maximum θ<sub>Ja</sub> is 133° C/W for 30 mm by 30 mm board. This numbers are much less than θ<sub>Ja</sub> of 240° C/W published in datasheet.

Using the method described in this article for calculating thermal resistance, design engineers will be able to make an accurate estimation of the thermal resistance of the ICs present on their board. The board size and board layout may have to be optimized to reduce the thermal resistance for the expected power consumption. Clearly, using a larger board size, larger amounts of copper area for ground pins, and significant air circulation and fans would help. Once the board is optimized, the junction temperature of individual ICs would not exceed the maximum temperature specified in the datasheet, thus preventing catastrophic board and IC failure.

<b>About the author</b>

<b><i>Hardik Patel</i></b> joined Micrel, Inc. in October 2000 as an application engineer. In 2003 he worked at iWatt as a Test Development Engineer, then rejoined Micrel in 2005 and became a Senior Application Engineer. He is currently responsible for new product evaluation, designing customer evaluation boards, and software and customer technical support. He handles Micrel's high-side power-distribution switches, current-limiting switches, temperature sensors, voltage supervisors, latch drivers, display drivers, fan controllers, and USB transceivers. He holds a Bachelor of Applied Science from University of Toronto in Electrical Engineering. He also is the author of several technical articles and has one patent pending.