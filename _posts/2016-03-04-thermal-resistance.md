---
ID: 277
post_title: Thermal Resistance
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/277
published: true
post_date: 2016-03-04 11:16:59
---
<div id="mainContents">
<div id="semicon_index">
<div id="semicon_index_contents">
<div id="document_area">
<div class="semicon_title">INTRODUCTION</div>
Generally, the life of a device would decrease to half, and the failure rate would double whenever Junction Temperature, Tj, goes up by 10°C. Moreover, when Tj exceeds 175°C, a device has the possibility of breaking.Therefore, it is necessary to keep Tj in the proper temperature range, which is the lower the better, and a heat design should be done under the condition of the range of 80-100℃.In fact, it is difficult for IC packages that handle high power to keep Tj in this range. Therefore, it is common to make Tj the 80% of a maximum permissible temperature.A value of a thermal resistance is dependent on a chip, a layout of a leadframe, a board, and so forth. It means even if sizes of the IC packages are the same and layouts of leadframes are different, thermal resistances are not the same.

<a name="product2"></a>
<div class="semicon_title">DEFINITIONS</div>
The thermal resistance of a IC package is calculated by the difference between Tj and the ambient Temperature, Ta, under the condition that the IC package dissipates electric power of 1W. Here are three expressions of the thermal resistance, and each term of expressions are defined in Table1 and Fig.1.
<div class="margin01">
<div class="pkglist2"><img src="http://www.njr.com/semicon/package/images/doc10-09.gif" alt="Thermal resistances" width="99" height="171" /></div>
<div class="pkglist2"><img src="http://www.njr.com/semicon/package/images/doc03-01.gif" alt="Thermal resistances" width="211" height="150" />Fig.1 Thermal resistances of a IC package</div>
</div>
<div class="margin01">
<div class="pkglist">
<table class="pkgtable" border="0" width="95%" cellspacing="0" cellpadding="0"><caption>Table1 Definitions</caption>
<tbody>
<tr>
<th>Item</th>
<th>Definitions</th>
</tr>
<tr>
<td>θja</td>
<td>thermal resistance between Tj and Ta</td>
</tr>
<tr>
<td>ψjt</td>
<td>thermal resistance between Tj and Tc<sub>1</sub></td>
</tr>
<tr>
<td>θjc</td>
<td>thermal resistance between Tj and Tc<sub>2</sub></td>
</tr>
<tr>
<td>θca</td>
<td>thermal resistance between Tc and Ta</td>
</tr>
<tr>
<td>Tj</td>
<td>junction temperature</td>
</tr>
<tr>
<td>Ta</td>
<td>ambient temperature</td>
</tr>
<tr>
<td>Tc<sub>1</sub></td>
<td>temperature of the top surface of IC package</td>
</tr>
<tr>
<td>Tc<sub>2</sub></td>
<td>temperature of the bottom surface of IC package</td>
</tr>
<tr>
<td>P<sub>d</sub></td>
<td>maximum permissible power</td>
</tr>
</tbody>
</table>
</div>
</div>
<div class="clear"></div>
<div class="go_up">
<div class="link_go_top"><a href="http://www.njr.com/semicon/package/thermal.html#top">PageTop</a></div>
</div>
<div class="clear"></div>
<a name="product3"></a>
<div class="semicon_title">Estimation of Tj when ψjt is known</div>
Tj can be estimated by following order
<div class="margin02">
<ol>
	<li>Power, P, is calculated by operating current and voltage.</li>
	<li>Tc<sub>1</sub> is measured by using a thermometer like a radiation thermometer and thermocouples.</li>
	<li>Tj is calculated by Tc<sub>1</sub>, and ψjt which is shown in Table 3.</li>
</ol>
</div>
<strong>Tj=ψjt×P + Tc<sub>1</sub></strong>Note) θja and ψｊt in Table 3 are measured values based on JEDEC with no wind.Each value is dependent on a chip, a layout of a leadframe, a board, and so forth.

<a name="product4"></a>
<div class="semicon_title">Measurement of Thermal Resistance</div>
The measurement of thermal resistance is based on JEDEC.
<div class="margin01"><strong>[Test board]</strong>The outline of the measurement board is shown in Fig.2, which is based on JEDEC.

<img src="http://www.njr.com/semicon/package/images/doc03-02.gif" alt="Measurement board" width="600" height="391" />Fig.2 Measurement board</div>
Note)
<div class="margin01">
<ul>
	<li>Board material : FR-4</li>
	<li>Board dimension:
<ul class="margin02">
	<li>( 2-layer board ) 114.3x76.2mm,Thickness 1.57mm</li>
	<li>( 4-layer board with Cu foil 1,2 ) 114.3x76.2mm,Thickness 1.6mm</li>
</ul>
</li>
	<li>Cu foil dimension : 74.2x74.2mm (Thickness 35µm) are applied to 4-layer board, as Cu foil 1, 2.</li>
</ul>
</div>
<div class="margin01 clear"><strong>[Chip for measurement of Thermal Resistance]</strong>A chip is composed of elements of a resistance and a diode. The resistance is used for heating, and the diode is for a sensor of temperature. We have three kinds of size, because thermal resistance is dependent on a chip size.

<img src="http://www.njr.com/semicon/package/images/doc03-03.gif" alt="Image of the chip" width="400" height="184" />Fig.3 Image of the chip</div>
<div class="margin01"><strong>[Measurement of K factor]</strong>Tj cannot be measured directly. However, by a character of a forward voltage, V <sub>F</sub> of a diode is dependent on temperature. Therefore, Tj is known during a measurement by measuring V<sub>F</sub>.However, dependency of diode which called K-factor, K, should be measured first.

<img src="http://www.njr.com/semicon/package/images/doc10-10_E.gif" alt="K-factor" width="500" height="195" /></div>
<div class="margin01"><strong>[JEDEC chamber]</strong>
<ul>
	<li class="pkglist2">JEDEC chamber with no wind condition (still air) is adopted.The ambient temperature is measured with thermocouples at the position that is located 25.4mm below the center of the IC package.</li>
	<li class="pkglist2"><img src="http://www.njr.com/semicon/package/images/doc10-14_E.gif" alt="JEDEC chamber" width="295" height="292" />Fig.4 JEDEC chamber</li>
</ul>
</div>
<div class="margin01"><strong>[Measurement circuit]</strong><img src="http://www.njr.com/semicon/package/images/doc10-11_E.gif" alt="Measurement circuit" width="411" height="210" />Fig.5 Measurement circuit</div>
<div class="margin01"><strong>[Measurement procedure]</strong>
<ol class="margin02">
	<li>V<sub>F0</sub> is measured by giving the diode with a current (1mA), I<sub>M</sub>, at the ambient temperature.</li>
	<li>A Voltage, V<sub>H</sub>, is given to the resistance in the chip until temperature at upper surface of the IC package, which is measured with a radiation thermometer, is saturated. After confirming the saturation, I<sub>H</sub> is read.</li>
	<li>V<sub>FSS</sub> is measured by giving the diode with a current, I<sub>M</sub>.</li>
</ol>
<img src="http://www.njr.com/semicon/package/images/doc10-12_E.gif" alt="Timing of measurement" width="350" height="107" />Fig.6 Timing of measurement
<p class="margin02">Note) V<sub>H</sub> is measured at three points, the voltage of Tstg-max, Vstg-max, and lower and higher than Vstg-max.</p>

</div>
<div class="margin01"><strong>[Calculation]</strong>θja an ψjt are calculated from the following Table 2.

Table 2 Thermal resistance calculation<img src="http://www.njr.com/semicon/package/images/doc03-08.gif" alt="Thermal resistance calculation" width="500" height="263" />

</div>
<div class="margin01"><strong>[The Permissible Regions of Dissipated Power]</strong>Pd is the maximum permissible power at Ta=25°C.Pd is dependent on the ambient temperture, which is shown in Fig.7.

<img src="http://www.njr.com/semicon/package/images/doc10-13_E.gif" alt="Ambient temperature" width="563" height="277" />Fig.7 The maximum permissible power</div>
<div class="clear"></div>
<div class="go_up">
<div class="link_go_top"><a href="http://www.njr.com/semicon/package/thermal.html#top">PageTop</a></div>
</div>
<div class="clear"></div>
<a name="product5"></a>
<div class="semicon_title">Thermal Resistance of each package</div>
There are typical measured value based on JEDEC with no wind. Each value is dependent on a chip, a layout of a leadframe, a board, and so forth.
<div class="margin01">
<div class="pkglist">
<table class="pkgtable" border="0" width="95%" cellspacing="0" cellpadding="0"><caption>Table 3 Thermal resistance of each package</caption>
<tbody>
<tr>
<th colspan="2" rowspan="4">PKG</th>
<th colspan="4">2 layer board</th>
<th colspan="4">4 layer board</th>
</tr>
<tr>
<th colspan="3">Tj:125°C</th>
<th>Tj:150°C</th>
<th colspan="3">Tj:125°C</th>
<th>Tj:150°C</th>
</tr>
<tr>
<th>θja</th>
<th>ψjt</th>
<th colspan="2">Pd@Ta=25°C</th>
<th>θja</th>
<th>ψjt</th>
<th colspan="2">Pd@Ta=25°C</th>
</tr>
<tr>
<th>(°C/W)</th>
<th>(°C/W)</th>
<th colspan="2">mW</th>
<th>(°C/W)</th>
<th>(°C/W)</th>
<th colspan="2">mW</th>
</tr>
<tr>
<td colspan="2">DMP8</td>
<td>235</td>
<td>47</td>
<td>425</td>
<td>530</td>
<td>175</td>
<td>40</td>
<td>570</td>
<td>710</td>
</tr>
<tr>
<td colspan="2">DMP14</td>
<td>195</td>
<td>47</td>
<td>510</td>
<td>640</td>
<td>150</td>
<td>40</td>
<td>665</td>
<td>830</td>
</tr>
<tr>
<td colspan="2">DMP16</td>
<td>195</td>
<td>47</td>
<td>510</td>
<td>640</td>
<td>150</td>
<td>40</td>
<td>665</td>
<td>830</td>
</tr>
<tr>
<td colspan="2">DMP20</td>
<td>150</td>
<td>37</td>
<td>665</td>
<td>830</td>
<td>120</td>
<td>33</td>
<td>830</td>
<td>1040</td>
</tr>
<tr>
<td colspan="2">SOP8 JEDEC(EMP8)</td>
<td>180</td>
<td>34</td>
<td>555</td>
<td>690</td>
<td>125</td>
<td>29</td>
<td>800</td>
<td>1000</td>
</tr>
<tr>
<td colspan="2">SOP16 JEDEC(EMP16-E2)</td>
<td>110</td>
<td>21</td>
<td>905</td>
<td>1135</td>
<td>70</td>
<td>18</td>
<td>1425</td>
<td>1785</td>
</tr>
<tr>
<td colspan="2">SOP8</td>
<td>165</td>
<td>26</td>
<td>605</td>
<td>755</td>
<td>110</td>
<td>23</td>
<td>905</td>
<td>1135</td>
</tr>
<tr>
<td colspan="2">SOP14</td>
<td>125</td>
<td>21</td>
<td>800</td>
<td>1000</td>
<td>80</td>
<td>17</td>
<td>1250</td>
<td>1560</td>
</tr>
<tr>
<td colspan="2">SOP22</td>
<td>120</td>
<td>18</td>
<td>830</td>
<td>1040</td>
<td>85</td>
<td>14</td>
<td>1175</td>
<td>1470</td>
</tr>
<tr>
<td colspan="2">SOP28</td>
<td>155</td>
<td>37</td>
<td>645</td>
<td>805</td>
<td>125</td>
<td>33</td>
<td>800</td>
<td>1000</td>
</tr>
<tr>
<td colspan="2">SOP40-K1</td>
<td>135</td>
<td>37</td>
<td>740</td>
<td>925</td>
<td>105</td>
<td>33</td>
<td>950</td>
<td>1190</td>
</tr>
<tr>
<td colspan="2">SSOP8</td>
<td>270</td>
<td>42</td>
<td>370</td>
<td>460</td>
<td>210</td>
<td>36</td>
<td>475</td>
<td>595</td>
</tr>
<tr>
<td colspan="2">SSOP8-A3</td>
<td>215</td>
<td>36</td>
<td>465</td>
<td>580</td>
<td>155</td>
<td>15</td>
<td>645</td>
<td>805</td>
</tr>
<tr>
<td colspan="2">SSOP10</td>
<td>270</td>
<td>42</td>
<td>370</td>
<td>460</td>
<td>210</td>
<td>36</td>
<td>475</td>
<td>595</td>
</tr>
<tr>
<td colspan="2">SSOP14</td>
<td>225</td>
<td>38</td>
<td>440</td>
<td>555</td>
<td>180</td>
<td>33</td>
<td>555</td>
<td>690</td>
</tr>
<tr>
<td colspan="2">SSOP16</td>
<td>210</td>
<td>35</td>
<td>475</td>
<td>595</td>
<td>160</td>
<td>26</td>
<td>625</td>
<td>780</td>
</tr>
<tr>
<td colspan="2">SSOP20</td>
<td>185</td>
<td>34</td>
<td>540</td>
<td>675</td>
<td>140</td>
<td>26</td>
<td>710</td>
<td>890</td>
</tr>
<tr>
<td colspan="2">SSOP20-B2</td>
<td>200</td>
<td>34</td>
<td>500</td>
<td>625</td>
<td>150</td>
<td>26</td>
<td>665</td>
<td>830</td>
</tr>
<tr>
<td colspan="2">SSOP20-C3</td>
<td>130</td>
<td>13</td>
<td>765</td>
<td>960</td>
<td>85</td>
<td>9</td>
<td>1175</td>
<td>1470</td>
</tr>
<tr>
<td colspan="2">SSOP32</td>
<td>110</td>
<td>20</td>
<td>905</td>
<td>1135</td>
<td>70</td>
<td>14</td>
<td>1425</td>
<td>1785</td>
</tr>
<tr>
<td colspan="2">SSOP44</td>
<td>110</td>
<td>20</td>
<td>905</td>
<td>1135</td>
<td>70</td>
<td>14</td>
<td>1425</td>
<td>1785</td>
</tr>
<tr>
<td colspan="2">TSSOP54-N1</td>
<td>105</td>
<td>10</td>
<td>950</td>
<td>1190</td>
<td>75</td>
<td>9</td>
<td>1330</td>
<td>1665</td>
</tr>
<tr>
<td colspan="2">HSOP8<sup>2)</sup></td>
<td>160</td>
<td>28</td>
<td>625</td>
<td>780</td>
<td>50</td>
<td>12</td>
<td>2000</td>
<td>2500</td>
</tr>
<tr>
<td colspan="2">HTSSOP24-P1<sup>2)</sup></td>
<td>115</td>
<td>14</td>
<td>865</td>
<td>1085</td>
<td>45</td>
<td>7</td>
<td>2220</td>
<td>2775</td>
</tr>
<tr>
<td colspan="2">MSOP8(TVSP8)</td>
<td>215</td>
<td>27</td>
<td>465</td>
<td>580</td>
<td>160</td>
<td>23</td>
<td>625</td>
<td>780</td>
</tr>
<tr>
<td colspan="2">MSOP10(TVSP10)</td>
<td>215</td>
<td>27</td>
<td>465</td>
<td>580</td>
<td>160</td>
<td>23</td>
<td>625</td>
<td>780</td>
</tr>
<tr>
<td colspan="2">MSOP8(VSP8)</td>
<td>210</td>
<td>33</td>
<td>475</td>
<td>595</td>
<td>155</td>
<td>25</td>
<td>645</td>
<td>805</td>
</tr>
<tr>
<td colspan="2">MSOP10(VSP10)</td>
<td>210</td>
<td>33</td>
<td>475</td>
<td>595</td>
<td>155</td>
<td>25</td>
<td>645</td>
<td>805</td>
</tr>
<tr>
<td colspan="2">SC-88A</td>
<td>355</td>
<td>89</td>
<td>280</td>
<td>350</td>
<td>260</td>
<td>73</td>
<td>380</td>
<td>480</td>
</tr>
<tr>
<td colspan="2">SC-82AB</td>
<td>365</td>
<td>89</td>
<td>270</td>
<td>340</td>
<td>255</td>
<td>72</td>
<td>390</td>
<td>490</td>
</tr>
<tr>
<td colspan="2">SOT-23-5</td>
<td>260</td>
<td>70</td>
<td>380</td>
<td>480</td>
<td>195</td>
<td>60</td>
<td>510</td>
<td>640</td>
</tr>
<tr>
<td colspan="2">SOT-23-6</td>
<td>245</td>
<td>70</td>
<td>405</td>
<td>510</td>
<td>175</td>
<td>60</td>
<td>570</td>
<td>710</td>
</tr>
<tr>
<td colspan="2">SOT-89-3<sup>1)</sup><sup>2)</sup></td>
<td>200</td>
<td>67</td>
<td>500</td>
<td>625</td>
<td>130</td>
<td>65</td>
<td>765</td>
<td>960</td>
</tr>
<tr>
<td colspan="2">QFP32-J2</td>
<td>115</td>
<td>17</td>
<td>865</td>
<td>1085</td>
<td>90</td>
<td>15</td>
<td>1110</td>
<td>1385</td>
</tr>
<tr>
<td colspan="2">QFP44-A1</td>
<td>95</td>
<td>17</td>
<td>1050</td>
<td>1315</td>
<td>75</td>
<td>15</td>
<td>1330</td>
<td>1665</td>
</tr>
<tr>
<td colspan="2">QFP48-P1</td>
<td>65</td>
<td>17</td>
<td>1535</td>
<td>1920</td>
<td>50</td>
<td>15</td>
<td>2000</td>
<td>2500</td>
</tr>
<tr>
<td colspan="2">LQFP48-R3</td>
<td>75</td>
<td>9</td>
<td>1330</td>
<td>1665</td>
<td>45</td>
<td>5</td>
<td>2220</td>
<td>2775</td>
</tr>
<tr>
<td colspan="2">LQFP52-H2</td>
<td>85</td>
<td>11</td>
<td>1175</td>
<td>1470</td>
<td>65</td>
<td>11</td>
<td>1535</td>
<td>1920</td>
</tr>
<tr>
<td colspan="2">QFP56-A1</td>
<td>105</td>
<td>17</td>
<td>950</td>
<td>1190</td>
<td>80</td>
<td>15</td>
<td>1250</td>
<td>1560</td>
</tr>
<tr>
<td colspan="2">QFP64-H1</td>
<td>70</td>
<td>17</td>
<td>1425</td>
<td>1785</td>
<td>50</td>
<td>15</td>
<td>2000</td>
<td>2500</td>
</tr>
<tr>
<td colspan="2">LQFP64-H2</td>
<td>65</td>
<td>6</td>
<td>1535</td>
<td>1920</td>
<td>50</td>
<td>5</td>
<td>2000</td>
<td>2500</td>
</tr>
<tr>
<td colspan="2">QFP100-U1</td>
<td>55</td>
<td>5</td>
<td>1815</td>
<td>2270</td>
<td>45</td>
<td>5</td>
<td>2220</td>
<td>2775</td>
</tr>
<tr>
<td colspan="2">TO-252-3<sup>1)</sup><sup>2)</sup></td>
<td>105</td>
<td>17</td>
<td>950</td>
<td>1190</td>
<td>40</td>
<td>12</td>
<td>2500</td>
<td>3125</td>
</tr>
<tr>
<td colspan="2">PLCC28</td>
<td>55</td>
<td>10</td>
<td>1815</td>
<td>2270</td>
<td>35</td>
<td>7</td>
<td>2855</td>
<td>3570</td>
</tr>
<tr>
<td colspan="2">EPFFP6-A2<sup>2)</sup></td>
<td>370</td>
<td>59</td>
<td>270</td>
<td>335</td>
<td>220</td>
<td>53</td>
<td>450</td>
<td>565</td>
</tr>
<tr>
<td colspan="2">EPFFP10-C4<sup>2)</sup></td>
<td>295</td>
<td>64</td>
<td>335</td>
<td>420</td>
<td>160</td>
<td>55</td>
<td>625</td>
<td>780</td>
</tr>
<tr>
<td colspan="2">PCSP12-C3</td>
<td>240</td>
<td>40</td>
<td>415</td>
<td>520</td>
<td>140</td>
<td>33</td>
<td>710</td>
<td>890</td>
</tr>
<tr>
<td colspan="2">PCSP20-CC</td>
<td>225</td>
<td>40</td>
<td>440</td>
<td>555</td>
<td>140</td>
<td>33</td>
<td>710</td>
<td>890</td>
</tr>
<tr>
<td colspan="2">PCSP20-E3</td>
<td>225</td>
<td>40</td>
<td>440</td>
<td>555</td>
<td>130</td>
<td>33</td>
<td>765</td>
<td>960</td>
</tr>
<tr>
<td colspan="2">PCSP24-ED</td>
<td>205</td>
<td>40</td>
<td>485</td>
<td>605</td>
<td>115</td>
<td>26</td>
<td>865</td>
<td>1085</td>
</tr>
<tr>
<td colspan="2">PCSP32-F7</td>
<td>225</td>
<td>24</td>
<td>440</td>
<td>555</td>
<td>115</td>
<td>17</td>
<td>865</td>
<td>1085</td>
</tr>
<tr>
<td colspan="2">PCSP32-G3<sup>2)</sup></td>
<td>205</td>
<td>24</td>
<td>485</td>
<td>605</td>
<td>115</td>
<td>17</td>
<td>865</td>
<td>1085</td>
</tr>
<tr>
<td colspan="2">PCSP32-GD<sup>2)</sup></td>
<td>205</td>
<td>24</td>
<td>485</td>
<td>605</td>
<td>115</td>
<td>17</td>
<td>865</td>
<td>1085</td>
</tr>
<tr>
<td colspan="2">EPCSP32-L2<sup>2)</sup></td>
<td>210</td>
<td>29</td>
<td>475</td>
<td>595</td>
<td>95</td>
<td>16</td>
<td>1050</td>
<td>1315</td>
</tr>
<tr>
<td colspan="2">DFN6-J1 (SON6-J1)</td>
<td>345</td>
<td>88</td>
<td>285</td>
<td>360</td>
<td>260</td>
<td>69</td>
<td>380</td>
<td>480</td>
</tr>
<tr>
<td colspan="2">DFN4-F1 (ESON4-F1)<sup>2)</sup></td>
<td>300</td>
<td>52</td>
<td>330</td>
<td>415</td>
<td>110</td>
<td>27</td>
<td>905</td>
<td>1135</td>
</tr>
<tr>
<td colspan="2">DFN6-H1 (ESON6-H1)<sup>2)</sup></td>
<td>280</td>
<td>42</td>
<td>355</td>
<td>445</td>
<td>110</td>
<td>26</td>
<td>905</td>
<td>1135</td>
</tr>
<tr>
<td colspan="2">DFN8-U1 (ESON8-U1)<sup>2)</sup></td>
<td>280</td>
<td>43</td>
<td>355</td>
<td>440</td>
<td>110</td>
<td>26</td>
<td>905</td>
<td>1135</td>
</tr>
<tr>
<td colspan="2">DFN8-V1 (ESON8-V1)<sup>2)</sup></td>
<td>215</td>
<td>16</td>
<td>465</td>
<td>580</td>
<td>70</td>
<td>8</td>
<td>1425</td>
<td>1785</td>
</tr>
<tr>
<td colspan="2">DFN8-W2 (ESON8-W2)<sup>2)</sup></td>
<td>195</td>
<td>21</td>
<td>510</td>
<td>640</td>
<td>60</td>
<td>8</td>
<td>1665</td>
<td>2080</td>
</tr>
<tr>
<td colspan="2">QFN24-T1/T2</td>
<td>150</td>
<td>22</td>
<td>665</td>
<td>830</td>
<td>75</td>
<td>15</td>
<td>1330</td>
<td>1665</td>
</tr>
<tr>
<td colspan="2">EQFN12-E2<sup>2)</sup></td>
<td>285</td>
<td>52</td>
<td>350</td>
<td>435</td>
<td>105</td>
<td>27</td>
<td>950</td>
<td>1190</td>
</tr>
<tr>
<td colspan="2">EQFN12-E4<sup>2)</sup></td>
<td>285</td>
<td>52</td>
<td>350</td>
<td>435</td>
<td>105</td>
<td>27</td>
<td>950</td>
<td>1190</td>
</tr>
<tr>
<td colspan="2">EQFN14-D7<sup>2)</sup></td>
<td>295</td>
<td>53</td>
<td>335</td>
<td>420</td>
<td>95</td>
<td>26</td>
<td>1050</td>
<td>1315</td>
</tr>
<tr>
<td colspan="2">EQFN16-G2<sup>2)</sup></td>
<td>255</td>
<td>43</td>
<td>390</td>
<td>490</td>
<td>100</td>
<td>26</td>
<td>1000</td>
<td>1250</td>
</tr>
<tr>
<td colspan="2">EQFN12-JE<sup>2)</sup></td>
<td>215</td>
<td>22</td>
<td>465</td>
<td>580</td>
<td>80</td>
<td>10</td>
<td>1250</td>
<td>1560</td>
</tr>
<tr>
<td colspan="2">EQFN16-JE<sup>2)</sup></td>
<td>180</td>
<td>21</td>
<td>555</td>
<td>690</td>
<td>70</td>
<td>11</td>
<td>1425</td>
<td>1785</td>
</tr>
<tr>
<td colspan="2">EQFN18-E7<sup>2)</sup></td>
<td>220</td>
<td>33</td>
<td>450</td>
<td>565</td>
<td>90</td>
<td>22</td>
<td>1110</td>
<td>1385</td>
</tr>
<tr>
<td colspan="2">EQFN26-HH<sup>2)</sup></td>
<td>160</td>
<td>15</td>
<td>625</td>
<td>780</td>
<td>60</td>
<td>7</td>
<td>1665</td>
<td>2080</td>
</tr>
<tr>
<td colspan="2">EQFN24-LK<sup>2)</sup></td>
<td>145</td>
<td>13</td>
<td>685</td>
<td>860</td>
<td>65</td>
<td>8</td>
<td>1535</td>
<td>1920</td>
</tr>
</tbody>
</table>
</div>
<div class="margin02">Notes
1) Thermal resistance values (θja,ψjt) are measured with the 2-layer board having 100mm<sup>2</sup> copper foil, which is based on JEDEC.
2) Thermal resistance values (θja,ψjt) are measured with the 4-layer board having thermal via holes, which is also based on JEDEC.</div>
</div>
<div class="clear"></div>
<div class="go_up">
<div class="link_go_top"><a href="http://www.njr.com/semicon/package/thermal.html#top">PageTop</a></div>
</div>
<div class="clear"></div>
<a name="product6"></a>
<div class="semicon_title">Thermal Resistance depending on area of Cu foil</div>
There are typical values by mounting on five kinds of boards, "PAT.1" through "PAT.5", shown in Table 4 and Table 5.Those are 2-layer boards based on JEDEC. However, they do not have any thermal via holes.

<img src="http://www.njr.com/semicon/package/images/netu_1.gif" alt="Thermal Resistance depending on area of Cu foil" width="600" height="581" />Fig.8 Thermal Resistance depending on area of Cu foil<img src="http://www.njr.com/semicon/package/images/netu_2.gif" alt="Image of Cu foil" width="150" height="60" />Table 4 Image of Cu foil
<div class="margin01">
<div class="pkglist">
<table class="pkgtable" border="0" width="95%" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td><img src="http://www.njr.com/semicon/package/images/teble.gif" alt="teble" width="100" height="50" /></td>
<td>TO-252</td>
<td>SOT-89</td>
<td>SOT-23-5
SOT-23-6</td>
</tr>
<tr>
<td>PAT.1</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_3.gif" alt="PAT" width="32" height="42" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_4.gif" alt="PAT" width="32" height="38" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_5.gif" alt="PAT" width="44" height="31" /></td>
</tr>
<tr>
<td>PAT.2</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_6.gif" alt="PAT" height="60" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_7.gif" alt="PAT" width="48" height="55" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_8.gif" alt="PAT" width="66" height="52" /></td>
</tr>
<tr>
<td>PAT.3</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_9.gif" alt="PAT" width="64" height="74" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_10.gif" alt="PAT" width="62" height="70" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_11.gif" alt="PAT" width="86" height="71" /></td>
</tr>
<tr>
<td>PAT.4</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_12.gif" alt="PAT" width="78" height="88" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_13.gif" alt="PAT" width="75" height="80" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_14.gif" alt="PAT" width="126" height="115" /></td>
</tr>
<tr>
<td>PAT.5</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_15.gif" alt="PAT" width="109" height="121" /></td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_16.gif" alt="PAT" width="108" height="116" /></td>
<td class="center">-</td>
</tr>
</tbody>
</table>
</div>
<div class="pkglist">
<table class="pkgtable" border="0" width="95%" cellspacing="0" cellpadding="0"><caption>Table 5 Image of Cu foil</caption>
<tbody>
<tr>
<td class="center"><img src="http://www.njr.com/semicon/package/images/teble.gif" alt="PAT" width="100" height="50" /></td>
<td class="center">SC-88A
SC-82AB</td>
</tr>
<tr>
<td class="center">PAT.1</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_17.gif" alt="PAT" width="42" height="30" /></td>
</tr>
<tr>
<td class="center">PAT.2</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_18.gif" alt="PAT" width="62" height="54" /></td>
</tr>
<tr>
<td class="center">PAT.3</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_19.gif" alt="PAT" width="82" height="70" /></td>
</tr>
<tr>
<td class="center">PAT.4</td>
<td class="center"><img src="http://www.njr.com/semicon/package/images/netu_20.gif" alt="PAT" width="123" height="114" /></td>
</tr>
</tbody>
</table>
</div>
<div class="pkglist">
<table class="pkgtable" border="0" width="95%" cellspacing="0" cellpadding="0"><caption>Table 6 Area of Cu foil</caption>
<tbody>
<tr>
<td class="center"><img src="http://www.njr.com/semicon/package/images/teble_2.gif" alt="teble" width="70" height="35" /></td>
<td class="center">TO-252</td>
<td class="center">SOT-89</td>
<td class="center">SOT-23-5
SOT-23-6</td>
<td class="center">SC-88A
SC-82AB</td>
</tr>
<tr>
<td class="center">PAT.1</td>
<td class="center" colspan="4">100mm<sup>2</sup></td>
</tr>
<tr>
<td class="center">PAT.2</td>
<td class="center" colspan="4">225mm<sup>2</sup></td>
</tr>
<tr>
<td class="center">PAT.3</td>
<td class="center" colspan="4">400mm<sup>2</sup></td>
</tr>
<tr>
<td class="center">PAT.4</td>
<td class="center" colspan="2">600mm<sup>2</sup></td>
<td class="center" colspan="2">1600mm<sup>2</sup></td>
</tr>
<tr>
<td class="center">PAT.5</td>
<td class="center" colspan="2">1225mm<sup>2</sup></td>
<td class="center" colspan="2">-</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="clear"></div>
</div>
<div class="clear"></div>
<div id="footer"></div>