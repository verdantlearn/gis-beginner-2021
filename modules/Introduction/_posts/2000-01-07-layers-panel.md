---
title: Layers panel
---

## Using the Layers panel
Most of QGIS' functionality is based around working with layers, and the Layers panel allows us quick access to fundamental tools 

### Adding landcover 

To help you become familiar with another type of spatial data, and practice managing layers, we're going to **add a landcover image** from the Copernicus global land cover map[^1]:

> 1. Download the <a href="{{site.baseurl}}/src/datasets/LandCover.tif" download>LandCover**.tif**</a> image (note the *.tif* file extension) and save it in your gibbon project folder
1. Download its partner <a href="{{site.baseurl}}/src/datasets/LandCover.qml" download>LandCover**.qml**</a> style file (note the *.qml* file extension) and save it in the same folder as the *.tif*.  This file ensures your image is coloured correctly by QGIS[^2]
2. Add the image using `Layer menu > Add Layer > Add Raster Layer...` - click on the `...` button to select *LandCover.tif*.  Don't worry at this stage if the landcover layer obscures your other datasets - we'll fix that shortly

### Zoom to landcover layer

Here's a shortcut to **zoom to a layer**, so that you can see its full extent in your map view:
> 1. Right-click on *LandCover.tif* in the Layers panel and choose `Zoom to layer`

### Change order of layers
The order of layers in the layers panel determines the drawing order of your data.  Layers lower down the list are drawn first (underneath), and layers higher up the list are drawn later (on top)

When you add new layers, QGIS stacks them above the active layer (highlighted in the Layers panel).  The landcover layer may be hiding your other layers.  Let's **reorder the layers** to improve their visibility.  Don't worry if the distribution polygons obscure most of the landcover image after this step - we will fix this in the next module
> 1. Drag and drop layers in the order that you wish them to overlay.  We recommend this order:
    - Points at the top (*GibbonSightings_Survey1*)
    - Lines (our project doesn't contain these yet)
    - Polygons (*NomascusConcolor_Distribution*)
    - Raster layers at the bottom (*LandCover*)

Your project should look like this:

<center><img src="{{site.baseurl}}/src/img/QGIS_LandCover.png" alt="QGIS project including landcover"></center>


### Hide/Reveal layers
You can also change layer visibility, to hide or reveal layers as you work on your project or create maps:
> 1. Click on the checkbox beside each layer's name in the Layers panel to hide or reveal them

### Remove layers
You can **remove layers** from your project if you no longer need them.  Remember that this does not delete the underlying spatial data files, just the link to them within your project
> 1. Right-click > `Remove Layer...`

### View layer properties
To view information about the layer:
> 1. Right-click on a layer and select `Properties` (bottom of the list)
2. Click on `Information` (top of the left-hand menu).  Note that here you can view the Path to where this layer's underlying spatial data is stored, and its CRS, amongst other things

Great work!  :star:  We have just one more QGIS task to complete in this module

---
[^1]: [Copernicus global land cover](https://land.copernicus.eu/global/content/annual-100m-global-land-cover-maps-available) map, downloaded from the [Global Land Cover Viewer](https://lcviewer.vito.be/) - available annually from 2015-2019, 100m cell size
[^2]: We'll explore how to use symbology in QGIS in more detail in Modules 2 and 4

*[CRS]: Coordinate Reference System, or spatial reference system - see Module 3