---
layout: post
title:  "3D Printed Audio Waveforms"
date:   2012-06-08
categories: coding music
---

[Instructables](http://www.instructables.com/) is a fantastic place to lounge
around in. It was in their email newsletter that I saw [this
project](http://www.instructables.com/id/Paper-Note-A-Tangible-Paper-Waveform/)
and loved the idea of taking a sound and giving it tactile presence and to see
the dynamics of a favorite piece of music. At first I just wanted to recreate
the Instructables project as a gift but I knew that assembling small paper
discs would be a pain, and paper was not going to be a tough enough material.
After stowing the thought away for a while, I realized I had all of tools
available to develop this individual’s idea into another direction.

![3D Printed Audio Waveform](/images/3dwaveform-pretty.png)

At Heartland Community College I have access to CNC lathe and a 3D printer with
no restrictions other than myself. For those who are not so familiar with the
CAD world, a 3D printer does exactly what an ink and paper printer does except
in three dimensions. In practice, a 3D shape is created by a technical artist
and is given worldly shape by the 3D printer through the medium of ABS plastic
. My alternative to the printer is the CNC lathe, which is like a normal lathe
except it is completely controlled through computer instruction. I had some
prior experience with the printer so I started out by studying it and writing
some code in Processing, which would play back a WAV file and use the buffer
levels to determine the radius of each cylinder slice just like on the
Instructables project. Rather than creating paper cylinders, the end result of
the program is an STL file ready to be sent to the printer. The completed
waveform is actually black, the grey material on the bottom is created
automatically by the printer and is used as support to print the main plastic.
The support material is designed to be broken away, but I left it attached
because it left me with a handy stand with no additional effort. 

![Waveform Mid-Printing](/images/3dwaveform-printing.jpg)

There are a few problems with using the 3D printer as there is only so much
available space available the on the printer, which affects the scale and
accuracy of the print. My next project is to use the CNC lathe and convert my
code to output GCode, which can give me increased accuracy, beautiful smooth
steps in between cylinders, and solid aluminum waveform. Unfortunately there
are no easy Processing/Java libraries for GCode, which means directly
controlling the lathe movements instead of just feeding data points into the
printer. I do not have any experience using a normal lathe, let alone a CNC
lathe, so it might be one of those fanciful ideas that never comes to fruition.

![Waveform Mid-Printing 2](/images/3dwaveform-printing2.jpg)
