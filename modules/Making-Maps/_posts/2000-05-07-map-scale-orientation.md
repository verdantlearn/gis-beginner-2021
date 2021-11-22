---
title: Map scale and orientation
published: false
---

## Communicate scale and orientation on your map

To help your readers understand the *real-world size* of features on your map, and estimate distances between them, we'll add a **scale bar** :straight_ruler: to show a reference distance.  We'll also add a **north arrow** :arrow_up: to indicate the *orientation* of your map with respect to the magnetic poles

By the end of this exercise, your map will look something like this:

<center><img style="border: 1px solid" src="{{site.baseurl}}/src/img/Map_Stage3_ScaleBar.png" alt="Map with scale bar and north arrow added"></center>

### Add a scale bar

> 1. Click on the `Add Scale Bar` tool <img src="{{site.baseurl}}/src/img/QGISTool_AddScaleBar.png" alt="QGIS Add Scale Bar tool"> on the Project toolbar, and click on the map where you want your scale bar to be.  Click `OK`
2. Adjust the way the scale bar is displayed by editing settings on its `Item Properties` tab - you can adjust the size or number of segments, the style, and many other details

### Add a north arrow

> 1. Click on the `Add North Arrow` tool <img src="{{site.baseurl}}/src/img/QGISTool_AddNorthArrow.png" alt="QGIS Add Scale Bar tool"> on the Project toolbar, and click on the map where you want your north arrow to be.  Click `OK`
1. Accept the default style, or select another from the `arrows` folder under `Item Properties`.  We recommend a very simply style, so as not to distract from the message of your map with unnecessary detail



<!-- Tie back to resolution/scale? -->


<!-- ‘Scale’ is used to refer both to the magnitude of a study (e.g. its
geographic extent) and also to the degree of detail (e.g. its level of
geographic resolution).  Geographic scale is important because it
defines the limits to our observations of the Earth.  All Earth
observation must have a small linear dimension, defined as the limiting
spatial resolution, the size of the smallest observable object, the
pixel size, the grain of the photographic emulsion, or some similarly
defined parameter.  Observation must also have a large linear dimension,
defining the geographic extent of the study, project or data collection
effort. (Goodchild, M.F.  and Quattrochi, D.A., 1997 ‘Scale,
multiscaling, remote sensing, and GIS’ in D.A.  Quattrochi and M.F. 
Goodchild (eds), Scale in Remote Sensing and GIS, CRC Press, pp.  1–11)

‘Scale’ can also indicate the size of the map relative to the real
world, and that’s the way in which we’re using the word here.  These
different meanings of scale can be confusing, so whenever you encounter
the word ‘scale’ take a moment to consider to what the author is likely
to be referring.

As you know, maps are a miniaturised (scaled-down) version of the real
world or, in other words, a drawing of the earth’s surface as if you
were viewing it from high in the air.  If maps were life-sized, we
wouldn’t be able to carry them around with us!

In cartography, map scale, or representative fraction, refers to the
ratio of the distance on a map to the distance on the earths’ surface. 
The first number of the scale, to the left of the colon ‘:’ is always 1,
indicating the distance on the map in your unit of measurement (for
example, centimetres).  The second number, to the right of the colon, is
the much larger ground distance, in the same unit of measurement.  Be
aware that the left-hand side of equation (‘1:’) is sometimes omitted. 
For example, we commonly use 1:50,000 topographic maps in the field,
which means that 1cm on the map is 50,000cm (= 500m) on the ground. 
Another way to think about map scales is that the size of the object on
the map is one fifty-thousandth of its size in the real world.

Given that your map may be printed in a variety of sizes or zoomed into
on screen, the best way to show scale is with a scale bar, which
illustrates a known real-world distance such as 10km.  Features on the
map can then be compared with the length of this scale bar to judge
their real-world dimensions.  It only makes sense to illustrate scale on
your map by writing a representative fraction (e.g. 1:50,000) if you
control the size at which your map will be printed. -->
