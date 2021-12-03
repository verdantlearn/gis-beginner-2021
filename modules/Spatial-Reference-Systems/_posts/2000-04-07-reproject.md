---
title: Reprojecting
---

## Reprojecting: Converting to a different SRS

It's not possible to measure distances or areas using angular coordinates, especially because the length of a degree of longitude varies depending on how close you are to the equator.  Therefore, if you need to do any **spatial analysis** on your data, it's necessary to **reproject** it

Reprojection
: Converting data from Latitude-Longitude to a projected SRS, or between different map projections

The advantages of reprojecting your datasets are:
1. **Simplicity** - if all your datasets and the project itself use the same SRSit's easier to manage GIS data and you're less likely to experience difficulties overlaying data.  This may not be possible, however, if you're working with datasets that have very different spatial extents - you will need to identify a projected SRS that works for all of the layers in your project
2. **Combining** data - if you wish to merge multiple datasets into a single geospatial file, e.g. field observations from repeated surveys, every dataset needs to use the same SRS 
3. **Analysis** - once your data are in a projected SRS, where the *unit of measurement is metres*, you can calculate meaningful distances and areas.  Many QGIS analysis tools will not work, or will give you a warning :warning: if you attempt to apply them to geospatial datasets that use angular coordinates

### Reproject gibbon sightings

Phuong has asked you to **combine the gibbon sightings** from the two gibbon surveys into a single dataset, for further analysis and map-making.  A preparatory step is to reproject one of the files into the same SRS as the other, before merging them together[^1].  We recommend reprojecting *GibbonSightings_Survey**1**.geojson* from Latitude-Longitude into the projected SRS *NSIDC EASE-Grid Global*, EPSG code *3410*.


> 1. Go to the `Processing` menu > `Toolbox`
1. Type *reproject* into the search bar of the Processing toolbox and double-click on `Reproject layer`
2. In the `Reproject Layer` pop-up window, under `Input layer`, select *GibbonSightings_Survey**1**.geojson*
3. Under `Target CRS`, search for and select *EPSG:3410 - NSIDC EASE-Grid Global*
4. Under `Reprojected`, click on the `...` button and select `Save to File...`
5. Specify a name for your new *.geojson*, including the EPSG code in the name so you can easily identify it as the reprojected layer
6. Click `Run` and close the `Reproject Layer` window


### Save .csv as .geojson

Before we can merge the two sources of survey data, we will convert the sightings from our *second* survey into a spatial data format[^2]

> 1. Right-click on *GibbonSightings_Survey**2**.csv* in the Layers panel > `Export > Save Features As...`
1. Under 'Select fields to export and their export options`, uncheck the columns *X* and *Y*.  We don't need these columns any more, and excluding them from our new file means we will have identical columns in the Attribute table of both Sightings layers, which will simplify the output Attribute table 
2. Save your file as a *.geojson*, again including the EPSG code in the name


### Merge into a single file
We are finally ready to merge our two layers!

> 1. Open `Processing > Toolbox` again if it's not already open and search for *merge*
1. Open `Merge vector layers`
2. On the `Merge Vector Layers` pop-up window, click the `...` button to the right of the `Input layers` box
3. Select your two survey datasets which use EPSG:3410 and click `OK`
4. Under `Merged`, click on the `...` button and select `Save to File...`
5. Specify a name for your new merged file, e.g. *GibbonSightings_Merged.geojson*
6. Click `Run` and close the `Merge Vector Layers` window
7. Open your new layer's Attribute table and check it contains 88 features, including sightings made by Binh


<!-- ### Final QGIS exercise
Are your layers all correctly aligned? -->

<!-- ### Optional
Identify and fix SRS errors in provided dataset e.g. wrong CRS applied -->

<br>

[^1]: In fact, the `Merge Vector Layers` tool can reproject and merge in a single step, but it's useful to know how to reproject so we'll do this preparatory step manually
[^2]: The `Merge Vector Layers` tool can cope with .csv as input, but making these separate steps explicit gives you more insight into the full process of merging geospatial datasets

*[SRS]: Spatial Reference System
