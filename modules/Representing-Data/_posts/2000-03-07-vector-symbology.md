---
title: Vector symbology
---

<!-- Add reference to the correct type of case study layer -->

## Adjust vector symbology

So what do we mean by symbology?

Symbology
: The way a dataset is visualised or displayed, for example colours, line thicknesses or patterns

<!-- :rainbow: :bullseye: -->

Let's have a go at changing how vector data are symbolised in QGIS.  Try adjusting the symbology of your own field data, or work with one of the gibbon datasets

First of all, you need to open the layer's Symbology tab in Layer Properties:

> 1. Double-click on the layer you want to edit in the `Layers panel`, to open the Layer Properties pop-up window
1. Select `Symbology` from the left-hand menu
2. Continue with the instructions below depending on what type of vector data you're visualising


### Point symbology

> 1. At the top, under where it says 'Marker', click on `Simple Marker`
2. Adjust the `Size` and `Fill color`
3. Click `Apply` to see the effect of these settings
4. Optionally play with some of the other settings to understand what they do


### Line symbology

> 1. At the top, under where it says 'Fill', click on `Simple Line`
1. Adjust the `Color`
2. Click `Apply` to see the effect of these settings
3. Adjust `Stroke width` and `Stroke style` to see some of the other effects you can create


### Polygon symbology

> 1. At the top, under where it says 'Fill', click on `Simple Fill`
2. Click on the `Symbol layer type` dropdown just below and select `Outline: Simple Line`
3. Click `Apply` to see the effect - your polygons should now be drawn as an outline only, with no fill colour
4. Switch the `Symbol layer type` back to `Simple Fill`
5. Try adjusting the `Color`, `Stroke width` and `Stroke style` to see the effect of these settings

<br>
<img src="{{site.baseurl}}/src/img/QGIS_Symbology-Polygon.png" alt="Adjust polygon symbology in QGIS">


