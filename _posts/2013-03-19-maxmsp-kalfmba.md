---
layout: post
title:  "Designing Instruments for Folding Laptops"
date:   2013-03-19
categories: coding music max
---

This is one of my latest creations: a kalimba-esque synthesizer called KalFMba.
No physical modelling (yet…), rather it works based off a simple FM synthesis
algorithm. I started this project because I was given a nearly-dead Dell XT2
tablet PC which I resurrected and beefed up. At the time I had recently
purchased Max 6 and was intrigued by the idea of creating unique touch screen
interfaces for software instruments. A few ideas were played with but nothing
came to complete fruition until I decided to further KalFMba as a project for
my human-computer interaction course.

![KalFMba in action, used within Ableton Live](/images/kalfmba-use.png)

As demonstrated in the above image, the LCD panel on most tablet PCs can swing
around but necessarily fold down onto the keyboard, creating an adjustable
touch screen “easel.” This is the type of environment KalFMba was designed for,
and it allows the laptop can truly become an instrument rather than sitting
behind MIDI devices. It also means that instruments that could only work on a
mobile platform such as an iPad or Android tablet could be ported to Windows or
OS X to allow for seamless DAW integration. All functionality can be changed
directly from the touch screen without needing to use the mouse, including
audio effect settings and preset loading/saving. KalFMba can be played without
a touch screen by manually clicking the buttons, but it’s harder to play and it
lacks MIDI input functionality for now.

![KalFMba Interfacd](/images/kalfmba-interface.png)

KalFMba uses a simple two-operator FM synthesis algorithm to generate the dry
tine signal, which can be routed through three available audio effects. There
is a chorus which can shift between typical chorus sounds and bizarre modulated
pitch-shifting, a simple non-synchronized delay, and a wispy yet powerful
reverb. All of the audio effects and tine tunings can be saved into one of 15
available preset slots, and the effect settings can be locked into place during
performances using the ‘lock’ button. The seven tines also have course and fine
tuning settings to allow the musician to create beat frequencies between
similarly tuned notes, just like on real kalimbas.

![KalFMba Internals](/images/kalfmba-internals.png)

You can listen to KalFMba in action from the SoundCloud link below:

[SoundCloud](https://soundcloud.com/griffinmoe_sounds/kalfmba-demo)

KalFMba has been ported over into Max for Live so it can be played within
Ableton Live, so if you like what you heard and have both of these products
(and a touch screen panel…these are a lot of qualifiers) you can download it
for free under [Creative Commons
  licensing](http://creativecommons.org/licenses/by-nc/3.0/). Have fun!

[KalFMba Download](/assets/KalFMba.amxd)
