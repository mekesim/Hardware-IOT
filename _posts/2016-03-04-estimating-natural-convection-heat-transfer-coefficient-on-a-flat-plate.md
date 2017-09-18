---
ID: 270
post_title: >
  Estimating Natural Convection Heat
  Transfer Coefficient on a Flat Plate
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/270
published: true
post_date: 2016-03-04 09:31:30
---
Although most of the emphasis today in the electronics cooling community is devoted to extending forced convection cooling capability, many applications still depend upon natural convection cooling. Basically, natural convection cooling combined with radiation is what results when a fan is not used in the cooling design to move air. Instead, movement of the air is induced by density differences resulting from the heat dissipated by the electronic components. An obvious advantage of natural convection, or “free” convection as it is sometimes called, is that the expense of incorporating a fan is avoided. Of course the penalty associated with this method of cooling is lower heat transfer coefficients.

To estimate the surface temperatures of components mounted on a card or board we sometimes approximate the surface as a flat plate. We can then use dimensionless natural convection correlations to estimate the natural convection heat transfer coefficient [1]. These correlations take the form,
<table border="0" width="100%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td><img class="alignnone size-full wp-image-271" src="http://www.mekesim.com/wp-content/uploads/2016/03/2001_August_calccorner_formula1-2.jpg" width="505" height="124" alt="" /></td>
</tr>
</tbody>
</table>
where
<table border="0" width="100%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td>
<table id="Table1" border="0" width="66%" cellspacing="0" cellpadding="1">
<tbody>
<tr>
<td width="8%">c<sub>p</sub></td>
<td align="center" width="7%">=</td>
<td width="84%">Specific heat constant pressure</td>
</tr>
<tr>
<td width="8%">g<sub>c</sub></td>
<td align="center" width="7%">=</td>
<td width="84%">Gravitational acceleration</td>
</tr>
<tr>
<td width="8%">Gr</td>
<td align="center" width="7%">=</td>
<td width="84%">Grashof number (dimensionless)</td>
</tr>
<tr>
<td width="8%">h</td>
<td align="center" width="7%">=</td>
<td width="84%">Heat transfer coefficient</td>
</tr>
<tr>
<td width="8%">k</td>
<td align="center" width="7%">=</td>
<td width="84%">Thermal conductivity of air</td>
</tr>
<tr>
<td width="8%">L</td>
<td align="center" width="7%">=</td>
<td width="84%">Height or length of plate</td>
</tr>
<tr>
<td width="8%">Nu</td>
<td align="center" width="7%">=</td>
<td width="84%">Nusselt number (dimensionless)</td>
</tr>
<tr>
<td width="8%">Pr</td>
<td align="center" width="7%">=</td>
<td width="84%">Prandtl number (dimensionless)</td>
</tr>
<tr>
<td width="8%">Ra</td>
<td align="center" width="7%">=</td>
<td width="84%">Rayleigh number (dimensionless)</td>
</tr>
<tr>
<td width="8%">T<sub>a</sub></td>
<td align="center" width="7%">=</td>
<td width="84%">Temperature of ambient air</td>
</tr>
<tr>
<td width="8%">T<sub>s</sub></td>
<td align="center" width="7%">=</td>
<td width="84%">Temperature of heated surface</td>
</tr>
<tr>
<td width="8%"><img id="Picture587" src="http://s3.electronics-cooling.com/legacy_images/2002/08/sym_068.gif" alt="" width="10" height="11" align="middle" border="0" hspace="0" />T</td>
<td align="center" width="7%">=</td>
<td width="84%">Temperature difference from surface to air</td>
</tr>
<tr>
<td width="8%"><strong><em>B</em></strong></td>
<td align="center" width="7%">=</td>
<td width="84%">Coefficient of thermal expansion for air</td>
</tr>
<tr>
<td width="8%"><img id="Picture589" src="http://s3.electronics-cooling.com/legacy_images/2001/08/sym_114.gif" alt="" width="7" height="11" align="middle" border="0" hspace="0" /></td>
<td align="center" width="7%">=</td>
<td width="84%">Density of air</td>
</tr>
<tr>
<td width="8%"><img id="Picture592" src="http://s3.electronics-cooling.com/legacy_images/2003/02/mu.gif" alt="" width="8" height="12" align="bottom" border="0" hspace="0" /></td>
<td align="center" width="7%">=</td>
<td width="84%">Dynamic viscosity of air</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
The value of constant C and exponent n will depend upon the orientation of the heated surface as given in Table 1.

Table 1. Value of Constant C and Exponent n
<table border="0" width="100%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td>
<table id="Table2" border="1" width="94%" cellspacing="0" cellpadding="1">
<tbody>
<tr>
<td width="15%">Plate</td>
<td width="50%">Dimensionless Correlation (1)
C n</td>
<td width="33%">Simplified Formula for h
C n</td>
</tr>
<tr>
<td width="15%">Vertical</td>
<td width="50%">.59 .25</td>
<td width="33%">1.42 .25</td>
</tr>
<tr>
<td width="15%">Horizontal
(heated)</td>
<td width="50%">.54 .25</td>
<td width="33%">1.32 .25</td>
</tr>
<tr>
<td width="15%">Horizontal
(heated)</td>
<td width="50%">.27 .25</td>
<td width="33%">.59 .25</td>
</tr>
</tbody>
</table>
</td>
</tr>
</tbody>
</table>
Thermophysical properties of air for use in equations 1 and 2 may be found in any basic heat transfer textbook [2]. The values of air properties to be used should be at the mean film temperature, which is defined as the average of the surface temperature and the free air temperature away from the plate.

The problem in using these correlations is that we usually have an idea of the power being dissipated and want to calculate a surface temperature so that we can estimate some component internal temperature. Since we do not know the surface temperature a priori, we must guess a temperature to obtain the air properties and <img id="Picture591" src="http://s3.electronics-cooling.com/legacy_images/2002/08/sym_068.gif" alt="" width="10" height="11" align="middle" border="0" hspace="0" />T to use in the correlations to calculate h.Fortunately, there is a simplified formula for air, which gives the heat transfer coefficient for natural convection of air over a flat plate [1]. This formula is of the form,
<table border="0" width="100%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td><img class="alignnone size-full wp-image-272" src="http://www.mekesim.com/wp-content/uploads/2016/03/2001_August_calccorner_formula3.jpg" width="300" height="41" alt="" /></td>
</tr>
</tbody>
</table>
Although this formula also depends upon surface temperature, T<sub>s</sub>, if we combine it with the Newton rate equation,
<table border="0" width="100%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td><img class="alignnone size-full wp-image-273" src="http://www.mekesim.com/wp-content/uploads/2016/03/2001_August_calccorner_formula4.jpg" width="250" height="41" alt="" /></td>
</tr>
</tbody>
</table>
after a little algebraic manipulation we can obtain an expression for T<sub>s</sub> as a function of the heat dissipation, q, from the plate surface,
<table border="0" width="100%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td><img class="alignnone size-full wp-image-274" src="http://www.mekesim.com/wp-content/uploads/2016/03/2001_August_calccorner_formula5.jpg" width="300" height="54" alt="" /></td>
</tr>
</tbody>
</table>
A comparison of the value of natural convection h for a 100 mm square plate calculated using dimension-less equation 2 versus the simplified dimensional equation 3 is shown in Figure 1. These results show that the simplified formula underpredicts h by 3 to 6 % for the vertical plate and the horizontal plate with heated side up. For the case of a horizontal plate with the heated side down the simplified formula underpredicts h by 13 to 15 %.
<table border="0" width="100%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td><img class="alignnone size-full wp-image-275" src="http://www.mekesim.com/wp-content/uploads/2016/03/2001_August_Cal_Corner_Fig1.jpg" width="500" height="255" alt="" /></td>
</tr>
</tbody>
</table>
Figure 1. Heat transfer coefficient plotted against surface temperature.The equations presented here are valid only for laminar natural convection. In most electronic cooling applications it is unlikely that turbulent natural convection will be encountered. It should also be noted that both the dimensionless equation and the simplified dimensional equation are valid only if there are no surfaces nearby to interfere with development of the natural convection boundary layer. The effect of nearby surfaces on natural convection heat transfer is a topic for future columns.

<strong>References
</strong>1. McAdams, W.H., Heat Transmission, 3rd ed., McGraw-Hill, New York, NY, 1954.
2. Incropera, F.P., and DeWitt, D.P., Fundamentals of Heat and Mass Transfer, John Wiley and Sons, New York, NY, 1985.