---
title: Tones
layout: page
comments: true
sharing: true
footer: true
---

Since tones are the basis of melody and harmony we will start by studying simple tones. Afterwards we will move on to relations of two or more tones.

I hope you have already heard many tones in your life (otherwise how poor a life would be without music). Nevertheless, we can listen to some examples first.

	TODO: a sound example of several tones
		- tones with various pitch, duration, intensity, timbre, etc.
		- a spectrogram (more concrete visualization)
		- a piano roll (more abstract one)

## Summary of the physical fundamentals

{% comment %}

Possibly move this to the summary section of the Physics chapter.

{% endcomment %}

### Harmonic sounds

We have already learnt in the physics chapter about *harmonic sounds*. They can be thought of as sinusoid waves with basic properties: *frequency*, *amplitude* and *phase*. The frequency is the number of cycles per second, the amplitude is the "size" of the wave from zero to a peak and the phase is how the wave is shifted in time relative to some reference time.

<figure class="center">
	<img src="{% asset_path sine-frequencies.png %}">
	<figcaption>Sine waves of various frequencies</figcaption>
	<img src="{% asset_path sine-amplitudes.png %}">
	<figcaption>Sine waves of various amplitudes</figcaption>
	<img src="{% asset_path sine-phases.png %}">
	<figcaption>Sine waves of various phases</figcaption>
</figure>

In practice tones are typically composed of a sum one or more such simple harmonically related sinusoid waves (*harmonics*) - the *fundamental* one (1st harmonic) and the *overtones* (2nd, 3rd, etc. harmonic). The frequencies of the overtones are multiples of the fundamental frequency by small natural numbers. We can visualize which frequencies a harmonic sound contains via its *spectrum*.

	TODO: a spectrum of some harmonic sound

Each overtone can be of different amplitude which can also vary in time and the particular combination of overtones makes up the timbre - the particular "color" of the tone.

	TODO: spectra of two sounds of different timbre

### Human perception

We have also learnt something about how humans perceive such sounds. For many harmonic sounds people are able to interpret multiple harmonically related sounds as a single tone instead of separate sounds and also to distinguish between multiple tones. The relative "height" of such perceived sound is called *pitch* and it is based on the frequency of the fundamental harmonic of the tone.

Some instruments (like violin) are capable of producing tones with pitch changing continuously, while other instruments (like piano) can only make tones of some selected pitches.

If we take two arbitrary couples of pitches such that humans perceive as they have equal distance the difference of their frequencies would be different. Similarly to the perception of pitch also the perception of intensity is not linear but rather logarithmic. Both allows to percieve small differences over a broad range of frequencies or intensities respectively by mapping them onto a smaller range.

	TODO: linear frequency domain vs. log-frequency domain (of pitch)

The operation of moving a pitch up or down by some distance is called *transposition*. In the frequency domain transposition is represented by multiplication (scaling) while in the pitch domain it is just addition (shifting).

	TODO: transposition of a harmonic tone in both domains

In the linear frequency domain the harmonics are equally spaced, on the other hand in the log-frequency (pitch) domain the octaves are equally spaced.

	TODO: illustration

As for the intensity the perception is not purely logarithmic. The perceived *loudness* depends also on the combination of pitch and intensity. This non-linearity can be measured and is called [equal-loudness countour](http://en.wikipedia.org/wiki/Equal-loudness_contour).

## Pitch circularity - a spiral of pitches

There is a very important feature of our sound perception - *pitch circularity* or *octave equivalence*. Some tones sound very similar and when played at once it might be not be easy to distinguish them.

Consider two tones composed of many harmonics, A and B. The fundamental frequency of the tone B is exactly twice as high as of tone A (this 2:1 ratio is generally called an *octave*). Now the each harmonic of the second tone is excatly aligned with every other harmonic of the first tone. It is illustrated here:

	A: 1   2   3   4   5   6   7   8   9  10  11  12  13  14  15  16
	B: .   1   .   2   .   3   .   4   .   5   .   6   .   7   .   8

	TODO: sound example	- two octave-related harmonic tones

[It has been found](http://www.neuroscience-of-music.se/Octave-History.htm) that our brain is structured in such way that tones related by one or more octaves - powers of two (2x, 4x, 8x, etc.) - are processed in similar places. In other words the perception of similarity of such tones is hard-wired into our brain.

To better demonstrate this relationship we can visualize the space of pitches as a spiral rather than just a line.

	TODO: illustration:
	- pitch space as a line
	- pitch space as a spiral

This phenomenon is heavily exploited both in musical practice and theory.

{% comment %}

- for octave interval the difference is equal to the base!
	- |2A - A| = A
	- there is no beating
	- only the harmonic profile (timbre) of the lower tone is changed

{% endcomment %}

### Pitch class (chroma) - from spiral to circle

Since humans perceive octave-related harmonic tones as of very similar or same quality we can make a further abstraction to pitch. We can group all pitches related by one or more octaves into a single group. If we picked some pitch on the spiral this would look like drawing a vertical line to join all the pitches above and below. Each such a group of pitches is then called a *pitch class* or *chroma*.

	TODO: illustration - pitch spiral with vertical lines connecting pitch classes

By discarding the "height" on the spiral we obtain a diagram called *pitch class circle*. The pitch class in then represented only by the angle on the circle.

	TODO: illustration - pitch class circle

Transposition on the pitch class circle is represented by rotation in one or the other direction.

	TODO: illustration - transposition on a pitch class circle

## From continuous to discrete pitches

In practice often musicians use not all possible pitches but rather only some selected ones, a collection. There might be multiple reasons:

- some intruments are tuned such that they produce only fixed pitches (eg. piano)
- a collection of pitches is selected so that they work well together (eg. a scale based on some tuning)
- a small set of pitches is better tangible than an infitite space of continuous pitches

Thus in practice we work often with a discrete collection of selected pitches. Still we can visualize them as points on the spiral or circle.

An example of a discrete set of pitches (and thus pitch classes) could be the chromatic scale under equal temperament tuning with some fixed reference frequency (eg. 440 Hz).

	TODO: illustration
	- spiral with selected pitches
	- circle with selected pitches

Since we can name the pitches in our discrete collection, we can make a nice abstraction and hide away the details of the reference frequency of the tuning, or the actual tuning system. This is for example the base of various music notations.

The power of such an abstraction is that the musicians do not have to bear in mind all the details that are not necessary for their work. Eg. the pitch class names C is the same no matter if the reference frequency is slightly higher or lesser depending on the technical needs of the orchestra (and thus the actual frequency of that pitch changes).

## Visualization
- spectrogram - low-level time-frequency-intensity
- piano roll - higher-level time-pitch
- piano keyboard diagram - static moment
- traditional notation - note staff - abstract time-pitch and more
- tone clock - static moment - pitch class

## The life of a tone - from the perspective of intensity

Although an ideal sinusoid wave is infinite in practice tones are of limited duration. At some time they are "born", they "live" for some shorter or longer time and finally they "die". They typically do not appear or vanish abruptly, but rather gradually.

Although tones can be created by many instruments via various physical principles their common life cycle can be roughly described in four phases.

	TODO: illustration
	- guitar tone, organ tone, percussive tone

- *attack* - The initial phase when the intensity is rising until it hits some maximum. A short attack is typical for instruments which produce sound via some percussion, such as plucking a string. In the attack phase the tone might contain much noise for some short time.
- *decay* - The phase when the intensity of the attack decreases and changes to sustain. Also the noise is fading away and the harmonic parts become more noticable.
- *sustain* - The phase when the intensity of the tone is held approximately constant for a longer time. Long constant sustain is typical for wind instruments when the tone is produced as long as there is a steady flow of air, or for violin with a continuous dragging of a bow.
- *release* - The last phase when the intensity falls down to complete silence. Eg. for plucked string typically there's no sustain phase and the decay and release phases are fused. Also for percussive sounds there might be just the noise components and no harmonic components to that in fact there's no sustain or release phase.

The characteristics of each phase depends not only on the instrument type but also on the specific way the tone is played.

This [ADSR envelope model](http://en.wikipedia.org/wiki/ADSR_envelope#ADSR_envelope) of tones is described in more detail on Wikipedia.

More information about the musical usage of lower-level variations of intensity (articulation) and higher-level ones (dynamics) will be discussed in more detail in a separate section.

## Summary

In this section we have learned about harmonic tones. We have summarized their basic physical properties, we have examined the basics of human perception of tones. The important is that human perception of pitch and loudness is not linear but rather logarithmic and that pitch perception has periodic attributes - octave-related pitches are perceived as very similar. This pitch circularity in addition to selecting only several discrete pitches to work with then can be exploited to reduce the number of pitch classes that we work with to just a few objects (out of the continuous space). Also we have explored the basics of the life cycle of a tone from the intensity point of view.

Now we are ready to start playing with a combination of multiple tones, beginning with [intervals](../intervals/).
