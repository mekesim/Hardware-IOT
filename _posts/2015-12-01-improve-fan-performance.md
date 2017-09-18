---
ID: 53
post_title: >
  Improve fan performance and lower
  downtime
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/53
published: true
post_date: 2015-12-01 02:33:43
---
<h5>By Oreste "Rusty" Scioscia Jr.</h5>
<div>
<div>
<h3>Fast Forward</h3>
<ul>
	<li>Understand how drives work to improve energy efficiency and optimize system performance.</li>
	<li>Control motor speed and reduce your utility bill.</li>
	<li>Adjustable frequency drives net significant energy savings and cut downtime.</li>
</ul>
</div>
</div>
"Approximately one-third of total U.S. delivered energy in 2012, 23.6 quadrillion Btu [British thermal units], was consumed in the industrial sector, which includes manufacturing, agriculture, construction, and mining," according to the U.S. Energy Information Administration. To put this in perspective, the average annual energy consumption for a U.S. household is roughly 10.8 megawatt hours (MWh) of energy. If the total U.S. power consumption for 2012 were split up among every U.S. household, each household would be using 60 MWh annually, with manufacturing accounting for 20 MWh of this.

Out of all the energy consumed by U.S. manufacturers annually, induction motors make up 50 percent of the load. Of that 60 MWh aggregate number, motors would account for 10 MWh.

<img title="MA-2014_Factory-Auto-fig1" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig1(1).gif" alt="MA-2014_Factory-Auto-fig1" />

<strong>Figure 1.</strong> Motor electricity use as a percentage of delivered energy by each industry

<strong>Source: </strong>U.S. Energy Information Administration

There are two inherent design limitations to induction motors that pertain to efficiency and energy consumption:
<ul>
	<li>Motors are rated to operate at one speed. They can be very efficient at this one speed; however, their efficiency drops significantly when mechanical or resistive means are used to vary motor speed.</li>
	<li>Because motors are heavily inductive loads, they have a power factor that is less than one.</li>
</ul>
The advent of adjustable frequency drives in the 1970s and 1980s provided the first economically viable method for circumventing these limitations. Using adjustable frequency drives, industrial facilities can control motor speed and the utility side power factor-increasing energy efficiency and providing greater control of their processes. The return on investment for purchasing adjustable speed drives is typically between 12 to 18 months, depending on motor utilization.
<h1>Motor basics</h1>
<h3>Defining speed</h3>
The speed of an induction motor is governed by two attributes: electrical driving frequency and the number of poles. In the U.S., a motor that is connected directly to the utility will have a driving frequency of 60 hertz (Hz). With a standard four-pole motor, the revolutions per minute (rpm) are 1800, calculated with the following formula.

Using a motor at its rated speed results in an efficiency rating close to the manufacturer's specifications. However, situations arise where an operator would like to change the motor's speed. For example, a hydraulic pump operator installs a flow-limiting valve to be able to control the flow of water from the pump. In this case, using the valve is analogous to driving a car with "the pedal to the metal" and varying the vehicle's speed with the brake. In both cases-driving with the brake on and adjusting a motor's speed with flow-limiting valve-energy usage is inefficient.

A motor's efficiency can be kept at a maximum by allowing it to turn at its rated speed, which is determined by the equation above. By adjusting the driving frequency delivered to the motor, the motor speed can be controlled and changed, while avoiding the use of a valve or mechanical brake. This is precisely what an adjustable frequency drive does.

<img title="MA-2014_Factory-Auto-equation1" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-equation1(1).gif" alt="MA-2014_Factory-Auto-equation1" />
<h3>Power factor control</h3>
Motors operate by utilizing magnetic fields. The specifics of how this works is not as important as realizing what producing a magnetic field entails. There are two kinds of current that the motor uses: rotor current and magnetizing current. The motor uses the rotor current to produce torque. Magnetizing current is used by the motor to create the magnetic fields. The ratio between the magnetizing current and the total current-which is the sum of the rotor and magnetizing currents-determines a motor's power factor. Figure 2 shows the motor circuit. The current equations highlight the current through the circuit (<em>I<sub>1</sub></em> is the stator current, <em>I<sub>M</sub></em> is the magnetizing current, and <em>I<sub>2</sub></em> is the rotor current).

<img title="MA-2014_Factory-Auto-fig2" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig2(1).gif" alt="MA-2014_Factory-Auto-fig2" />
<strong>Figure 2. </strong>Equivalent circuit for an AC induction motor

Figure 3 depicts the intensity of magnetic fields within a motor. These fields are constantly changing, and every motor uses magnetizing current to create them. The horsepower (hp) of the motor, its geometry, the material it is made of, and a number of other factors determine the amount of magnetizing current it requires to create these magnetic fields.

<img title="MA-2014_Factory-Auto-fig3" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig3(1).gif" alt="MA-2014_Factory-Auto-fig3" />
<strong>Figure 3. </strong>Magnetic fields in a motor

Some utilities have limits on the amount of magnetizing current that can be drawn by a customer. If customers exceed this limit, then the utility will bill them to correct the power factor. Capacitors or other more advanced power factor correction systems can be used to mitigate the magnetizing current that is drawn from the utility.

Adjustable frequency drives help to remove the need for capacitors. When a motor and an adjustable frequency drive combination is used, the drive is installed between the motor and the utility. Because the drive's power factor is typically no lower than 98 percent, it acts as a buffer. Therefore, the utility will not be able to "see" the low power factor of the motor, and no additional capacitor banks need be installed.
<h3>Understanding adjustable frequency drives</h3>
Drives consist of four main sections: a direct current (DC) rectifier, a DC bus, an inverter, and a microprocessor. Three-phase or single-phase power from a 60 Hz alternating current (AC) source is fed into the input of the drive. An AC-to-DC converter (or rectifier) converts that alternating current into direct current; typically, a rectifier uses six diodes to make this conversion. After this energy is converted, it is stored on the DC bus. The DC bus consists of capacitors, which keep the power factor of the drive close to one and remove the need for external capacitors on motors with a low power factor, as specified by the utility.

The DC bus is used to regulate or maintain a consistent DC voltage and feed the inverter section of the drive. The inverter uses the switching capabilities of insulated gate bipolar transistors (IGBTs) to convert the DC bus voltage into pulses, simulating an AC sine wave. The output frequency and voltage to the motor is adjusted by varying the duration of each IGBT pulse; this is where the term <em>pulse width modulation</em> (PWM) comes from.

Finally, the microprocessor (not shown in figure 4) interprets user commands through a keypad, input/output terminals, or communication protocols and regulates the modulation of the IGBTs. A simplistic diagram of an AC adjustable frequency drive is shown in figure 4.

<img title="MA-2014_Factory-Auto-fig4" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig4(1).gif" alt="MA-2014_Factory-Auto-fig4" />

<strong>Figure 4. </strong>Basic configuration of an adjustable frequency drive

&nbsp;
<h3>Speed and torque control</h3>
Adjustable frequency drives enable users to adjust the speed of motors without additional mechanical means. They also provide constant torque, maintaining a consistent speed-even while the load changes. An escalator is a great example of this feature. Escalators maintain a constant speed; it does not matter if one person or twenty people are riding at the same time. Likewise, drives can monitor the load and adjust dynamically to maintain the speed. Programmable logic controller-like functionality is also incorporated into some drives. Both digital and analog inputs and outputs are common to most adjustable frequency drive platforms. This allows both simple and complex control logic to be added into drive operation. For example, drives can change the motor speed based on predetermined changes to conditions in their operating environments.
<h3>Less mechanical stress and lower current draw</h3>
Drives also help to reduce the mechanical and electrical stresses on the facilities infrastructure. Across-the-line starting can create large instantaneous torsion, friction, and tension strains on motor shafts, linkages, belts, and couplers. The instantaneous and repetitive stress can lead to premature failure of these devices. Further, it can draw an excessive amount of current, up to 13 times the motor's full load amps (FLA), depending on the NEMA type of motor being used.

Typical NEMA style-B squirrel cage induction motors will draw up to six or seven times the motors FLA. The inrush of current on larger loads can drain a facility's electrical capacity and create numerous problems, including contactor dropouts, light sags, and disruption to information technology networks. In addition, some electrical utilities charge facilities based on peak demand usage. Large inrush currents or multiple motors starting at once can easily exceed a facility's capacity and lead to excessive peak demand charges. Furthermore, most drives operate on the linear slope of a motor's torque/speed curve by matching the electrical and mechanical frequency of the motor. This produces more torque per amp than an across-the-line starter, thus maximizing the power being used.

An exploration of a typical torque-versus-speed curve (figure 5) for a NEMA B motor helps illustrate this. Ideally, the motor operates in the linear portion of the torque-versus-speed curve. This supports rated torque and efficiency. However, when a mechanical brake is used, motor performance moves left, out of this high efficiency, linear region-over the maximum torque hump-and into the nonlinear region. This is where the motor draws more amps for the torque it produces, and the efficiency drops significantly.

Adjustable frequency drives shift the torque-speed curve, so that the motor operates in the linear portion of the curve. Figure 6 depicts how the drive lowers the frequency and moves the torque-speed curve left, so that the motor consistently operates at the maximum possible efficiency.

<img title="MA-2014_Factory-Auto-fig5" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig5(1).gif" alt="MA-2014_Factory-Auto-fig5" />

<strong>Figure 5. </strong>Typical torque-versus-speed curve for a NEMA B motor

<img title="MA-2014_Factory-Auto-fig6" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig6(1).gif" alt="MA-2014_Factory-Auto-fig6" />

<strong>Figure 6. </strong>Shift of torque-versus-speed curve as drive reduces frequency
<h1>Driving energy savings</h1>
<h3>Optimizing conveyor systems</h3>
When used in conveyor systems, drives avoid the need for gears and clutches, which also enable multiple speeds within conveyor systems. Removing gears and clutches increases efficiency and decreases the overall mechanical components in a facility-helping to reduce maintenance and downtime. In addition, when paired with sensors, drives are ideal for conveyor spacing applications. They can very quickly and precisely control conveyor speeds.
<h3>Enhancing efficiency in pumping applications</h3>
To add monetary values to this concept, consider a plant that pays $0.17/kWh from 12 PM to 8 PM and $0.13/kWh for off-peak times. The plant has a 100-hp motor running 15 hours a day with a throttling valve (three hours at 100 percent, three hours at 80 percent, and nine hours at 50 percent speed). If the valve control unit and valve were replaced with an adjustable frequency drive to match the required speed, the theoretical energy savings would be $2,000 per month.

These kinds of savings can be better understood by reviewing the affinity laws (figure 7). Then we can calculate the theoretical load requirements and potential energy savings. The first curve shows that flow varies linearly with speed. Decrease speed to 50 percent, and the flow decreases to 50 percent. The second curve shows that pressure or head varies as the square of speed. If we go to 50 percent speed, we will have 50 percent flow from the first curve, but the pressure or head will be only 25 percent from the second curve. The third curve shows the power required for a particular flow requirement. For this we see that energy varies as the cube of speed. Again if we set speed to 50 percent, we have 50 percent flow at 25 percent pressure, but at only 12.5 percent power. This is where the potential for energy saving comes. These curves apply only to fan applications where there is no static pressure. There are also significant savings to be had with pumps; however, the curves are slightly different due to the presence of static head.

<img title="MA-2014_Factory-Auto-fig7" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig7(1).gif" alt="MA-2014_Factory-Auto-fig7" />

<strong>Figure 7. </strong>The affinity laws

Figure 8 shows potential energy savings in a fan application. If a throttling device is used to control flow, the energy used can be described by the upper curve of the figure. If an adjustable frequency drive is used, the lower curve describes the energy used. The difference is energy savings. The figure shows that the maximum energy savings occur when the operator needs to reduce the flow rate of the system.

&nbsp;

&nbsp;
<div><img title="MA-2014_Factory-Auto-fig8" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig8(1).gif" alt="MA-2014_Factory-Auto-fig8" /></div>
<div><strong>Figure 8.</strong> Energy savings from using an adjustable frequency drive versus a throttling valve</div>
<h1>Regeneration</h1>
<h3>Centrifuge applications</h3>
<div><img title="GOOD--MA-2014_Factory-Auto-fig9" src="https://www.isa.org/uploadedImages/Content/Standards_and_Publications/ISA_Publications/InTech_Magazine/2014/Jan-Feb/MA-2014_Factory-Auto-fig9(2).gif" alt="MA-2014_Factory-Auto-fig9" width="202" height="400" align="left" />
<div><strong>Figure 9. </strong>
Two centrifuges utilizing regenerative capabilities</div>
</div>
Centrifuges can be large and have a very high moment of inertia. These kinds of loads are often used in food processing applications (e.g., sugar refineries). Although it takes a significant amount of energy to begin spinning these large inertias, after they begin spinning, it does not take much energy to maintain rotation. If a facility has two centrifuges that run at opposing times, it will expend a significant amount of energy spinning one centrifuge up, and then it will simply dissipate energy as the other centrifuge spins down very slowly. By using two drives with a common DC bus, centrifuge operators can cut their energy use almost in half.

&nbsp;

In figure 9, two centrifuges are connected to their own individual inverter units. The front end feeds electricity from the utility to power the DC bus. The inverter powering centrifuge 1 draws power from the DC bus to bring the centrifuge up to full speed. When it is time to stop centrifuge 1 and start centrifuge 2, centrifuge 1 begins to act like a generator and power the common DC bus. Centrifuge 2 is then able to spin up using the energy from centrifuge 1. Any extra power that is required to bring centrifuge 2 to full speed will be provided by the front end to the common DC bus. In this way, energy is recycled by using an adjustable frequency drive with two inverters and a common DC bus.

Figure 9. Two centrifuges utilizing regenerative capabilities

&nbsp;
<h3>Unwinders and rewinders</h3>
Another beneficial application for regenerative adjustable frequency drives is paper slitting. In the manufacturing process, paper is initially pressed into wide sheets, which need to be cut into smaller ones. This requires the paper to be held taut as it is cut, which is accomplished by an unwinder and rewinder combination. The unwinder holds the roll of paper and acts as a brake; the winder pulls the paper toward it and requires a motor to apply torque. Like the previous centrifuge example, the unwinder provides power to the common DC bus as it is acting like a generator. The winder draws power from the common DC bus to apply torque. The front end keeps the common DC bus charged, but this only requires a very small amount of power from the utility.
<h3>Returns beyond energy savings</h3>
An adjustable frequency drive configuration with two inverters and a common DC bus provides regenerative capabilities and tremendous energy savings. Beyond saving energy, drives also provide torque/speed control and automation control. These capabilities can be observed in pumping applications, people movers, conveyor systems, and many others. Additionally, drives can also be used as a powerful diagnostic tool to record and analyze motor load profiles, system faults data, and other operational characteristics. An adjustable frequency drive also has many features that help protect the motor. With these features, manufacturers can take steps to prevent downtime and protect the investment they have made in their equipment.
<h5>ABOUT THE AUTHOR</h5>
<strong>Oreste "Rusty" Scioscia Jr.</strong> (<a title="RustyVScioscia@eaton.com" href="https://www.isa.org/standards-and-publications/isa-publications/intech-magazine/2014/mar-apr/factory-automation/drive-energy-savings/RustyVScioscia@eaton.com">RustyVScioscia@eaton.com</a>), a senior application engineer at Eaton, completed his undergraduate degree in mechanical engineering at the University of Pittsburgh with magna cum laude honors. He graduated cum laude from the University of Pittsburgh in December 2013 with his masters in electrical engineering (concentrating on electric machines and power systems). Scioscia performed electric machine and transformer research using advanced high-frequency magnetic materials under a grant from the U.S. Advanced Research Project Agency - Energy.

- See more at: https://www.isa.org/standards-and-publications/isa-publications/intech-magazine/2014/mar-apr/factory-automation/drive-energy-savings/#sthash.xlYtUkr9.dpuf