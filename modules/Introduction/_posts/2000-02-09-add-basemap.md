---
title: Add a base map
---

## Add a base map
A base map helps you to orient yourself in space, check that your layers are situated in the correction location, and understand your field sites better.  We're going to use Open Street Map for our base map

**Add a base map** to your QGIS project as follows:

1. `Layer > Add Layer > Add XYZ Layer...`
2. In the *XYZ Connections* pop-up, click the `New` button
3. In the *Connection Details* pop-up, add Name as *OpenStreetMap* and URL as *https://tile.openstreetmap.org/{z}/{x}/{y}.png*
4. Click `OK`, `Add` and `Close`
5. Drag the base map down to the bottom of the Layers panel

Your project should look like this:

<center><img src="{{site.baseurl}}/src/img/QGIS_BaseMap.png" alt="QGIS project including base map"></center>

Look at that!  You've created your first QGIS project and learned the basics of navigating around the map, and displaying layers - well done  :fireworks:


<!-- https://atcoordinates.info/2020/12/17/adding-basemaps-to-qgis-with-web-mapping-services/ -->