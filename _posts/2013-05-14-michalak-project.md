---
layout: post
title:  "Michalak Project"
date:   2013-05-14
categories: coding michalak
---

The Library Archives at Loyola University Chicago has a collection of over
1,000 artifacts from the eighteenth and nineteenth centuries, including
broadside prints and satirical cartoons. This collection was donated to LUC by
Thomas J. Michalak, and the [Center for Textual Studies and Digital
Humanities](http://luc.edu/ctsdh/) has been
[digitizing](http://content.library.luc.edu/cdm/landingpage/collection/coll32)
these prints and making them available to other scholars.  In an effort to
expand the reach and utility of these artifacts, I was
[invited](http://luc.edu/ctsdh/researchprojects/digitizingthemichalakcollection/)
by the CTSDH to develop a mobile application capable of viewing annotated
high-resolution prints from the collection. Below are some images from the
prototype that I developed over the Spring ’13 semester; all functionality and
appearances are subject to change as this application is still far from
completion.

![Michalak Project - Print Display](/images/michalak-print.png)

After selecting a print from the list at the beginning of the application, the
user is presented with a clean image with no annotations. The print can be
manipulated in the same way as the native iOS image gallery application:
single-finger panning, pinch gesture zooming, and double-tap zooming. Pressing
the magnifying glass in the bottom right corner displays annotations of the
print that are interactable and describes details of the print.

![Michalak Project - Annotation Interaction](/images/michalak-annotation.png)

The print can still be manipulated while the annotation popover is being
displayed to allow the user to look at other details surrounding the current
annotation. Annotations can contain links to other online content, for example
the above link takes the user to an artifact on the British Museum’s website.
The annotation popover points to the annotation controls, which guide the user
through the intended order that the annotations are meant to be read. This
functionality is intended for instructors who may wish to use this application
as a lecture aid, or for students who may be researching this print. Annotation
overlays can also be turned on or off while using the guided pathway to get a
better view of an obscured detail. The user can view all of the annotations
associated with this print by pressing the booklet icon in the bottom-right
corner:

![Michalak Project - Annotation List](/images/michalak-annotation-list.png)

Entries in this annotation list can be tapped, which will hide the list and
display the relevant annotation. The navigation button in the top-right corner
allows the user to view some of the metadata associated with the print:

![Print metadata – expandable to contain more data](/images/michalak-print-metadata.png)

Currently this application only targets iPad devices, though iOS 5.1 is the
minimum required version so all iPads are supported. This application is built
on top of OpenGL ES 2.0 for performance and greater visual enhancements not
available in ES 1.1. Print images are restricted to a maximum of 2048 pixels in
either dimension, as this is a device limitation of iOS devices (which we hope
to circumvent by chopping the prints into tiles). Each print has an associated
XML data file which stores the annotations and metadata. All prints and data
files are currently built into the application, but in the future we would like
to support [CONTENTdm](http://www.contentdm.org/) integration where users could
download other prints directly from their mobile device.

When we are satisfied with application, we will be making this project open
source and available to other Digital Humanities scholars.
