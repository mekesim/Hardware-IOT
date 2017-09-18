---
ID: 168
post_title: >
  MIT Cracks Nanoscale Heat Transfer
  Calculations
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/168
published: true
post_date: 2016-01-31 18:57:41
---
<h1>Heat Transfer at the Nanoscale Can Be Characterized</h1>
<div>

<img class="alignnone size-full wp-image-169" src="http://en.mekesim.com/wp-content/uploads/2016/01/MIT-Nano-Heat_0_qmohza.jpg" width="350" height="233" alt="MIT researchers crack heat flow on the nanoscale. Image courtesy of MIT News." />

MIT researchers crack heat flow on the nanoscale. Image courtesy of MIT News.

</div>
Engineers have a tough time determining the interactions between the nanoscale and macroscale.

Take radiative heat transfer, for example. We have derived equations and simulations so well that we can optimize our designs before building a prototype. However, optimizing this same interaction on the nanoscale, 10<sup>-9</sup>m, is a lot more elusive.

That is, until MIT researchers derived a formula that can determine the maximum heat transfer between two objects that are less than eight microns (10<sup>-6</sup> m) apart, even on the nanoscale. MIT reports that as long as the material of the objects and the distance between them is known, the formula can calculate the maximum heat that can be passed between these objects.

“Our work is not a new model, but is instead a new <em>bound</em>, or <em>limit</em>, on how much power can be exchanged in the heat-transfer process,” said Owen Miller, a postdoc in the MIT Department of Mathematics. “The relevant comparisons are to Planck's Law and the Stefan-Boltzmann Limit.”

The initial findings suggest that optimizations made with this new equation can improve nanoscale heat transfer calculation accuracy by orders of magnitude.
<h1>How Do You Fix the Stefan-Boltzmann Equation for the Nanoscale</h1>
Typically, engineers have used the Stefan-Boltzmann equation to determine the theoretical maximum heat transfer between two distant objects. However, this equation assumes the objects are black bodies that absorb all of the heat radiating toward them and that they are at a distance further than the wavelength of the heat energy. As a result, when objects are extremely close, at about eight microns or less, the Stefan-Boltzmann equation severely underestimates the heat transfer capabilities of the black body objects.

This underestimation is attributed to evanescent waves. Since these evanescent waves dissipate quickly, they have little effect on the macro scale where electromagnetics dominate. However, if the objects are close enough, these evanescent waves can tunnel energy transfer between the objects. This level of heat transfer has only recently been characterized on the nanoscale.

To solve this issue, Miller and his team derived a formula that describes the heat transfer as electrical currents flowing through the bodies caused by each body’s electric dipoles. Using energy conservation, they were able to discover the following equation:
<div align="center">

<img class="alignnone size-full wp-image-170" src="http://en.mekesim.com/wp-content/uploads/2016/01/drawing_nontransparent_hjptlh.jpg" width="640" height="334" alt="Comparison of Stefan-Boltzmann and MIT’s new equation. A is the cross sectional area, d is the distance between the objects, T is the temperature of the hotter object (assuming large temperature differences), λ is the wavelength at T, σ is the Stefan-Boltzmann constant and χ is a material-specific constant, “susceptibilities.”" />
<div>Comparison of Stefan-Boltzmann and MIT’s new equation. A is the cross sectional area, d is the distance between the objects, T is the temperature of the hotter object (assuming large temperature differences), λ is the wavelength at T, σ is the Stefan-Boltzmann constant and χ is a material-specific constant, “susceptibilities.”</div>
</div>
“The equation on the left is Stefan-Boltzmann, while ours is on the right,” said Miller, in referencing the image above. “You will notice two extra terms, dependent on the spacing ‘<em>d’ </em>between the two bodies and the material susceptibilities ‘<em>χ</em>.’ The first term arises from a larger ‘available energy,’ when two bodies are close, while the second represents resonant amplification, i.e. ability to excite a large current with just a little energy (analogous to wine-glass amplification of a vibration).”

This simple equation can be applied to various shapes. With only the distance between the objects and a material constant that depicts the amount of electric current the object can build up, they are able to characterize the heat transfer.

“Now we have a formula for the upper bound,” said Steven Johnson, professor of applied mathematics at MIT. “Given the material and the separation you want, you’d just plug it into the formula and boom, you’re done — it’s very easy. Now you can go backwards and try to play with materials and optimize them.”
<h1>Why Is Nanoscale Heat Transfer Useful?</h1>
Using this formula, engineers will be able to better characterize, understand, and optimize the heat transfer between two objects that are close together. Some product examples include the cooling of computer chips and thermophotovoltaics that convert heat into electricity.

In fact, the team at MIT has tested that the heat transfer in these objects can be improved by orders of magnitude when using their model.

“This [formula] provides a target to say, ‘this is what we should be looking for,’ and, compared to what we’ve seen so far in simple structures, there’s orders of magnitude more room for improvement for this kind of heat transfer,” says Miller. “If that’s practically achievable, that could make a huge difference in, for example, thermophotovoltaics.”

Johnson explained that this formula will be able to help engineers determine the best orientation and materials to optimize their designs for heat transfer at the nanoscale. For example, engineers will be able to better design the etching in thermophotovoltaics, which will improve heat transfer capabilities.

However, there will be some time before simulation software like ANSYS, Abaqus, and COMSOL are using this equation to optimize these nanoscale heat transfer systems.

“This is still ongoing work, but aluminum looks like it has a lot of potential if it can be designed properly,” Miller says. “It has to be designed properly in order to achieve the limit, which is why people haven’t seen large enhancements with such materials before, but this really opens up a new class of materials that may be used.”

Miller added that, “Many electromagnetic simulation tools, commercial — ANSYS, COMSOL, Lumerical FDTD Solutions) — and open-source — meep, scuff-em, etc. — can, in fact, already compute radiative heat transfer. At the moment, it is very computationally expensive to do so, but as this gets faster, we will certainly see optimization efforts to try to reach our limits. An ideal approach would be topology optimization.”