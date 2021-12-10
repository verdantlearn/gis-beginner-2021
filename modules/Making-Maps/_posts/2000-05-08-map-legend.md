---
title: Map legend
---


## Add a legend to your map

Legend
: A **legend** explains the symbology used for each of your map layers, so that readers can interpret what the symbols on your map mean, and understand your message

By the end of this exercise, your map will look something like this:

<center><img style="border: 1px solid" src="{{site.baseurl}}/src/img/Map_Stage4_Legend.png" alt="Map with legend added"></center>

<br>

### Add a legend

> 1. Select the `Add Legend` tool <img src="{{site.baseurl}}/src/img/QGISTool_AddLegend.png" alt="QGIS Add Legend tool"> on the Project toolbar, and click on the map where you want your legend to be.  Click `OK`
1. The default is for QGIS to add the legend for all your layers, regardless of whether they are visible on your map.  To remove all unnecessary items from the legend, tick the checkbox beside `Only show items inside linked map` on the legend's `Item Properties` tab
2. Alternatively, remove and add layers to your legend using the green `+` and red `-` buttons below the list of layers
3. You can edit the names of your layers in the `Layers Panel` of the main QGIS window, but if you want to rename the layer *only* on the legend, you can uncheck the `Auto update` box and double-click on the layer to open up the `Label` property for that legend item, where you can manually edit its name
