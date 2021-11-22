---
title: Inspect data
---

## Inspecting data

Let's take a closer look at your field data or the gibbon datasets :eyes: with the help of two very useful QGIS toolbars

### Map navigation toolbar
<img src="{{site.baseurl}}/src/img/QGISToolbar_MapNav.png" alt="QGIS map navigation toolbar">  

> 1. If you have a mouse with a wheel, you can use the wheel to zoom in/out.  If not, click on the `Zoom In` tool <img src="{{site.baseurl}}/src/img/QGISTool_ZoomIn.png" alt="QGIS Zoom in tool"> and use it to draw a box (click and drag) on an area of your map that you want to view more closely
2. Use the `Pan` tool <img src="{{site.baseurl}}/src/img/QGISTool_Pan.png" alt="QGIS Pan tool"> to drag the map around
3. Use the `Zoom Out` tool <img src="{{site.baseurl}}/src/img/QGISTool_ZoomFull.png" alt="QGIS Zoom full tool"> to move 'further away' from your data
4. A handy shortcut to view the full extent of your datasets is the `Zoom Full` tool <img src="{{site.baseurl}}/src/img/QGISTool_ZoomFull.png" alt="QGIS Zoom full tool">
5. The `Zoom Last` and `Zoom Next` tools <img src="{{site.baseurl}}/src/img/QGISTool_ZoomLastNext.png" alt="QGIS Zoom last and Zoom next tools"> are useful to rapidly switch between areas, or go back to a previous view if you moved your view by accident
6. We'll use the other tools on this toolbar later in the course, but you're welcome to explore them now


### Attributes toolbar
<img src="{{site.baseurl}}/src/img/QGISToolbar_Attributes.png" alt="QGIS attributes toolbar">  

> 1. Select the `Identify features` tool and click on one of the polygons or points to reveal information about that feature  
> :warning: **Warning!**  This tool only shows information for the layer that is currently highlighted in the Layers panel (top left).  So if you're clicking on points but the Layers panel has *NomascusConcolor_Distribution* highlighted, **nothing will happen**!  To reveal information from a particular layer, e.g. the gibbon sightings, make sure you've first clicked on that layer (*GibbonSightings_Survey1*) in the Layers panel
1. You can close the Identify Results pane by clicking on the top-right [x] button


If you clicked on a polygon to bring up the Identify Results pane, your project will look like this:
<center><img src="{{site.baseurl}}/src/img/QGIS_IdentifyDistributionPoly.png" alt="QGIS project with Identify results pane"></center>