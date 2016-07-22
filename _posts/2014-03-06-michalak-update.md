---
layout: post
title:  "Michalak Project Update"
date:   2014-03-06
categories: coding michalak
---

It has been a busy year since I last mentioned the Michalak Project and a lot
has happened since then. The Michalak Project is a collaboration with [Loyola
University Chicago’s Center for Textual Studies and Digital
Humanities](http://www.luc.edu/ctsdh/) to provide greater access to the Loyola
Archive’s [Michalak
Collection](http://content.library.luc.edu/cdm/.landingpage/collection/coll32).
Apple’s release of iOS 7 forced a few interface changes such as the new flat
design, and there have been a few under-the-hood improvements. We are currently
adding and annotating other broadsides from the Michalak Collection.

![Michalak Print with Annotations](/images/michalak2-annotations.png)

Much of the basic functionality has remained the same such as familiar gestures
and interface layout. The biggest app-wide change has been the transition to
the iOS 7 flat design style, with simple high-contrast colors that lend focus
to the broadsides. We also added a thumbnail gallery of the broadsides in the
app, which has replaced the original starting page. There will be more
broadsides added in the future, with the possibility that the app will
automatically view and retrieve other artifacts from Loyola University
Chicago’s CONTENTdm servers.

![Michalak Print Wall](/images/michalak2-printwall.png)

The older version of the app relied on popovers to display annotations, which
broke during the transition to iOS 7. The new annotation implementation is a
scrollable list on the side of the app which highlights and attempts to center
the relevant text. A swipe gesture can tuck the annotations into the side of
the interface, providing a clear view to the print. These changes have reduced
the need for toolbar buttons, which are now just the navigation and annotation
hide/display buttons.

![Michalak Annotation Table](/images/michalak2-annotationtable.png)

There are number of smaller improvements I am quite happy about, such as
sinusoidal animation interpolation, reduced memory usage, and true aspect ratio
accuracy. The latter was the result of the switch from a per-pixel to a
percentage based projection, which also tightened up view-window centering for
annotations. Much of the codebase has been trimmed and simplified, and now
everything documented with [Doxygen](http://www.stack.nl/~dimitri/doxygen/).

Once we have annotated and integrated enough prints we intend on releasing the
Michalak app on the App store. This is a slow process since this relies on busy
Loyola faculty to create the annotations and for me to integrate them into the
XML metadata. We do not have an ETA but expect to see the release announced on
this website and at the CTSDH.
