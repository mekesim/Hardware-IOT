---
ID: 135
post_title: >
  Introduction to thermal and electrical
  conductivity
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/135
published: true
post_date: 2016-01-25 14:45:04
---
<h2>Contents</h2>
<div class="navlist3">
<ul>
	<li>Aims</li>
	<li>Before you start</li>
	<li>Introduction</li>
	<li>Introduction to conduction</li>
	<li>Metals: the Drude model of electrical conduction</li>
	<li>Factors affecting electrical conduction</li>
	<li>Thermal conduction metals</li>
	<li>Electrical conduction: non metals</li>
	<li>Non-metals: thermal phonons</li>
	<li>Applications</li>
	<li>Summary</li>
	<li>Questions</li>
	<li>Going further</li>
</ul>
</div>
<h2>Aims</h2>
On completion of this tutorial package, you should:
<ul type="disc">
	<li>Understand the basic mechanisms and models of thermal and electrical conduction, in metals and non metals.</li>
	<li>Be aware of some of the factors that affect both types of conduction.</li>
	<li>Know some of the applications for both types of conductors and insulators.</li>
</ul>
<h2>Before you start</h2>
This TLP is an introduction, so no specific prior knowledge is required. There are, however, other TLPs that cover more advanced topics, such as semiconductors, which are linked to in the further reading section.
<h2>Introduction</h2>
Electrical conductivity spans an incredibly large order of magnitudes (30!) from insulators to metals, and can even be infinite in superconductors. Knowledge of  how to control it has allowed for the computer revolution, and ever increasing miniaturisation

Thermal conductivity, while only spanning arround 10 orders of magnitude for known materials, is still crucial for many important technological advancements, from jet turbines and space travel to USB drinks coolers.

To truly appreciate these achievements, it is vital to have an understanding of how conductivity arises in materials. There are simple models that can be used to predict the behaviour of many materials; close parallels exist between thermal and electrical conduction in metals, whereas the conduction mechanisms in non-metals are quite different.
<h2>Introduction to conduction</h2>
<h2>Electrical conduction</h2>
It is important to not get confused by conduction, conductivity, resistance, and resistivity.

The materials properties are electrical conductivity, <span class="greekSymbol">σ</span> , and electrical resistivity, <span class="greekSymbol">ρ</span>

The electrical conductivity of a material is defined as the amount of electric charge transferred per unit time across unit area under the action of a unit potential gradient: <span class="variable">J</span> = <span class="greekSymbol">σ</span> <span class="variable">E</span>

where <span class="variable">J</span> is the current density (current per unit area) and <span class="variable">E</span> is the potential gradient. This is another way of expressing Ohm’s law, which is more commonly stated as <span id="MathJax-Element-1-Frame" class="MathJax"><span id="MathJax-Span-1" class="math"><span id="MathJax-Span-2" class="mrow"><span id="MathJax-Span-3" class="mi">V</span><span id="MathJax-Span-4" class="mo">=</span><span id="MathJax-Span-5" class="mi">I</span><span id="MathJax-Span-6" class="mi">R</span></span></span></span>.

For an isotropic material:
<div class="MathJax_Display"><span id="MathJax-Element-2-Frame" class="MathJax"><span id="MathJax-Span-7" class="math"><span id="MathJax-Span-8" class="mrow"><span id="MathJax-Span-9" class="mi">σ</span><span id="MathJax-Span-10" class="mo">=</span><span id="MathJax-Span-11" class="mfrac"><span id="MathJax-Span-12" class="mn">1</span><span id="MathJax-Span-13" class="mi">ρ</span></span></span></span></span></div>
The units of electrical resistivity are the ohm metre (<strong><span class="greekSymbol">Ω</span><span class="variable">m</span></strong>), and for conductivity, the inverse (<strong><span class="greekSymbol">Ω</span><sup>-1</sup> <span class="variable">m</span><sup>-1</sup> </strong>). For an actual sample of length <span class="variable">l</span>, and cross sectional area <span class="variable">A</span>, the resistance, <span class="variable">R</span>, is calculated by :
<div class="MathJax_Display"><span id="MathJax-Element-3-Frame" class="MathJax"><span id="MathJax-Span-14" class="math"><span id="MathJax-Span-15" class="mrow"><span id="MathJax-Span-16" class="mi">R</span><span id="MathJax-Span-17" class="mo">=</span><span id="MathJax-Span-18" class="mi">ρ</span><span id="MathJax-Span-19" class="mfrac"><span id="MathJax-Span-20" class="mi">l</span><span id="MathJax-Span-21" class="mi">A</span></span></span></span></span></div>
Electrical signals propagate at close to the speed of light, though this does <strong>not</strong> mean the electrons themselves move this quickly. Instead, the typical electron <em>drift velocity</em> (their average velocity) is much lower: less than 1 mm s<sup>-1</sup>. This is expanded upon in the Drude model section.

Another pertinent reminder is that of potential and current – current is the flow of electrons, and potential is the driving force that makes them flow. With sufficient potential, electrons may carry charge through any material, including a vacuum (see CRT), though they are powerless without any net current flow.

The best electrical conductors (apart from superconductors) are pure copper and pure silver, with resistivities of 16.78 and 15.87  nΩm respectively.  For comparison, polystyrene has a resistivity of up to 10<sup>28</sup> nΩm, 27 orders of magnitude different!
<h2>Thermal conduction:</h2>
To understand thermal conductivity in materials, it is important to be familiar with the concept of heat transfer, which is the movement of thermal energy from a hotter to a colder body. It occurs in several circumstances:
<ul type="disc">
	<li>When an object is at a different temperature from its surroundings;</li>
	<li>When an object is at a different temperature to another object in contact with it;</li>
	<li>When a temperature gradient exists within the object.</li>
</ul>
The direction of heat transfer is set by the second law of thermodynamics, which states that the entropy of an isolated system which is not in thermal equilibrium will tend to increase over time, approaching a maximum value at equilibrium. This means heat transfer always occurs from a body at a higher temperature to a body at a lower temperature, and will continue until thermal equilibrium is reached.

A transfer of thermal energy occurs only through 3 modes: conduction, convection, and radiation. Each mode has a different mechanism and rate of heat transfer, and thus, in any particular situation, the rate of heat transfer depends on how much a certain mode is prevalent.

<strong>Conduction</strong> involves the transfer of thermal energy by a combination of diffusion of electrons and phonon vibrations – applicable to solids.

<strong>Convection</strong> involves the transfer of thermal energy in a moving medium – the hot gas/liquid moves through the cooler medium(normally due to density differences).

<strong>Radiation</strong> involves the transfer of thermal energy by electromagnetic radiation. The sun is a good example of energy transfer through a (near) vacuum.

This TLP focuses on conduction in crystalline solids.

Thermal conductivity, <strong><span class="greekSymbol">Κ</span>,</strong> is the materials property that indicates the ability to conduct heat. Fourier’s first law gives the heat flux as proportional to the temperature difference, surface area, and length of the sample:
<div class="MathJax_Display"><span id="MathJax-Element-4-Frame" class="MathJax"><span id="MathJax-Span-22" class="math"><span id="MathJax-Span-23" class="mrow"><span id="MathJax-Span-24" class="mi">H</span><span id="MathJax-Span-25" class="mo">=</span><span id="MathJax-Span-26" class="mfrac"><span id="MathJax-Span-27" class="mrow"><span id="MathJax-Span-28" class="mi">Δ</span><span id="MathJax-Span-29" class="mi">Q</span></span><span id="MathJax-Span-30" class="mrow"><span id="MathJax-Span-31" class="mi">Δ</span><span id="MathJax-Span-32" class="mi">t</span></span></span><span id="MathJax-Span-33" class="mo">=</span><span id="MathJax-Span-34" class="mi">κ</span><span id="MathJax-Span-35" class="mi">A</span><span id="MathJax-Span-36" class="mfrac"><span id="MathJax-Span-37" class="mrow"><span id="MathJax-Span-38" class="mi">Δ</span><span id="MathJax-Span-39" class="mi">T</span></span><span id="MathJax-Span-40" class="mi">l</span></span></span></span></span></div>
where <span class="greekSymbol">Δ</span><span class="variable">Q</span> / <span class="greekSymbol">Δ</span><span class="variable">t</span> is the rate of heat transfer, <span class="variable">A</span> is the surface area and <span class="variable">l</span> is the length.

The best metallic thermal conductors are pure copper and silver. At room temperature, commercially pure copper typically has a conductivity of about 360 Wm<sup>-1</sup>K<sup>-1</sup> (although the thermal conductivity of a single crystal of copper was measured at 12,200 Wm<sup>-1</sup>K<sup>-1</sup> at a temperature of 20.8 K). In metals, the movement of electrons dominates the conduction of heat.

The bulk material with the highest thermal conductivity (aside from the superfluid helium II) is, perhaps surprisingly, a non-metal: pure single crystal diamond, which has a thermal conductivity at room temperature of around 2200 Wm<sup>-1</sup>K<sup>-1</sup>. The high conductivity is even used to test the authenticity of a diamond. Strong covalent bonds within the molecule are responsible for the high conductivity even though there are no free electrons, heat is conducted by phonons. Most natural diamonds also contain boron atoms that replace carbon atoms in the crystal matrix, which also have high thermal conductance.
<h2>Metals: the Drude model of electrical conduction</h2>
Due to the quantum mechanical nature of electrons, a full simulation of electron movement in a solid (i.e. conduction) would require consideration of not only all the positive ion cores interacting with each electron, <em>but also each electron with every other electron</em>. Even with advanced models, this rapidly becomes far too complicated to model adequately for a material of macroscopic scale.

The Drude model simplifies things considerably by using classical mechanics and treats the solid as a fixed array of nuclei in a ‘sea’ of unbound electrons. Additionally, the electrons move in straight lines, do not interact with each other, and are scattered randomly by nuclei.

Rather than model the whole lattice, two statistically derived numbers are used:
<strong><span class="greekSymbol">τ</span></strong>, the average time between collisions (the <strong>scattering time</strong>), and
<strong><span class="variable">l</span></strong>, the average distance traveled between collisions  (the <strong>mean free path</strong>)

Under the application of a field, <span class="variable">E</span>, electrons experience a force –<span class="variable">e E</span>, and thus an acceleration from <span class="variable">F = m a</span>

For an electron emerging from a collision with velocity <span class="variable">v</span><sub>0</sub>, the velocity after time <span class="variable">t</span> is given by:
<div class="MathJax_Display"><span id="MathJax-Element-5-Frame" class="MathJax"><span id="MathJax-Span-41" class="math"><span id="MathJax-Span-42" class="mrow"><span id="MathJax-Span-43" class="mi">v</span><span id="MathJax-Span-44" class="mo">=</span><span id="MathJax-Span-45" class="msubsup"><span id="MathJax-Span-46" class="mi">v</span><span id="MathJax-Span-47" class="texatom"><span id="MathJax-Span-48" class="mrow"><span id="MathJax-Span-49" class="mn">0</span></span></span></span><span id="MathJax-Span-50" class="mo">−</span><span id="MathJax-Span-51" class="mfrac"><span id="MathJax-Span-52" class="mrow"><span id="MathJax-Span-53" class="mi">e</span><span id="MathJax-Span-54" class="mi">E</span><span id="MathJax-Span-55" class="mi">t</span></span><span id="MathJax-Span-56" class="mi">m</span></span></span></span></span></div>
Of course, if the electrons are scattered randomly by each collision, <span class="variable">v</span><sub>0</sub> will be zero. If we also consider the time <span class="variable">t</span> = <span class="greekSymbol">τ</span>, an equation for the <strong>drift velocity</strong> is given:
<div class="MathJax_Display"><span id="MathJax-Element-6-Frame" class="MathJax"><span id="MathJax-Span-57" class="math"><span id="MathJax-Span-58" class="mrow"><span id="MathJax-Span-59" class="mi">v</span><span id="MathJax-Span-60" class="mo">=</span><span id="MathJax-Span-61" class="mfrac"><span id="MathJax-Span-62" class="mrow"><span id="MathJax-Span-63" class="mo">−</span><span id="MathJax-Span-64" class="mi">e</span><span id="MathJax-Span-65" class="mi">E</span><span id="MathJax-Span-66" class="mi">τ</span></span><span id="MathJax-Span-67" class="mi">m</span></span></span></span></span></div>
For <strong><span class="variable">n</span></strong> free electrons per unit volume, the current density <span class="variable">J</span> is: <span class="variable">J</span> = -<span class="variable">n e v</span>

Substituting <span class="variable">v</span> for the drift velocity:
<div class="MathJax_Display"><span id="MathJax-Element-7-Frame" class="MathJax"><span id="MathJax-Span-68" class="math"><span id="MathJax-Span-69" class="mrow"><span id="MathJax-Span-70" class="mi">J</span><span id="MathJax-Span-71" class="mo">=</span><span id="MathJax-Span-72" class="mfrac"><span id="MathJax-Span-73" class="mrow"><span id="MathJax-Span-74" class="mi">n</span><span id="MathJax-Span-75" class="msubsup"><span id="MathJax-Span-76" class="mi">e</span><span id="MathJax-Span-77" class="texatom"><span id="MathJax-Span-78" class="mrow"><span id="MathJax-Span-79" class="mn">2</span></span></span></span><span id="MathJax-Span-80" class="mi">τ</span><span id="MathJax-Span-81" class="mi">E</span></span><span id="MathJax-Span-82" class="mi">m</span></span></span></span></span></div>
The conductivity <span class="greekSymbol">σ</span> = <span class="variable">n e</span> <span class="greekSymbol">μ</span>, where <span class="greekSymbol">μ</span> is the <strong>mobility</strong>, which is defined as
<div class="MathJax_Display"><span id="MathJax-Element-8-Frame" class="MathJax"><span id="MathJax-Span-83" class="math"><span id="MathJax-Span-84" class="mrow"><span id="MathJax-Span-85" class="mi">μ</span><span id="MathJax-Span-86" class="mo">=</span><span id="MathJax-Span-87" class="mfrac"><span id="MathJax-Span-88" class="mrow"><span id="MathJax-Span-89" class="texatom"><span id="MathJax-Span-90" class="mrow"><span id="MathJax-Span-91" class="mo">|</span></span></span><span id="MathJax-Span-92" class="mi">v</span><span id="MathJax-Span-93" class="texatom"><span id="MathJax-Span-94" class="mrow"><span id="MathJax-Span-95" class="mo">|</span></span></span></span><span id="MathJax-Span-96" class="mi">E</span></span><span id="MathJax-Span-97" class="mo">=</span><span id="MathJax-Span-98" class="mfrac"><span id="MathJax-Span-99" class="mrow"><span id="MathJax-Span-100" class="mi">e</span><span id="MathJax-Span-101" class="mi">E</span><span id="MathJax-Span-102" class="mi">τ</span></span><span id="MathJax-Span-103" class="mrow"><span id="MathJax-Span-104" class="mi">m</span><span id="MathJax-Span-105" class="mi">E</span></span></span><span id="MathJax-Span-106" class="mo">=</span><span id="MathJax-Span-107" class="mfrac"><span id="MathJax-Span-108" class="mrow"><span id="MathJax-Span-109" class="mi">e</span><span id="MathJax-Span-110" class="mi">τ</span></span><span id="MathJax-Span-111" class="mi">m</span></span></span></span></span></div>
The net result of all this maths is a reasonable approximation of the conductivity of a number of monovalent metals. At room temperature, by using the kinetic theory of gases to estimate the drift velocity, the Drude model gives <span class="greekSymbol">σ</span>  ~ 10<sup>6</sup> <span class="greekSymbol">Ω</span><sup>-1</sup> m<sup>-1</sup>. This is about the right order of magnitude for many monovalent metals, such as sodium (<em>σ</em>  ~ 2.13 <strong>×</strong> 10<sup>5</sup> <span class="greekSymbol">Ω</span><sup>-1</sup> m<sup>-1</sup>).

The Drude model can be visualised using the following simulation. With no applied field, it can be seen that the electrons move around randomly. Use the slider to apply a field, to see its effect on the movement of the electrons.

<object width="550" height="400" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,28,0"><embed src="http://www.doitpoms.ac.uk/tlplib/thermal_electrical/flash/part_sim_electron_a_2.swf" quality="high" pluginspage="http://www.adobe.com/shockwave/download/download.cgi?P1_Prod_Version=ShockwaveFlash" type="application/x-shockwave-flash" width="550" height="400" /></object>

<em>Note: This animation requires Adobe Flash Player 8 and later, which can be <a href="http://sdc.shockwave.com/shockwave/download/alternates/" target="_blank">downloaded here</a>.</em>

However, it is important to note that for non-metals, multivalent metals, and semiconductors, the Drude model fails miserably. To be able to predict the conductivity of these materials more accurately, quantum mechanical models such as the Nearly Free Electron Model are required. These are beyond the scope of this TLP

Superconductors are also not explained by such simple models, though more information can be found at the <a href="http://www.doitpoms.ac.uk/tlplib/superconductivity/index.php">Superconductivity TLP</a>.
<h2>Factors affecting electrical conduction</h2>
Electrical conduction in most metallic conductors (not semiconductors!) is straightforward to approximate. There are three important cases:
<h2>Pure and nearly pure metals</h2>
For pure metals at around room temperature, the resistivity depends linearly on temperature.
<div class="MathJax_Display"><span id="MathJax-Element-9-Frame" class="MathJax"><span id="MathJax-Span-112" class="math"><span id="MathJax-Span-113" class="mrow"><span id="MathJax-Span-114" class="msubsup"><span id="MathJax-Span-115" class="mi">ρ</span><span id="MathJax-Span-116" class="mn">2</span></span><span id="MathJax-Span-117" class="mo">=</span><span id="MathJax-Span-118" class="msubsup"><span id="MathJax-Span-119" class="mi">ρ</span><span id="MathJax-Span-120" class="mn">1</span></span><span id="MathJax-Span-121" class="mo">[</span><span id="MathJax-Span-122" class="mn">1</span><span id="MathJax-Span-123" class="mo">+</span><span id="MathJax-Span-124" class="mi">α</span><span id="MathJax-Span-125" class="mo">(</span><span id="MathJax-Span-126" class="msubsup"><span id="MathJax-Span-127" class="mi">T</span><span id="MathJax-Span-128" class="mn">2</span></span><span id="MathJax-Span-129" class="mo">−</span><span id="MathJax-Span-130" class="msubsup"><span id="MathJax-Span-131" class="mi">T</span><span id="MathJax-Span-132" class="mn">1</span></span><span id="MathJax-Span-133" class="mo">)</span><span id="MathJax-Span-134" class="mo">]</span></span></span></span></div>
However, at low temperatures, the conductivity ceases to be linear (superconductors are dealt with separately), and resistivity is related to temperature by Matthiesen’s rule:
<div class="MathJax_Display"><span id="MathJax-Element-10-Frame" class="MathJax"><span id="MathJax-Span-135" class="math"><span id="MathJax-Span-136" class="mrow"><span id="MathJax-Span-137" class="mi">ρ</span><span id="MathJax-Span-138" class="mo">(</span><span id="MathJax-Span-139" class="mi">T</span><span id="MathJax-Span-140" class="mo">)</span><span id="MathJax-Span-141" class="mo">=</span><span id="MathJax-Span-142" class="texatom"><span id="MathJax-Span-143" class="mrow"><span id="MathJax-Span-144" class="msubsup"><span id="MathJax-Span-145" class="mi">ρ</span><span id="MathJax-Span-146" class="texatom"><span id="MathJax-Span-147" class="mrow"><span id="MathJax-Span-148" class="texatom"><span id="MathJax-Span-149" class="mrow"><span id="MathJax-Span-150" class="texatom"><span id="MathJax-Span-151" class="mrow"><span id="MathJax-Span-152" class="mi">d</span><span id="MathJax-Span-153" class="mi">e</span><span id="MathJax-Span-154" class="mi">f</span><span id="MathJax-Span-155" class="mi">e</span><span id="MathJax-Span-156" class="mi">c</span><span id="MathJax-Span-157" class="mi">t</span></span></span></span></span></span></span></span></span></span><span id="MathJax-Span-158" class="mo">+</span><span id="MathJax-Span-159" class="texatom"><span id="MathJax-Span-160" class="mrow"><span id="MathJax-Span-161" class="msubsup"><span id="MathJax-Span-162" class="mi">ρ</span><span id="MathJax-Span-163" class="texatom"><span id="MathJax-Span-164" class="mrow"><span id="MathJax-Span-165" class="texatom"><span id="MathJax-Span-166" class="mrow"><span id="MathJax-Span-167" class="texatom"><span id="MathJax-Span-168" class="mrow"><span id="MathJax-Span-169" class="mi">t</span><span id="MathJax-Span-170" class="mi">h</span><span id="MathJax-Span-171" class="mi">e</span><span id="MathJax-Span-172" class="mi">r</span><span id="MathJax-Span-173" class="mi">m</span><span id="MathJax-Span-174" class="mi">a</span><span id="MathJax-Span-175" class="mi">l</span></span></span></span></span></span></span></span></span></span></span></span></span></div>
<img class="alignnone size-full wp-image-136" src="http://en.mekesim.com/wp-content/uploads/2016/01/matthiessens_1.png" alt="" width="396" height="250" />

The low temperature resistivity ( <span id="MathJax-Element-11-Frame" class="MathJax"><span id="MathJax-Span-176" class="math"><span id="MathJax-Span-177" class="mrow"><span id="MathJax-Span-178" class="texatom"><span id="MathJax-Span-179" class="mrow"><span id="MathJax-Span-180" class="msubsup"><span id="MathJax-Span-181" class="mi">ρ</span><span id="MathJax-Span-182" class="texatom"><span id="MathJax-Span-183" class="mrow"><span id="MathJax-Span-184" class="texatom"><span id="MathJax-Span-185" class="mrow"><span id="MathJax-Span-186" class="texatom"><span id="MathJax-Span-187" class="mrow"><span id="MathJax-Span-188" class="mi">d</span><span id="MathJax-Span-189" class="mi">e</span><span id="MathJax-Span-190" class="mi">f</span><span id="MathJax-Span-191" class="mi">e</span><span id="MathJax-Span-192" class="mi">c</span><span id="MathJax-Span-193" class="mi">t</span></span></span></span></span></span></span></span></span></span></span></span></span> )depends on the concentration of lattice defects, such as dislocations, grain boundaries, vacancies, and interstitial atoms. Consequently, it is lower in annealed, large crystal metal samples, and higher in alloys and work hardened metals. You might think that at higher temperatures the electrons would have more energy to be able to move through the material, so perhaps it is rather surprising that resistivity increases (and conductivity therefore decreases) as temperature increases. The reason for this is that as temperature increases, the electrons are scattered more frequently by lattice vibrations, or phonons, which causes the resistivity to increase. This contribution to the resistivity is described by <span class="greekSymbol">ρ</span><sub><strong>thermal</strong></sub>.

The temperature dependence of the conductivity of pure metals is illustrated schematically in the following simulation. Use the slider to vary the temperature, to see how the movement of the electrons through the lattice is affected. You can also introduce interstitial atoms by clicking within the lattice.

<object width="550" height="400" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,28,0"><embed src="http://www.doitpoms.ac.uk/tlplib/thermal_electrical/flash/part_sim_electron_b_2.swf" quality="high" pluginspage="http://www.adobe.com/shockwave/download/download.cgi?P1_Prod_Version=ShockwaveFlash" type="application/x-shockwave-flash" width="550" height="400" /></object>

<em>Note: This animation requires Adobe Flash Player 10 and later, which can be <a href="http://get.adobe.com/flashplayer/" target="_blank">downloaded here</a>.</em>
<h2>Alloys - Solid solution</h2>
As before, adding an impurity (in this case another element) decreases the conductivity. For a solid solution, the variation of resistivity with composition is given by Nordheim’s rule:
<div class="MathJax_Display"><span id="MathJax-Element-12-Frame" class="MathJax"><span id="MathJax-Span-194" class="math"><span id="MathJax-Span-195" class="mrow"><span id="MathJax-Span-196" class="mi">ρ</span><span id="MathJax-Span-197" class="mo">=</span><span id="MathJax-Span-198" class="msubsup"><span id="MathJax-Span-199" class="mi">χ</span><span id="MathJax-Span-200" class="texatom"><span id="MathJax-Span-201" class="mrow"><span id="MathJax-Span-202" class="mi">α</span></span></span></span><span id="MathJax-Span-203" class="msubsup"><span id="MathJax-Span-204" class="mi">ρ</span><span id="MathJax-Span-205" class="texatom"><span id="MathJax-Span-206" class="mrow"><span id="MathJax-Span-207" class="mi">α</span></span></span></span><span id="MathJax-Span-208" class="mo">+</span><span id="MathJax-Span-209" class="msubsup"><span id="MathJax-Span-210" class="mi">χ</span><span id="MathJax-Span-211" class="texatom"><span id="MathJax-Span-212" class="mrow"><span id="MathJax-Span-213" class="mi">β</span></span></span></span><span id="MathJax-Span-214" class="msubsup"><span id="MathJax-Span-215" class="mi">ρ</span><span id="MathJax-Span-216" class="texatom"><span id="MathJax-Span-217" class="mrow"><span id="MathJax-Span-218" class="mi">β</span></span></span></span><span id="MathJax-Span-219" class="mo">+</span><span id="MathJax-Span-220" class="mi">C</span><span id="MathJax-Span-221" class="msubsup"><span id="MathJax-Span-222" class="mi">χ</span><span id="MathJax-Span-223" class="texatom"><span id="MathJax-Span-224" class="mrow"><span id="MathJax-Span-225" class="mi">α</span></span></span></span><span id="MathJax-Span-226" class="msubsup"><span id="MathJax-Span-227" class="mi">χ</span><span id="MathJax-Span-228" class="texatom"><span id="MathJax-Span-229" class="mrow"><span id="MathJax-Span-230" class="mi">β</span></span></span></span></span></span></span></div>
where <span class="variable">C</span> is a constant and <span class="variable">C</span>A and <span class="variable">C</span>B are the atomic fractions of the metals A and B, whose resistivities are <span class="greekSymbol">ρ</span>A and <span class="greekSymbol">ρ</span>B respectively.

Further, the difference in valency between the bulk lattice and the impurity atoms is proportional to the difference in resistivity -  Linde’s rule.
<div class="MathJax_Display"><span id="MathJax-Element-13-Frame" class="MathJax"><span id="MathJax-Span-231" class="math"><span id="MathJax-Span-232" class="mrow"><span id="MathJax-Span-233" class="mi">Δ</span><span id="MathJax-Span-234" class="mi">ρ</span><span id="MathJax-Span-235" class="mo">∝</span><span id="MathJax-Span-236" class="mo">(</span><span id="MathJax-Span-237" class="mi">Δ</span><span id="MathJax-Span-238" class="mi">Z</span><span id="MathJax-Span-239" class="msubsup"><span id="MathJax-Span-240" class="mo">)</span><span id="MathJax-Span-241" class="mn">2</span></span></span></span></span></div>
where ΔZ is the difference in valence between the solute and the solvent.

Thus, solute atoms with a higher (or lower) charge than the lattice will have a greater effect on the resistivity.
<h2>Alloys- many phases</h2>
For an alloy where there are two or more distinct phases, the contributions simply contribute linearly to the total resistivity (though the effect of  many grain boundaries increases resistivity slightly).
<div class="MathJax_Display"><span id="MathJax-Element-14-Frame" class="MathJax"><span id="MathJax-Span-242" class="math"><span id="MathJax-Span-243" class="mrow"><span id="MathJax-Span-244" class="mi">ρ</span><span id="MathJax-Span-245" class="mo">=</span><span id="MathJax-Span-246" class="msubsup"><span id="MathJax-Span-247" class="mi">χ</span><span id="MathJax-Span-248" class="mi">α</span></span><span id="MathJax-Span-249" class="msubsup"><span id="MathJax-Span-250" class="mi">ρ</span><span id="MathJax-Span-251" class="mi">α</span></span><span id="MathJax-Span-252" class="mo">+</span><span id="MathJax-Span-253" class="msubsup"><span id="MathJax-Span-254" class="mi">χ</span><span id="MathJax-Span-255" class="mi">β</span></span><span id="MathJax-Span-256" class="msubsup"><span id="MathJax-Span-257" class="mi">ρ</span><span id="MathJax-Span-258" class="mi">β</span></span></span></span></span></div>
The following animation illustrates Mattheisen’s rule, Nordheim’s rule and the mixture rule.

<object width="550" height="400" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,28,0"><embed src="http://www.doitpoms.ac.uk/tlplib/thermal_electrical/flash/Phase_scroller_4.swf" quality="high" pluginspage="http://www.adobe.com/shockwave/download/download.cgi?P1_Prod_Version=ShockwaveFlash" type="application/x-shockwave-flash" width="550" height="400" /></object>

<em>Note: This animation requires Adobe Flash Player 8 and later, which can be <a href="http://sdc.shockwave.com/shockwave/download/alternates/" target="_blank">downloaded here</a>.</em>
<h2>Thermal conduction metals</h2>
Metals typically have a relatively high concentration of free conduction electrons, and these can transfer heat as they move through the lattice. Phonon-based conduction also occurs, but the effect is swamped by that of electronic conduction.

The following simulation shows how electrons can conduct heat by colliding with the nuclei and transferring thermal energy. Click the “source” button to apply a heat source to one side of the sample. The graph will show the thermal gradient within the sample, and you can also apply a heat sink to the opposite side of the sample using the “sink” button.

<object width="550" height="400" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,28,0"><embed src="http://www.doitpoms.ac.uk/tlplib/thermal_electrical/flash/part_sim_heat_a_3.swf" quality="high" pluginspage="http://www.adobe.com/shockwave/download/download.cgi?P1_Prod_Version=ShockwaveFlash" type="application/x-shockwave-flash" width="550" height="400" /></object>

<em>Note: This animation requires Adobe Flash Player 10 and later, which can be <a href="http://get.adobe.com/flashplayer/" target="_blank">downloaded here</a>.</em>
<h2>Wiedemann-Franz law</h2>
Since the dominant method of conduction is the same in metals for thermal and electrical conduction (i.e. electrons!), it makes sense that there is a relationship between the two conductivities.

The <strong>Wiedemann-Franz law</strong> states that the ratio of thermal conductivity to the electrical conductivity of a metal is proportional to its temperature.
<div class="MathJax_Display"><span id="MathJax-Element-15-Frame" class="MathJax"><span id="MathJax-Span-259" class="math"><span id="MathJax-Span-260" class="mrow"><span id="MathJax-Span-261" class="mi">L</span><span id="MathJax-Span-262" class="mi">T</span><span id="MathJax-Span-263" class="mo">=</span><span id="MathJax-Span-264" class="mfrac"><span id="MathJax-Span-265" class="mi">κ</span><span id="MathJax-Span-266" class="mi">σ</span></span></span></span></span></div>
Where <span class="variable">L</span> the proportionality constant (also known as the Lorenz number), is:
<div class="MathJax_Display"><span id="MathJax-Element-16-Frame" class="MathJax"><span id="MathJax-Span-267" class="math"><span id="MathJax-Span-268" class="mrow"><span id="MathJax-Span-269" class="mi">L</span><span id="MathJax-Span-270" class="mo">=</span><span id="MathJax-Span-271" class="mfrac"><span id="MathJax-Span-272" class="mi">κ</span><span id="MathJax-Span-273" class="texatom"><span id="MathJax-Span-274" class="mrow"><span id="MathJax-Span-275" class="mi">σ</span><span id="MathJax-Span-276" class="mi">T</span></span></span></span><span id="MathJax-Span-277" class="mo">=</span><span id="MathJax-Span-278" class="mn">2.45</span><span id="MathJax-Span-279" class="mo">×</span><span id="MathJax-Span-280" class="texatom"><span id="MathJax-Span-281" class="mrow"><span id="MathJax-Span-282" class="msubsup"><span id="MathJax-Span-283" class="mn">10</span><span id="MathJax-Span-284" class="texatom"><span id="MathJax-Span-285" class="mrow"><span id="MathJax-Span-286" class="mo">−</span><span id="MathJax-Span-287" class="mn">8</span></span></span></span></span></span><span id="MathJax-Span-288" class="mi">W</span><span id="MathJax-Span-289" class="mi">Ω</span><span id="MathJax-Span-290" class="texatom"><span id="MathJax-Span-291" class="mrow"><span id="MathJax-Span-292" class="msubsup"><span id="MathJax-Span-293" class="mi">K</span><span id="MathJax-Span-294" class="texatom"><span id="MathJax-Span-295" class="mrow"><span id="MathJax-Span-296" class="mo">−</span><span id="MathJax-Span-297" class="mn">2</span></span></span></span></span></span></span></span></span></div>
The law can be explained by the fact that free electrons in the metal are involved in the mechanisms in both heat and electrical transport. The thermal conductivity increases with the average electron velocity since this increases the forward transport of energy. However, the electrical conductivity decreases with an increase in particle velocity because the collisions divert the electrons from forward transport of charge.

<img class="alignnone size-full wp-image-137" src="http://en.mekesim.com/wp-content/uploads/2016/01/weidemann_graph.png" alt="Wiederman graph" width="624" height="420" />
<h2>Electrical conduction: non metals</h2>
Although the drude model works reasonably well for monovalent metals, it does not predict the properties of semiconductors, superconductors, or non-metallic conductors.

<a href="http://www.doitpoms.ac.uk/tlplib/superconductivity/index.php" target="_blank">Superconductors</a>  and <a href="http://www.doitpoms.ac.uk/tlplib/semiconductors/index.php" target="_blank">Semiconductors</a> are best explained in their own TLPs.
<h2>Ionic conduction</h2>
For certain materials, there is no net movement of electrons, yet they still conduct electricity.

The mechanism is that of ionic conduction, whereby some charged ions can move through the bulk lattice (by the usual diffusion mechanisms, except with an electric field driving force).

Such ionic conductors are used in solid oxide fuel cells – though for the example of yttria stabilised zirconia (YZT), operational temperatures are between 500 and 1000 degrees C. Because they conduct by a diffusion like mechanism, higher temperatures lead to higher conductivity, the reverse of what the simple Drude model would predict.
<h2>Breakdown voltage</h2>
There is an important, and potentially lethal mechanism by which an insulator can become conductive. In air, it may be commonly recognised as lightning. Of note is that the mechanism can ionise the ‘insulator’, leaving it temporarily more conductive..

Gases are commonly ionised in domestic lighting devices. The most common are fluorescent tubes and neon lights.

To initially excite the mercury vapour in a fluorescent tube type light, a voltage spike exceeding the breakdown voltage is needed. This can be noticed when switching such a light on as a sudden ignition, with an associated radio interference spike. A faulty tube may not fully ionise, leading to only a small glow at the ends.

<img class="alignnone size-full wp-image-138" src="http://en.mekesim.com/wp-content/uploads/2016/01/breakdown.jpg" alt="" width="564" height="655" />
<p class="caption">Under high voltages, even plexiglass may conduct. The temporarily ionised path is opaque on cooling, giving a Lichtenberg figure in this case. <em>Image “Lichtenberg figure” by </em><em>Bert Hickman</em></p>
More information is available in the <a href="http://www.doitpoms.ac.uk/tlplib/dielectrics2/breakdown.php">Dielectrics TLP page on breakdown</a>
<h2>Non-metals: thermal phonons</h2>
As mentioned previously, metals have two modes of thermal conduction: electron based and phonon based. For non metals, there are relatively few free electrons, so the phonon method dominates.

Heat can be thought of as a measure of the energy in the vibrations of atoms in a material. As with all things on the atomic scale, there are quantum mechanical considerations; the energy of each vibration is quantised (and proportional to the frequency). A phonon is a quantum of vibrational energy, and by the combination (superposition) of many phonons, heat is observed macroscopically.

The energy of a given lattice vibration in a rigid crystal lattice is quantised into a quasiparticle called a <strong>phonon</strong>. This is analogous to a photon in an electromagnetic wave; thermal vibrations in crystals can be described as thermally excited phonons, which can be related to thermally excited photons. Phonons are a major factor governing the electrical and thermal conductivities of a material.

A phonon is a quantum mechanical adaptation of normal modal vibration in classical mechanics. A key property of phonons is that of wave-particle duality; normal modes have wave-like phenomena in classical mechanics but gain particle-like behaviour under quantum mechanics.

The energy of a phonon is proportional to its angular frequency <span class="greekSymbol">ω</span>:
<div class="MathJax_Display"><span id="MathJax-Element-17-Frame" class="MathJax"><span id="MathJax-Span-298" class="math"><span id="MathJax-Span-299" class="mrow"><span id="MathJax-Span-300" class="mi">ε</span><span id="MathJax-Span-301" class="mo">=</span><span id="MathJax-Span-302" class="mo">(</span><span id="MathJax-Span-303" class="mi">n</span><span id="MathJax-Span-304" class="mo">+</span><span id="MathJax-Span-305" class="mfrac"><span id="MathJax-Span-306" class="mn">1</span><span id="MathJax-Span-307" class="mn">2</span></span><span id="MathJax-Span-308" class="mo">)</span><span id="MathJax-Span-309" class="mi">ℏ</span><span id="MathJax-Span-310" class="mi">ω</span></span></span></span></div>
with quantum number <em>n</em>. The term <span id="MathJax-Element-18-Frame" class="MathJax"><span id="MathJax-Span-311" class="math"><span id="MathJax-Span-312" class="mrow"><span id="MathJax-Span-313" class="mfrac"><span id="MathJax-Span-314" class="mn">1</span><span id="MathJax-Span-315" class="mn">2</span></span><span id="MathJax-Span-316" class="mi">ℏ</span><span id="MathJax-Span-317" class="mi">ω</span></span></span></span> is the zero point energy of the mode. This is defined as the lowest possible energy that the system possesses and is the energy of the ground state.

If a solid has more than one type of atom in the unit cell, there will be two possible types of phonons: “acoustic” and “optical” phonons. The frequency of acoustic phonons is around that of sound, and for optical phonons, close to that of infrared light. They are referred to as optical because in ionic crystals they are excited easily by electromagnetic radiation.

If a crystal lattice is at zero temperature, it lies in its ground state, and contains no phonons. When the lattice is heated to and held at a non-zero temperature, its energy is not constant, but fluctuates randomly about some mean value. These energy fluctuations are caused by random lattice vibrations, which can be viewed as a gas of phonons. Because the temperature of the lattice generates these phonons, they are sometimes referred to as <strong>thermal phonons</strong>. Thermal phonons can be created or destroyed by random energy fluctuations.

It is accepted that phonons also have momentum, and therefore can conduct energy through the lattice. Unlike electrons, there is a net movement of phonons - from the hotter to the cooler part of the lattice, where they are destroyed. Electrons must maintain charge neutrality in the lattice, so there is no net movement of electrons during thermal conduction.

The following simulation shows schematic optical and acoustic phonons in a 2D lattice, and has the option to animate a 2D wavevector defined by clicking inside the green box.

<object width="550" height="400" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,28,0"><embed src="http://www.doitpoms.ac.uk/tlplib/thermal_electrical/flash/Part_sim_Phonons_3.swf" quality="high" pluginspage="http://www.adobe.com/shockwave/download/download.cgi?P1_Prod_Version=ShockwaveFlash" type="application/x-shockwave-flash" width="550" height="400" /></object>

<em>Note: This animation requires Adobe Flash Player 10 and later, which can be <a href="http://get.adobe.com/flashplayer/" target="_blank">downloaded here</a>.</em>
<h2>Umklapp scattering</h2>
When two phonons collide, the resulting phonon has the vector sum of their momenta. The way of treating particles moving in a lattice quantum mechanically under the reduced zone scheme (which is beyond the scope of this TLP but is explored in more depth in the <a href="http://www.doitpoms.ac.uk/tlplib/semiconductors/index.php%3EIntroduction%20to%20semiconductors" target="_blank">Brillouin Zones</a> TLP), leads to a conceptually strange effect. If the momentum is too great (outside the first Brillouin zone) then the resulting phonon moves in almost the opposite direction. This is <strong>Umklapp scattering</strong>, and is dominant at higher temperatures- acting to reduce thermal conductivity as the temperature increases.

<img class="alignnone size-full wp-image-139" src="http://en.mekesim.com/wp-content/uploads/2016/01/umklapp.png" alt="Diagram showing umklapp scattering" width="784" height="396" />
<h2>Applications</h2>
<h2>Silicon chips</h2>
As electrical properties vary with microstructure, a type of computer memory called phase-change random-access memory (PC-RAM) has been developed. The material used is a chalcogenide reffered to as GST (Ge<sub>2</sub>Sb<sub>2</sub>Te<sub>5</sub>).

The amorphous state is semiconducting, while in a (poly)crystalline form it is metallic. Heating above the glass transition, but below the melting point, crystallises a previously semiconducting amorphous cell. Likewise, fully melting, then rapidly cooling a cell leaves it in the metallic crystalline state.

This variation of resistivity with microstructure is crucial to the operation of such devices. By varying the heating conditions, a varying proportion of each GST cell may be crystalline and amorphous - the mixture rule applies as it’s effectively two phases. This allows for multiple distinguishable levels of resistance per cell, increasing the storage density, and reducing the cost per megabyte.

<img class="alignnone size-full wp-image-140" src="http://en.mekesim.com/wp-content/uploads/2016/01/pram.jpg" alt="" width="492" height="327" />

The more common problem with silicon devices is dissipating heat.

A modern processor has a thermal design power of above 70w (Intel i7 3770, 22 nm process). A cooler must dissipate that specified amount of heat from the die’s surface, which is typically less than 10 cm<sup>2</sup>. It is common for heat sinks to have a copper block attached to the microprocessor casing by thermal paste, and pressure. The bulk of the heat sink is usually made from much cheaper aluminium, though the high thermal conductivity of copper is necessary for the interface. Thermal paste, whilst a better thermal conductor than air, is much worse than most metals, so it is only used as a thin layer to replace air gaps.

<img class="alignnone size-full wp-image-141" src="http://en.mekesim.com/wp-content/uploads/2016/01/heatsink.jpg" alt="" width="385" height="273" />

Conduction is not the most efficient method to carry heat to a separate heat sink, so convection and the latent heat of evaporation can be used. Heat pipes, typically made from copper are filled with a low boiling point liquid, which boils at the hot end, and condenses at the cool end of the pipe. This is a much faster way of transferring heat over longer distances.
<h2>Space</h2>
There are many applications of thermal insulators, with development coming from attempts to improve bulk mechanical properties, while retaining insulating properties, (i.e. Don’t let heat through, but don’t melt)

A particularly famous application of thermal insulation is the (now retired) space shuttle tiles which are responsible for protecting the shuttle during re-entry into the atmosphere. They are such good insulators, that the outside may glow red-hot, while inside the shuttle the astronauts are still alive.

One of the best thermal insulators is silica aerogel.

An aerogel is an extremely low-density solid-state material made from a gel where the liquid phase of the gel has been replaced with gas. The result is an extremely low density solid, which makes it effective as a thermal insulator.

One use of aerogels is for a lightweight micrometeorite collector, aerogel was used. While extremely light, it is strong enough to capture micrometeors.

<img class="alignnone size-full wp-image-142" src="http://en.mekesim.com/wp-content/uploads/2016/01/aerogel.jpg" alt="Image showing aerogel in use" width="900" height="430" />
<p class="caption">Matches stay cool millimetres from a blowtorch, a large array of aerogel bricks is ready to be launched into space, and the resulting space dust is photographed upon return to earth</p>
Aerogels can be made from a variety of materials, but share a universal structure style. (amorphous, open-celled “nanofoams”). However, a common material used is silicate. Silica aerogels were first discovered in 1931.

Aerogels have extreme structures and extreme physical properties. The highly porous nature of an aerogel structure provides a low density. The percentage of open space within an aerogel structure is about 94% for a gel with a density of 100 kg m<sup>-</sup><sup>3</sup>.

Aerogels are good thermal insulators because they eliminate the three methods of heat transfer (convection, conduction and radiation). They are good convective insulators due to the fact that air cannot circulate throughout the lattice. Silica aerogel is an especially good conductive insulator because silica is a poor conductor of heat - a metallic aerogel, on the other hand, would be a less effective insulator. Carbon aerogel is an effective radiative insulator because carbon is able to absorb the infrared radiation that transfers heat. Hence, for maximum thermal insulation, the best aerogel is silica doped with carbon.
<h2>Power transmission</h2>
One of the largest scale uses of electrical conductors is in power transmission.

Unfortunately, the properties that are desirable for a strong cable seem opposed to those for a good conductor.

Aluminium alloys can be very strong for their density, but following Nordheim’s rule, are much poorer conductors.

There are a huge variety of steels, but again, the interstitial carbon atoms increase the resistance compared to pure iron. This means that a larger diameter cable is needed, which, due to the density of steel, ends up being very heavy and expensive. Heavier cable also means we must construct additional pylons, which is a large component of the cost.

Copper, while appropriate for home wiring, is dense, and increasingly expensive.

<object width="550" height="400" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,28,0"><embed src="http://www.doitpoms.ac.uk/tlplib/thermal_electrical/flash/Powerlines_thing_4.swf" quality="high" pluginspage="http://www.adobe.com/shockwave/download/download.cgi?P1_Prod_Version=ShockwaveFlash" type="application/x-shockwave-flash" width="550" height="400" /></object>

<em>Note: This animation requires Adobe Flash Player 10 and later, which can be <a href="http://get.adobe.com/flashplayer/" target="_blank">downloaded here</a>.</em>

For most overhead power cables, the solution is to use two materials – a steel core, surrounded by many individual aluminium cores. This achieves light, high strength, and acceptable conductivity cables.

Superconductors have been trialled for power transmission, though only underground, and at a considerably higher cost (and efficiency!).
<h2>Thermoelectric effect</h2>
The thermoelectric effect is the direct conversion of a difference in temperature into electric voltage and vice versa. Simply put, a thermoelectric device creates a voltage when there is a different temperature on each side of the device. It can also be run “backwards”, so when a voltage is applied across it, a temperature difference is created. This effect can be used to generate electricity, to measure temperature, to cool objects, or to heat them. Because the sign of the applied voltage determines the direction of heating and cooling, thermoelectric devices make very convenient temperature controllers.

The Peltier effect is that when a (direct) current flows through a metal-semiconductor junction, and heat is either absorbed or released. This is because the average energy of electrons in the two materials is different, and heat makes up this difference.

A fuller understanding requires knowledge of the band structure, explored further in the <a href="http://www.doitpoms.ac.uk/tlplib/semiconductors/index.php" target="_blank">TLP on Semiconductors</a>.

<object width="640" height="480" classid="clsid:D27CDB6E-AE6D-11cf-96B8-444553540000" codebase="http://download.macromedia.com/pub/shockwave/cabs/flash/swflash.cab#version=9,0,28,0"><embed src="http://www.doitpoms.ac.uk/tlplib/thermal_electrical/flash/peltier_1.swf" quality="high" pluginspage="http://www.adobe.com/shockwave/download/download.cgi?P1_Prod_Version=ShockwaveFlash" type="application/x-shockwave-flash" width="640" height="480" /></object>

<em>Note: This animation requires Adobe Flash Player 10 and later, which can be <a href="http://get.adobe.com/flashplayer/" target="_blank">downloaded here</a>.</em>
<h2>Summary</h2>
We have now gone over the foundation behind electrical and thermal conduction, as well as some of the more common applications. You should understand the role of electrons and phonons in thermal conduction, as well as how the interactions between them lead to changes in electrical conductivity with temperature. You should appreciate that metals have more heat transfer mechanisms than their non-metal counterparts, therefore explaining why they have higher thermal conductivity. Also, this TLP should have touched on some of the major applications of thermal and electrical conductors and insulators. Finally, the connections between thermal and electrical conductivity in metals have been made, including the Wiedemann-Franz Law.

To summarise the factors affecting conductivity:
<ul type="disc">
	<li>Temperature – as temperature increases, the average energy per phonon increases, and by the umklapp scattering mechanism, thermal conductivity is decreased. Phonons also scatter electrons more.</li>
</ul>
<ul type="disc">
	<li>Electron density (in metals) – if electrons are the conductors, more (valence) electrons usually leads to better conduction.</li>
</ul>
<ul type="disc">
	<li>Alloying – interstitials scatter electrons, and decrease conductivity. Phase boundaries, impurities, dislocations, etc. decrease conductivity, even at low temperature.</li>
</ul>