---
ID: 55
post_title: Introduction to the Fan Laws
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/55
published: true
post_date: 2015-12-01 02:35:33
---
The fan engineer is faced with many challenges when selecting a fan to meet specified requirements. Often, many solutions must be evaluated to make the optimum selection. This can be daunting task even with modern computing methods. Fan airflow performance is characterized by three basic parameters – the flow rate, pressure rise, and required power. These parameters are easily obtained in the laboratory for a given fan speed, fan size, and air density. But what about the fan performance at a different fan speed, fan size, or air density? Clearly, it is not very practical to test the fan at all possible conditions.

Fortunately, the fan engineer has a very powerful tool in the <em>Fan Laws</em>.

The <em>Fan Laws</em> provide a simple way to evaluate fan performance for various speeds, diameters, and air densities using data obtained for a known fan speed, fan size, and standard air density. The <em>Fan Laws</em> for airflow performance are as follows:

<img class="alignnone size-full wp-image-56" src="http://en.mekesim.com/wp-content/uploads/2015/12/fan_laws.png" width="160" height="144" alt="f" />

where <em>Q</em>, <em>P</em>, and <em>H</em> are the airflow rate, pressure rise, and fan power respectively. <em>N</em>, <em>D</em>, and <em>ρ</em>, are the fan speed, fan diameter, and air density. The subscript '<em>r</em>' represents the known, or reference, operating conditions. The <em>Fan Laws</em> are expressed in the form of ratios so that it easy to see the effect of changes in speed, diameter, and air density. For example, if the speed of a given fan is doubled then the speed ratio (<em>N/Nr</em>) is 2, the diameter ratio is 1 (it's the same fan) – so the resulting airflow rate ratio is 2. Simply stated, doubling the speed will double the airflow output. Likewise, the pressure will increase by a factor of 4 and the power by a factor of 8, provided that the air density remains the same.

Although the <em>Fan Laws</em> are based on well established physical principles, certain conditions must be met to assure their proper use.

The most restrictive condition involves changes in fan size. Changes in fan diameter strictly apply to fans that are geometrically similar. This means that dimensional features of the two fans must be in proportion to their diameters. In addition, the two fans must have the same number of blades. This condition is often difficult to meet. Fortunately, fan performance data is readily available for various fan diameters except in the case of very large fans (&gt;60" diameter) were laboratory testing is not practical. Outside of these cases, the application of fan laws for changes in fan diameter is seldom needed.

Changes in fan speed are more common. Here too there are limits to what can be predicted with the fan laws. A speed change of about 20% will generally give good results. Predicting fan performance for higher speeds will give conservative results since higher speeds will generally be more efficient. It is not recommended to predict fan performance at lower speeds than the reference data since the efficiency may be over predicted.

Finally, performance changes due to variations in air density can be calculated. This aspect is often overlooked and can be significant when selecting fans to operate at altitude. A fan rated at sea level will have the same airflow rate under all density conditions, but pressure rise and power required will become smaller as the air density decreases. The table below shows the effect of altitude and temperature on the air density ratio.

<center><strong>Density Ratio with Altitude and Temperature</strong>
(relative to sea level and 70 °F)
<img class="alignnone size-full wp-image-57" src="http://en.mekesim.com/wp-content/uploads/2015/12/density_ratio.jpg" width="465" height="219" alt="f" /></center>For example, a fan operating at 5000 ft and 60° F will have 15% less pressure rise and power than at standard sea level conditions.

Example: A 12" fan running at 1250 rpm produces an airflow rate of 3000 cfm at 2.5 in-wg pressure rise and requires 1.9 Hp. The customer would like to move 3500 cfm through the same airflow system. What is the required speed and power to accomplish this? The new speed can be calculated using the airflow rate fan law relationship. Note that the diameter and density ratios are both equal to one. The new speed is 1458 rpm. The new pressure rise and power required can be calculated from the other two fan law relationships, giving 3.4 in-wg and 3 Hp. This is a considerable change in motor power. The fan engineer must review these results to assure that the new speed is within the fan's capability and that the existing motor can produce the required power.