---
title: Sound and Silence
layout: page
comments: true
sharing: true
footer: true
---

Before we start playing with music we dig a bit deeper into the lower-level of musical abstraction - the physical principles of sound - how it its created, how it behaves and how it is perceived by humans. Thanks to understanding the foundations some problems in the higher levels will be much clearer to understand.

## Let's ask the fundamental questions

Imagine this situation: *Alice sings a tone. Bob listens to this sound. After a breif moment of silence he claps his hands in an applause.*

<img src="{% asset_path tone-and-clap.jpg %}">

Very simple, huh? However, we might ask several questions:

- what is sound?
- what is silence?
- what is a tone?
- what is a handclap? how it differs from a tone?
- how Alice created tone the tone?
- how it gets into Bob's ears?
- how Bob hears the music via his ears?

Let's try to figure out the answers.

## What is sound?

First take a medium in which sound can exists. One of such media is air that we breathe - tiny particles of gases, such as oxygen, water vapor, etc. There might be more or less such particles in some place. We call this *density* and this might be variable.

These particles usually make some tiny random motions but if we let some air closed and do not affect it from outsite on average the density doesn't change. Since no energy is transported via the medium, in this case air, we can hear nothing - it's *silence*.

### Click

Now what happens if something disturbs the quiet air? Let's say Bob claps his hands. Or similarly we can have a box with one side movable (imagine a loudspeaker with a membrane) and we move the membrane very quickly outside. The particles of air are pushed away and their local density increases. Each particle affects its neighbors with some force and they want to eventually achieve stability again. So the this change in density moves away and also fades away. What you could hear is a click or clap. Some energy were transported via the medium.

### Sound wave

Then what happens if this movable side of the box (the membrane) is moving periodically back and forth in *time*? Then the density would fluctuate between high and low and these sound waves would travel away from the source.

<p>
<figure class="center">
	<img src="//upload.wikimedia.org/wikipedia/commons/thumb/8/82/CPT-sound-physical-manifestation.svg/500px-CPT-sound-physical-manifestation.svg.png">
	<figcaption>
		Sound waves travel from the speaker to the ear.
		Credit: <a href="http://commons.wikimedia.org/wiki/File:CPT-sound-physical-manifestation.svg">Pluke - Wikipedia</a> (<abbr title="Creative Commons CC0 1.0 Universal Public Domain Dedication">CC</abbr>).
	</figcaption>
</figure>
</p>

Let's take one point through which the sound wave is propagating. The density varies there up and down in a similar way as the membrane is moving back and forth.

### Frequency and amplitude

The number of times there's a maximum of this simple wave in this point per second is called the *frequency*. If the membrane is moving slow the frequency is low, if its moving faster the frequency is higher. It is measured in Hertz (Hz). It is connected with how low or high we perceive a tone.

Also we might be interested how loud the wave is. The amount of how the membrane gets displaced is affecting the amount of displacement of the air particles. This is called *amplitude* of the wave.


### Attenuation with distance

Since the energy in the waves propagate in all directions it gets spread into the space thus the farther from the source the amplitude gets lower and lower. This is the reason why we can hear whispered words from close distance while we can't hear loud speak from several kilometers.

<p>
<figure class="center">
	<img src="//upload.wikimedia.org/wikipedia/commons/8/82/Spherical_pressure_waves.gif">
	<figcaption>
		Propagation of sound waves in all directions.
		Credit: <a href="http://en.wikipedia.org/wiki/File:Spherical_pressure_waves.gif">Thierry Dugnolle - Wikipedia</a> (<abbr title="Creative Commons CC0 1.0 Universal Public Domain Dedication">CC</abbr>).
	</figcaption>
</figure>
</p>

### Complex sound

In practice the typical sounds are not just clicks or waves of a single frequency. Rather many simple sound waves are mixed together.

TODO

- further reading:
	- http://en.wikipedia.org/wiki/Sound

- [iphone 4 inside a guitar oscillation](http://www.youtube.com/watch?v=ttgLyWFINJI)
- [visualizing vibrations on singing strings](http://www.youtube.com/watch?v=INqfM1kdfUc)
- [Bowed violin string in slow motion](http://www.youtube.com/watch?v=6JeyiM0YNo4)
- [stunning bass-string shot](https://vimeo.com/4041788)


- http://staff.science.uva.nl/~rein/MM/Topics/soundProcessing.html
- http://en.wikibooks.org/wiki/A-level_Computing/AQA/Problem_Solving,_Programming,_Data_Representation_and_Practical_Exercise/Fundamentals_of_Data_Representation/Sounds

- [transmisson of sound](http://www.youtube.com/watch?v=GkNJvZINSEY)
