---
ID: 66
post_title: Sound Propagation
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/66
published: true
post_date: 2015-12-02 08:04:07
---
<span class="blackTen">The sound power level of a source is independent of the environment. However, the sound pressure level at some distance (r) from the source is dependant on that distance and the sound-absorbing characteristics of the environment. Sound propagation is explained in terms of:</span>
<ul>
	<li>Sound Power Level</li>
	<li>Sound Pressure Level</li>
	<li>The Difference Between Sound Power Level and Sound Pressure Level</li>
	<li>The Relationship Between Sound Power Level and Sound Pressure Level
<ul>
	<li>Non-Directional Sound in a Free-field</li>
	<li>Directional Sound in a Free-field</li>
	<li>Unknown Sound Pressure Level</li>
</ul>
</li>
</ul>
<h2>Sound Power Level</h2>
<span class="blackTen">Sound Power (W) is the amount of energy per unit time that radiates from a source in the form of an acoustic wave. The Sound Power Level (L<sub>w</sub>), in decibels, is defined as:</span>
<blockquote>L<sub>w</sub> = 10 log<sub>10</sub> (W/W<sub>0</sub>)

W = sound power in watts
W<sub>o</sub> = reference sound power (10<sup>-12</sup> watts)</blockquote>
<span class="blackTen"><span class="blackTen"><strong>Doubling the sound power increases the sound power level by 3 decibels (dB).</strong></span></span>
<blockquote><strong>Example:</strong>

W = 2 watts:    L<sub>w</sub> = 10 log (2/10<sup>-12</sup>) = 123 dB

W = 4 watts:    L<sub>w</sub> = 10 log (4/10<sup>-12</sup>) = 126 dB</blockquote>
<span class="blackTen">In a free field (no reflections), the sound from a point source radiates equally in all directions in the form of a spherical wave. This distribution of sound power over the area of the propagating wave is designated as intensity and is measured in units of watts per square meter.</span>

Sound power cannot be measured directly. It is possible to measure intensity, but the instruments are relatively expensive and must be used carefully. Under most conditions of sound radiation, sound intensity is proportional to the sound pressure. Sound pressure can be measured more easily, so sound measuring instruments are built to measure the sound pressure level in dB.
<h2>Sound Pressure Level</h2>
<span class="blackTen">The Sound Pressure Level (L<sub>p</sub>), in decibels, is given by the following:</span>
<blockquote>L<sub>p</sub> = 20 log<sub>10</sub> (p/p<sub>0</sub>)

p = measured root-mean-square (rms) sound pressure
p<sub>0</sub> = reference rms sound pressure (20 micropascals (µPa))</blockquote>
<span class="blackTen">The reference sound pressure of 20 micropascals approximates the normal threshold of human hearing at 1,000 Hz.</span>
<ul>
	<li>Note: The multiplier above is 20 and not 10 (as in the case with sound power level). This is because the sound power is proportional to the square of sound pressure and 10 log p<sup>2</sup> = 20 log p.</li>
</ul>
<span class="blackTen">There is a significant advantage to using decibel notation rather than the wide range of pressure or power.</span>
<ul>
	<li>Note: A change in sound pressure by a factor of 10 corresponds to a change in sound pressure level of 20 dB:</li>
</ul>
<blockquote><span class="blackTen">p = 40 µPa:    L<sub>p</sub> = 20 log (40/20) = 6 dB
p = 400 µPa:   L<sub>p</sub> = 20 log (400/20) = 26 dB</span></blockquote>
<span class="blackTen"><span class="blackTen"><strong>Doubling the sound pressure results in an increase of 6 dB in sound pressure level</strong>:</span></span>
<blockquote>p = 40 µPa:    L<sub>p</sub> = 20 log (40/20) = 6 dB
p = 80 µPa:    L<sub>p</sub> = 20 log (80/20) = 12 dB</blockquote>
<img class="alignnone" src="https://www.osha.gov/dts/osta/otm/noise/images/common_sounds.gif" alt="" width="262" height="502" />
<h2>The Difference Between Sound Power Level and Sound Pressure Level</h2>
<span class="blackTen">There is a common tendency to confuse sound power with sound pressure. Sound power is analogous to the power rating of a light bulb.</span>
<ul>
	<li>A "weak" sound source will produce low sound levels, whereas a "stronger" sound source will produce higher sound levels.
<ul>
<ul>
	<li>Sound power level is independent of the environmental surroundings.</li>
</ul>
</ul>
<ul>
	<li>The magnitude of the sound pressure from a given sound source, however, depends on the distance from the source and the characteristics of the environmental surroundings.</li>
</ul>
</li>
	<li>Sound pressure level is readily measured by instruments, but sound power cannot be measured directly.</li>
</ul>
<h2>Non-Directional Sound in a Free-Field</h2>
<span class="blackTen">The simplest relation between sound power level and sound pressure level is found for a free-field, non-directional sound source, as given by the following equation:</span>
<blockquote>L<sub>p</sub> = L<sub>w</sub> - 20 log<sub>10</sub>r - k + T

L<sub>p</sub> = sound pressure level (dB) re 20 µPa
L<sub>w</sub> = sound power level (dB) re 10<sup>-12</sup> watts
r = distance from the source in meters or feet
k = 11.0 dB for metric units and 0.5 dB for English units
T = correction factor for atmospheric pressure and temperature (dB) (since most industrial noise problems are concerned with air at or near standard conditions, T is usually negligible and , therefore, equals 0)</blockquote>
<h2>Directional Sound in a Free-Field</h2>
<span class="blackTen">If the sound is directional in a free field, the relationship between sound power level and sound pressure level becomes (T=0):</span>
<blockquote>L<sub>p</sub> = L<sub>w</sub> - 20 log<sub>10</sub>r + 10 log<sub>10</sub>Q - k

Q = directivity factor</blockquote>
<span class="blackTen">The Directivity Factor (Q) is a dimensionless quantity that is a measure of the degree to which sound emitted by a source is concentrated in a certain direction rather than radiated uniformly in a spherical pattern. Directivity factors for radiation patterns associated with various surfaces surrounding a sound source are shown below. Basically, each radiation pattern is a portion of a spherical radiation pattern; that is, a fraction of the area of a sphere (4pr<sup>2</sup>). The relationship between L<sub>p</sub> and L<sub>w</sub> is also provided for each radiation pattern, as simplified from the previous equation.</span>
<table border="0" summary="" width="80%">
<tbody>
<tr>
<td width="30%"><img title="Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " src="https://www.osha.gov/dts/osta/otm/noise/images/physics1.gif" alt="Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " width="65" height="64" border="0" /></td>
<td class="blackTen" valign="top" width="70%"><strong>Spherical Radiation</strong>
Q = 1
L<sub>p</sub> = L<sub>w</sub> - 20 log<sub>10</sub>r - 1 (r in feet)</td>
</tr>
<tr>
<td width="30%"><img title="1/2 Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " src="https://www.osha.gov/dts/osta/otm/noise/images/physics2.gif" alt="1/2 Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " width="122" height="73" border="0" /></td>
<td class="blackTen" valign="top" width="70%"><strong>1/2 Spherical Radiation</strong>
Q = 2
L<sub>p</sub> = L<sub>w</sub> - 20 log<sub>10</sub>r + 2 (r in feet)</td>
</tr>
<tr>
<td width="30%"><img title="1/4 Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " src="https://www.osha.gov/dts/osta/otm/noise/images/physics3.gif" alt="1/4 Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " width="98" height="89" border="0" /></td>
<td class="blackTen" valign="top" width="70%"><strong>1/4 Spherical Radiation</strong>
Q = 4
L<sub>p</sub> = L<sub>w</sub> - 20 log<sub>10</sub>r + 5 (r in feet)</td>
</tr>
<tr>
<td width="30%"><img title="1/8 Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " src="https://www.osha.gov/dts/osta/otm/noise/images/physics4.gif" alt="1/8 Spherical Radiation - For problems with accessibility in using figures and illustrations, please contact the Directorate of Technical Support and Emergency Management at (202) 693-2300. " width="91" height="95" border="0" /></td>
<td class="blackTen" valign="top" width="70%"><strong>1/8 Spherical Radiation</strong>
Q = 8
L<sub>p</sub> = L<sub>w</sub> - 20 log<sub>10</sub>r + 8 (r in feet)</td>
</tr>
</tbody>
</table>
<span class="blackTen"><span class="blackTen"><strong>Example:</strong> Consider a point source having a L<sub>w</sub> of 110 dB, located outdoors on the ground. The sound pressure level at a distance of 20 feet from the source would be calculated as follows (since the source is located on the ground, the equation for hemispherical radiation from a point source is used):</span></span>
<blockquote>L<sub>p</sub> = L<sub>w</sub> - 20 log<sub>10</sub>r + 2, therefore: L<sub>p</sub> = 110 dB - 20 log<sub>10</sub>(20)  + 2 = 86 dB</blockquote>
<h2>Unknown Sound Pressure Level</h2>
<span class="blackTen">In most situations, the sound power level is unknown. However, we can measure the sound pressure level at a point in the far field, and relate it to another point further from the source. For sound radiation from a point source in a free field, the following relationship applies:</span>
<blockquote><span class="blackTen">L<sub>p1</sub> - L<sub>p2</sub> = 20 log<sub>10</sub> (r<sub>2</sub>/r<sub>1</sub>)</span>

L<sub>p1</sub> = sound pressure level at point 1<sub>
</sub>L<sub>p2</sub> = sound pressure level at point 2
r<sub>1</sub>= distance from source to point 1
r<sub>2</sub> = distance from source to point 2.</blockquote>
<ul>
<ul>
	<li>The distances r<sub>2</sub> and r<sub>1</sub> can be in any units of length (for example, feet, meters), so long as they are the same units, since the argument of a logarithm must always be dimensionless.</li>
	<li>Note the particular case when r<sub>2</sub> = 2r<sub>1</sub>:L<sub>p1</sub> - L<sub>p2</sub> = 20 log<sub>10</sub> (r<sub>2</sub>/r<sub>1</sub>) = 20 log (2) = 6 dB</li>
</ul>
</ul>
<ul>
	<li>This is the familiar inverse-square law (decrease of 6 dB by doubling the distance).</li>
</ul>
<span class="blackTen"><strong>Example:</strong></span> <span class="blackTen"><span class="blackTen">Consider a sound pressure level of 100 dB at a distance of 10 feet. The sound pressure level at a distance of 30 feet from the source would be calculated as follows:</span></span>
<blockquote>L<sub>p2</sub> = L<sub>p1</sub> - 20 log<sub>10</sub> (r<sub>2</sub>/r<sub>1</sub>) = 100 - 20 log (30/10) = 90.5 dB</blockquote>
&nbsp;