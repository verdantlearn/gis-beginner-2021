---
title: Maps with QGIS
---

## Create a map in QGIS

Over the next few pages, we're going to gradually build up a map in QGIS, including all the components necessary for readers to understand your message, and relate the features on your map back to the real world.  We'll start by:
1. Creating a blank **print layout** in QGIS
2. Adjusting the **page size** to generate a map suitable for inserting into a pdf report - 180mm wide by 130mm tall, or you can choose a different size if you wish
3. Adding a **map** component to display your spatial layers

By the end of this exercise, your map will look something like this:

<center><img style="border: 1px solid" src="{{site.baseurl}}/src/img/Map_Stage1_Layers.png" alt="Map with layers added"></center>

<br>

> 1. Reveal the Project Toolbar by right-clicking on the grey toolbar area of QGIS and selecting `Project Toolbar`
1. Click on the `New Print Layout` tool <img src="{{site.baseurl}}/src/img/QGISTool_NewPrintLayout.png" alt="QGIS New Print Layout tool"> on the Project toolbar to create a blank canvas for your new map.  This will ask you to name your canvas, and then open a QGIS Print window.  Alternatively you can use the keyboard shortcut for printing, `Ctrl+P` or `Cmd+P`
2. To specify the page size, right-click on the blank canvas > `Page Properties`.  This will open up the `Item Properties` tab on the right-hand side of the print window
3. Under `Size`, select *Custom*, and manually enter a `Width` of 180 and `Height` of 130

### Add components

To build up the components of our map, we'll use the print layout `Toolbox` toolbar, which appears vertically along the left-hand edge of your print layout window:

<center><img src="{{site.baseurl}}/src/img/QGISToolbar_PrintToolbox.png" alt="QGIS Print Toolbox toolbar"></center>

<br>

Let's add a map to our blank canvas:

> 1. Click on the `Add Map` tool <img src="{{site.baseurl}}/src/img/QGISTool_AddMap.png" alt="QGIS Add Map tool"> on the Toolbox toolbar and then drag to highlight an area of your blank map canvas.  We suggest dragging across two-thirds of the width and three-quarters of the height
2. Click on your map to reveal the `Item Properties` sidebar if it's not already visible
3. Scroll down and tick the checkbox beside `Frame` to add a border around your map

<br>

:information_source: At this point, the precise position and size of your map on the canvas doesn't matter.  You can easily **reposition** the map at any point in the design process by dragging and dropping it (or any other map component) using the `Select/Move item` tool <img src="{{site.baseurl}}/src/img/QGISTool_SelectMoveItem.png" alt="QGIS Select or move item tool"> on the Project toolbar.  You can also **resize** the map by grabbing the corners or the centre of the edges and dragging.  Alternatively, you can specify the map's coverage manually under `Item Properties > Extents` if you need precise control of the geographic area shown

:warning: If you make changes to your project such as hiding/revealing layers in your main QGIS window, or changing their symbology, the map in your print layout may not update automatically.  Trigger layers to update by clicking the `Update Map Preview` tool <img src="{{site.baseurl}}/src/img/QGISTool_UpdateMapPreview.png" alt="QGIS Update map preview tool">  in the map's `Item Properties` tab
