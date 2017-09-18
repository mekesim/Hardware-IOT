---
ID: 287
post_title: >
  THERMAL DESIGN EXPLORATION FOR THE OPEN
  COMPUTE PROJECT
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/287
published: true
post_date: 2016-03-10 16:25:36
---
By Tom Gregory
<div class="sharethis-buttons">
<div class="sharethis-wrapper">
<div id="___plusone_0"></div>
</div>
</div>
<div class="field field-name-field-image field-type-image field-label-hidden">
<div class="field-items">
<div class="field-item even"><img class="alignnone size-full wp-image-288" src="http://www.mekesim.com/wp-content/uploads/2016/03/2016-01-06-jh-signaopen1.jpg" width="595" height="373" alt="" /></div>
</div>
</div>
<div class="field field-name-field-header field-type-text-long field-label-hidden">
<div class="field-items">
<div class="field-item even">The Open Compute Project Foundation is tackling a big challenge: how to scale computing infrastructure in the most efficient and economical way possible.</div>
</div>
</div>
<div class="field field-name-body field-type-text-with-summary field-label-hidden">
<div class="field-items">
<div class="field-item even">

The Foundation, founded by Facebook, is fostering a rapidly growing community of engineers around the world whose mission is to design and enable the delivery of the most efficient server, storage and data centre hardware designs for scalable computing.

To achieve this aim the Open Compute Project Foundation provides a structure in which individuals and organisations can share their intellectual property with Open Compute Projects.

The University of Texas at Arlington (UTA) is one such organisation that is involved in the Open Compute Project. UTA wanted to investigate new cooling strategies to improve the thermal design of the Open Compute Project's Intel-based servers. To assist this work the team at UTA turned to thermal simulation to help find a solution.

Two different methods were chosen to improve the server’s thermal design: one improved the ducting inside the server, while the other utilised warm water cooling. To assess these options UTA used the 6SigmaET software throughout their project to create, simulate and fine-tune their proposed solutions to the server’s thermal design issues.

<strong>Solution 1: Improved Ducting</strong>

The first server had a removable chassis cover with an integrated air ducting system. However, this ducting was only provided in the CPU1 region: this caused excessive flow bypass in the CPU0 region, resulting in warm air entering heat sink 1. The university decided to investigate whether modifications to the server’s ducting system would improve its thermal performance.

Physical experiments were conducted on the server to determine its system impedance, flow rates, total server power consumption, fan speeds and fan power consumption at various power levels. This experimental data was used to generate and calibrate a detailed CFD model of the server using 6SigmaET. It was solved using the KE turbulence model, and the CFD model was matched with the temperatures obtained from testing. The CFD model and experimental data showed good agreement (see figure 1), with a maximum error of 12%.

<img class="alignnone size-full wp-image-289" src="http://www.mekesim.com/wp-content/uploads/2016/03/2016-01-06-jh-signaopenfig1.jpg" width="622" height="474" alt="" />
<h6 class="Legend">Fig. 1: Comparison of experimental temperature results and CFD temperature results for CPU0</h6>
&nbsp;

The university then used 6SigmaET to improve the server’s ducting system parametrically. The key goal was to reduce flow bypass in the CPU0 region without causing a temperature rise in the CPU1 region (and an increase in fan power, which would increase total server power consumption). The calibrated CFD model was used to parameterize the size and location of the duct, and solved for each new design iteration to determine how the processor temperatures would be affected in each case. This process led to a final design for the improved ducting system. This design was prototyped, then tested in the same way as the original server.

<img class="alignnone size-full wp-image-290" src="http://www.mekesim.com/wp-content/uploads/2016/03/2016-01-06-jh-signaopenfig2.jpg" width="918" height="356" alt="" />
<h6 class="Legend"><span class="newsletter4">Fig. 2: Temperature plots of the original server (top) and the server with improved ducting (bottom).</span></h6>
&nbsp;

The test results were positive: fan power consumption was reduced by 23.4-40%, fan speeds by 22-26% and flow rate by 31.3-37.3%, while the server’s temperature stayed within the recommended range (see figure 2).

<strong>Solution 2: Liquid Cooling</strong>

The university then investigated whether a liquid-cooled system would improve the server’s thermal performance. To achieve a completely liquid-cooled system, the air-cooled heat sinks were replaced with liquid-cooled cold plates and the system was sealed from the ambient air to prevent gaseous and component contamination.

A heat exchanger was incorporated to cool the air inside the server, as the remaining components are not directly liquid cooled. A combination of warm water and recirculated air would be used to cool the server. This solution required custom ducting to direct the recirculated air over the server’s DIMMs (dual in-line memory modules), PCH (Platform Controller Hub), hard drive (HDD) and other heat generating components.

A range of candidate ducts were designed, with the goal of ensuring adequate airflow through the system and keeping component temperatures within the server’s critical limits. These designs were modelled and simulated in 6SigmaET, and the results used to determine the optimum duct design.

A prototype was created from this design, which was then subjected to thermal testing. It was tested with water inlet temperatures from 27.5-45°C in increments of 2.5°C. The server was exercised computationally at idle, 40%, 60%, 80% and 100% CPU loading, and one test was performed with maximum CPU and memory power levels to provide continuous heat dissipation.

<img class="alignnone size-full wp-image-291" src="http://www.mekesim.com/wp-content/uploads/2016/03/2016-01-06-jh-signaopenfig3.jpg" width="1216" height="259" alt="" />
<h6 class="Legend">Fig. 3: CFD simulation showing airflow velocity through the improved system.</h6>
&nbsp;

The thermal testing results showed a correlation between the server’s performance and the increased water inlet temperatures. The server’s cooling power consumption, radiator fan speeds, CPU temperatures and IT power consumption increased as the water temperature increased. However, the CPU temperatures remained below the critical die temperature of 80°C throughout the experiment.

The prototyped duct regulated the air flow through the DIMMs, HDD and other auxiliary components as expected, maintaining component temperatures below critical. The university concluded that there was ample incentive to operate at higher water temperatures, up to 45°C.

<img class="alignnone size-full wp-image-292" src="http://www.mekesim.com/wp-content/uploads/2016/03/2016-01-06-jh-signaopenfig4.jpg" width="628" height="478" alt="" />
<h6 class="Legend">Fig. 4: DIMM temperatures from experimental tests. A4-A7 are closer to the internal radiator fan. A0-A3 are further from the fan, and are affected by pre-heat from the other DIMMS. The modified design maintains component temperatures below critical, up to 45°C</h6>
&nbsp;

<strong>Conclusions</strong>

Both projects used thermal simulation to analyse airflow and temperatures in the original server and determine where improvements could be made. This allowed the university to create and test a range of designs, iteratively improve them, and determine which performed best. The design with the best results was then prototyped and physically tested, with good agreement between the CFD model and the experimental results. Thermal simulation using 6SigmaET reduced the time and cost of the design stage, and meant that a wide range of potential solutions could be investigated.

This case study gives a perfect demonstration of how thermal simulations give engineers a unique visual representation of the temperature and airflow inside equipment. This insight allows them to make better engineering decisions. Even in the context of a global mission like the Open Compute Project, these details matter and can make a big difference.

<strong>About the author:</strong>

Tom Gregory is 6SigmaET Product Specialist at Future Facilities -http://www.6sigmaet.info/

</div>
</div>
</div>