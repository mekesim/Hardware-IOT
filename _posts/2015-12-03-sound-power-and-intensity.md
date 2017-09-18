---
ID: 68
post_title: Sound Power and Intensity
author: Robot Yang
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/68
published: true
post_date: 2015-12-03 07:13:49
---
There has been a major missing ingredient so far in our discussion of quantifying loudness, making the connection between the amplitude of the sound wave (sound pressure) and the qualitative notion of loudness. We have talked about sound at a particular point (in a room, on a city street, or near an airport listening to jets taking off) without worrying about how the sound is produced. Connecting loudness to the source of sound energy is important, because as we know from our direct experience, how loud we perceive a produced sound depends on the distance between the source and our ear. Today, we'll quantify how loudness depends on the amount of sound energy produced and the distance between the source and our ear.
<h2>Sound Power</h2>
Sound always has a source. The source could be a musical instrument, people talking, a stereo system or a jet taking off. Different sources produce sounds with different qualities such as pitch and timbre. What concerns us here is another difference between sources of sound: the amount of sound energy they produce. Sound waves, like other waves, transport energy. For a sound wave, the amount of energy transported is proportional to the square of the amplitude of the wave. We have indicated this amplitude as p, because it corresponds to the amount of pressure oscillation in the air caused by the sound wave.

Where does the sound energy come from? The answer is that some object has converted energy of a different kind into sound energy. Typically, there is some sort of mechanical motion, a vibration of some sort, so mechanical energy is converted into sound energy. How loud a sound is depends on how rapidly the object converts energy into sound energy. So the relevant physical quantity to relate to loudness is the <i>sound power</i> produced by the source, or the rate at which sound energy is produced versus time. Referring back to our earlier discussions, power is the time rate of change of energy and has units of Joules per second. We give a new name to this unit: 1 Watt = 1 Joule/second. The Watt is the unit of power.

We will introduce a logarithmic scale for sound power, just like we did for sound pressure, because our perception of sound loudness is logarithmic. We define the <i>sound power level</i> from a source as
<p align="CENTER"><i>sound power level</i> = L<sub>W</sub> = 10 log( W / W<sub>0</sub>)</p>
As with our defintion of sound pressure level, we are forced to first find the ratio of the sound power to some reference power level. In this case, the reference sound power we'll use is W<sub>0</sub> = 10<sup>-12</sup> W. The "units" of sound power level are in decibels. This is really a <i>dimensionless</i> quantity. We quote the sound power level in decibels to remind ourselves that its a logarithmic quantity with a specific reference power.
<h2><a name="Intensity"></a>Sound Intensity</h2>
We haven't yet made contact with loudness. To do so, we need a <i>receiver</i> of the sound energy produced from the source. Before we get there, we have to ask the question where does the sound power produced from the source go? The simple answer is, <i>everywhere</i>. Most sources of sound send sound waves out uniformly in all directions. What this means is that if we are a certain distance from a source of sound, say a jet taking off, we will hear the same loudness sound independent of where we listen: either in front of the jet or behind the jet or to the side of the jet. The loudness of the noise we hear depends only on how far we are from the source of sound.

The geometrical shape that has all points equal distance away from a source is a <i>sphere</i>. The loudness we hear depends on the ratio of the <i>area</i> of our <i>sound collector</i> to the total area of the sphere surrounding the sound source. This motivates the introduction of another physical quantity associated with sound waves: <i>intensity</i>. The intensity of a sound wave is the amount of power in the wave per unit area and has units of W/m<sup>2</sup>. The intensity of a sound wave depends on how far we are from a source. If we label that distance as R, then the sound intensity is
<p align="CENTER">sound intensity = sound power / (4 pi R<sup>2</sup>)</p>
This says that on the surface of a sphere centered on the sound source, all points get equal intensity which agrees with our intuition. The sound intensity is just the ratio of the sound power to the <i>surface area of a sphere</i> of radius R (surface area of sphere = 4 pi R<sup>2</sup>), where R is the distance we are from the sound source.

We now have something that relates to our perception of loudness. This means that we should introduce a logarithmic scale, once again. We talk about the <i>sound intensity level</i>
<p align="CENTER">sound intensity level = L<sub>I</sub> = 10 log ( I / I<sub>0</sub> )</p>
with the reference intensity defined as I<sub>0</sub> = 10<sup>-12</sup> W/m<sup>2</sup>.

Both <i>sound pressure level</i> and <i>sound intensity level</i> are purported to measure the same thing: the loudness of a sound that we hear. This means that they better be equal. They are for the following reason. The sound pressure level can be written as
<p align="CENTER">sound pressure level = L<sub>p</sub> = 20 log ( p / p<sub>0</sub> ) = 10 log ( p<sup>2</sup> / p<sub>0</sub><sup>2</sup>)</p>
The last step in the chain of equal signs makes use of a property of logarithms, log( A<sup>n</sup> ) = n log A. In the above equation, n = 2 and A = p / p<sub>0</sub>. The next step to show the equality of sound pressure level and sound intensity level is to realize that the intensity in a sound wave is proportional to the square of the amplitude of the sound wave. This means that p<sup>2</sup> / p<sub>0</sub><sup>2</sup> = I / I<sub>0</sub>. The end result is that the sound intensity level and the sound pressure levels are identical quantities!
<h2>Multiple Sources of Sound</h2>
The final thing we need to discuss is how we get the total loudness of sound when more than one source produces sound power. Before we can do this, we need to make a subtle distinction in combining sound waves. It is possible to arrange two different sound waves so that they have a <i>fixed phase relationship</i>. This condition is called <i>coherence</i>. In this case, there can be either <i>constructive interference</i> (in other words the amplitudes of the two waves add when the crests and troughs of the two waves align) or <i>destructive interference</i> (when the crest of one wave aligns with the trough of the other and vice versa). There is interference between sound waves only when the crests and troughs of the waves have a fixed relationship. In general, this is very hard to arrange and requires that the source of the two interfering waves is identical.

When we have the coherent addition of two sounds, resulting in constructive interference, we must use the relationship:
<p align="CENTER">sound level, L = 20 log(p / p<sub>0</sub>)</p>

to find the amplitude of the individual sound waves, if the level is known. Once we have the amplitude, we ADD the amplitudes from the constructively interfering sounds, to find the amplitude of the wave when the two sounds are played together. We can then convert this to a level with the above equation, using the total amplitude of the sound wave.More generally, sounds from different sources have no <i>phase relationship</i>, meaning that the alignment of crests and troughs between the two waves is random: sometimes they align and sometimes they don't. In this case, there is <i>no interference</i> between the two sound waves. What happens when the two incoherent sounds are played together, is that the <i>intensities</i> of the individual sounds add together. This is actually easier to understand than interference. If you're at a party and one stereo system has a power output of 20 W and a second stereo of equal power is turned on, then the total sound power is just the sum of the powers from the two separate stereos.

Let's see how this works by looking at an example. Let's say that the sound intensity from one person talking is
<p align="CENTER">I<sub>1</sub> = 10<sup>-6</sup>W/m<sup>2</sup>.</p>

The sound intensity level from the person's voice is
<p align="CENTER">L<sub>I</sub> (1) = 10 log ( I<sub>1</sub> / I<sub>0</sub>) = 60 dB</p>

(prove this for yourself, remembering that I<sub>0</sub> = 10<sup>-12</sup> W/m<sup>2</sup> !). If a second person talks and produces sound with the same intensity, then the total intensity you hear is just the sum of the two intensitities: I<sub>total</sub> = 2 I<sub>1</sub>. The total sound intensity level is
<p align="CENTER">L<sub>I</sub> (total) = 10 log ( I<sub>total</sub> / I<sub>0</sub> ) = 10 log ( 2 I<sub>1</sub> / I<sub>0</sub> ).</p>
Now, we make use of a property of logarithms, log(A x B) = log A + log B to write
<p align="CENTER">L<sub>I</sub> (total) = 10 log (2) + 10 log ( I<sub>1</sub> / I<sub>0</sub> ) = 3 dB + L<sub>I</sub> (1)</p>
When two equal sound intensitities are added, the sound intensity level compared to the level from a single source is increased by 10 log (2) = 3 dB!