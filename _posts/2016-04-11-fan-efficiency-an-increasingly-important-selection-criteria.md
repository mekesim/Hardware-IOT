---
ID: 308
post_title: >
  Fan Efficiency, An Increasingly
  Important Selection Criteria
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/308
published: true
post_date: 2016-04-11 09:34:24
---
<h2 class="re-def">The Importance of Fan Efficiency</h2>
Why is fan efficiency so important? As a general rule, successive generations of electronic enclosures such as personal computers, telecommunications cabinets, as well as system routers, pack increasing functionality into smaller and smaller spaces. Accompanying this trend is the need to remove ever higher levels of heat energy from within those enclosures. Thermal engineers will often force air through a system using fans to regulate the internal temperatures; however as the aerodynamic performance increases so will input power.
In modern day equipment racks it’s not uncommon for the total fan load to be a significant factor in the system’s power budget. Coupled with the advent of equipment efficiency legislation and a growing awareness of cost of ownership, fan efficiency is becoming a critical selection parameter. Engineers now need to gain an understanding of fan efficiency, balancing it against more familiar metrics such as airflow and noise.
<h2 class="re-def">Understanding Fan Static Efficiency</h2>
Fan manufacturers typically provide static efficiency as the value of efficiency, while total efficiency includes the outlet velocity term. Fan total efficiency is calculated using total pressure. Static efficiency is calculated using only static pressure.
Positive static pressure is created as a fan moves air through a system. Negative static pressure is what all other components in the airflow path create as they resist air movement. Different fan types will generate different airflow values while creating a positive static pressure to balance the negative static pressure caused by system obstructions. The fan performance curve (see Fig 1) is a representation of the airflow (X axis) that a particular fan type produces to overcome given static pressure values (Y axis).
Total pressure is the summation of static pressure and outlet velocity pressure. Outlet velocity pressure does not contribute to a fans ability to remove system heat energy; therefore it’s not normally included in fan efficiency calculations.
<h2 class="re-def">Calculating Fan Efficiency</h2>
As with any energy converter, efficiency is the ratio of input and output power:-
Fan efficiency = Pout / Pin
Fan input power (Pin) is:-
Pin (Watts) = V &lt;Volts&gt; x I &lt;Amps&gt;
Fan output power (Pout) or airpower using Metric units is:-
Pout (Watts) = Air pressure &lt;m3/sec&gt; x Air flow &lt;Pascal’s&gt;
Using standard units the formula becomes:-
Pout (Watts) = (Air pressure &lt;inch H2O&gt; x Air flow &lt;cfm&gt;) / 8.5
Example:-
A 48V fan drawing 1A working at an operating point of 200 cfm and 0.5 inch H2O
Pin = 48 x 1 = 48 W
Pout = (200 x 0.5) / 8.5 = 11.76 W
Fan efficiency = 11.76 / 48 = 0.245 or 24.5 %
<h2 class="re-def">The Fan Efficiency Curve</h2>
Fan efficiency varies dramatically as a function of aerodynamic loading. Because airpower is the product of flow and pressure, a fan working in the free air condition (no backflow pressure) has zero pressure and thus is producing no airpower and by definition has zero efficiency. Similarly, a fan in the fully shut off condition (no flow) has zero flow and is also producing no airpower and zero efficiency. The peak efficiency of an axial fan typically occurs at a pressure point of 1/3rd the maximum pressure.
<i>Figure 1 below represents a performance plot of a 120mm size axial fan with curves for both airflow and efficiency.</i>
<img src="http://www.nmbtc.com/fans/white-papers/Fan_Efficiency_Curve.jpg" alt="Fan Performance Airflow and Effeciency" width="526" />
<b>Figure 1: Pressure vs. Flow Curve – 120mm Axial Fan</b>
As a general rule, fan efficiency increases with blade diameter and speed. Fan manufacturers are now focusing on higher efficiency fans, resulting in new designs with significantly increased peak efficiency compared to older designs.
Table 1 provides an indication of peak efficiency values for different standard axial fan sizes and the comparative improvement with newer generation designs.
<strong>Table 1: Axial Fans Typical Peak Efficiency</strong>
<table class="search-results">
<tbody>
<tr>
<th>Form Factor</th>
<th>Old</th>
<th>New</th>
</tr>
<tr>
<td>40 x 40</td>
<td>10%</td>
<td>25%</td>
</tr>
<tr>
<td>60 x 60</td>
<td>14%</td>
<td>30%</td>
</tr>
<tr>
<td>80 x 80</td>
<td>16%</td>
<td>33%</td>
</tr>
<tr>
<td>92 x 92</td>
<td>18%</td>
<td>35%</td>
</tr>
<tr>
<td>120 x 120</td>
<td>24%</td>
<td>40%</td>
</tr>
<tr>
<td>172 round</td>
<td>35%</td>
<td>45%</td>
</tr>
</tbody>
</table>
<h2 class="re-def">Fan Selection Taking Account of Efficiency</h2>
Historically, fans were chosen by finding a standard form factor to occupy the available space and then matching airflow performance against system requirement; typically using free flow as a figure of merit. This approach has the potential for missing significant power savings which could be realized by carefully matching fan efficiency to the system operating point.
In the example shown below, (Fig. 2), selecting the fan based upon free air performance would favor the high flow fan option. Overlaying the system resistance line on the performance curve shows the high flow fan would achieve the required performance of 110cfm at 0.48 inch H2O. However, comparing this fan efficiency at the operating point against an alternative lower free air flow fan design, it can be seen the second design would actually provide higher efficiency while still meeting the duty point.
<img src="http://www.nmbtc.com/fans/white-papers/FanEfficiencyAndSystemImpedance.png" alt="Pressure Vs. Flow Curve with Fan Efficiency and System impedance" width="500" />
<strong>Figure 2: Pressure Vs. Flow Curve with Fan Efficiency and System impedance</strong>
<h2 class="re-def">Benefits of Selecting High Efficiency Fans</h2>
Higher levels of power are required to cool the large amount of heat generated by today’s high end servers. As a result, more electrical power will be needed to be allocated to the system’s cooling components. In some instances, 25% or more of the total power budget for a high end rack system is allocated to the cooling fans.
Using high efficiency fans has a cascade effect on system design. Power supplies can be down sized saving weight and space and the fans power distribution network can be minimized.
The long term benefit of specifying high efficiency fans is a reduction of ownership costs. Large data centers can contain tens of thousands of servers with anywhere between 10 and 50 fans in each. A few percentage points improvement in the efficiency of every fan installed can quickly represent many thousands of dollars in annual energy savings.
High efficiency fans can be more costly than older fan types, and this can be seen as a deterrent. Engineers and purchasing managers should understand the wider implications of using these newer fan designs. System level savings can result from the lower power requirements and substantial energy savings can be realized by the end user.

<strong>Authored by:</strong>
Mr. Nigel D. Strike
Principal Engineer
NMB Technologies Corporation
A Minebea Group Company
Cool Tech R &amp; D Facility
Tempe, Arizona, USA