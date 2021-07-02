---
title: Symbolise attributes
published: false
---


## Symbolise layers by attributes

So far we've ignored information in the attributes table of vector layers, and used identical symbology for all features in a layer.  Now it's time to explore a powerful visualisation option in QGIS :muscle: - the ability to symbolise vector features depending on properties in their attributes table

For all of these instructions you need to have the `Layer Properties` window open on the `Symbology` tab

### Visualise categorical attributes

For **vector** layers :diamond_shape_with_a_dot_inside:

> 2. Select `Categorized` from the dropdown menu at the top (the default is `Single Symbol`)
1. Choose the column you want to symbolise from the `Value` dropdown menu; for example *ThreatType* from the *ThreatEvidence* layer
2. Click on the `Classify` button in the bottom left
3. Click `Apply` and `OK` to finish

<br>

For *thematic* **raster** layers :black_square_button:

> 1. Ensure `Render type` is *Paletted/Unique values*
2. Double click on the `Color` or `Label` to manually edit the colour or label of each pixel value in your 

### Visualise continuous attributes

For **vector** layers :diamond_shape_with_a_dot_inside:

> 1. Select `Graduated` from the dropdown menu at the top
1. Choose the column you want to symbolise from the `Value` dropdown menu; for example *GroupSize* in one of the *GibbonSightings* layers 
2. Click on the `Classify` button in the bottom left
3. Click `Apply` and `OK` to finish


<br>

For *continuous* **raster** layers :black_square_button:

We don't have an example of a continuous raster layer in the gibbon case study, but a DEM would be one example.  These instructions are included for completeness, to help those working with their own data 

> 1. Under `Render Type`, select *Single band gray* or *Single band pseudocolor*
1. Click Classify to see the result of the default settings
2. Experiment with the settings e.g. `Interpolation`, `Color ramp` and `Mode` until you're happy with the result



### Adjust layer transparency

It can be useful to make layers partially **transparent**, particularly if you want to reduce the visual impact of thematic raster layers, or allow layers such as a hillshade/terrain to be faintly visible without dominating your map

For **vector** layers :diamond_shape_with_a_dot_inside:

> 1. On the `Symbology` tab, click on the triangle beside `Layer rendering` to expand that section
1. Adjust the `Opacity` to below 100% (e.g. 60%) and click `Apply` to see the result

<br>

For **raster** layers :black_square_button:

> 1. Switch to the `Transparency` tab
2. Adjust `Global opacity` to below 100% (e.g. 60%) and click `Apply` to see the result


*[DEM]: Digital Elevation Model