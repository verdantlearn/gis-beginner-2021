---
title: Import a spreadsheet
published: false
---

<Obsolete!  Don't publish>

## Import spatial data from a spreadsheet

Let's work with an example of Latitude-Longitude coordinates, to learn how to import spatial data from a spreadsheet

The Che Tao NR staff have provided us with a new dataset from their most recent patrol, looking for evidence of **threats to wildlife**

### *.csv* file format
*Threats_Evidence.csv* is in *.csv* format, or *comma-delimited*, with columns separated by a comma.  *.csv* is a non-spatial file format, although as you'll see, it does contain spatial information

To add this new layer to your GIS project, you'll need to use a new method.  QGIS won't automatically know where to draw data in *.csv* format, so we have to tell it where the location coordinates are stored.  Before we do that, let's take a look at the raw data

> 1. Download <a href="{{site.baseurl}}/src/datasets/Threats_Evidence.csv" download>Threats_Evidence.csv</a>
1. Open up the .csv file in Excel (or a text editor if you prefer)
2. Examine the columns:
   1. Does the information you've been given make sense?
   2. What type of vector data do we have - points, lines or polygons?
   3. Do you understand what the numbers in the coordinate columns mean?

## Add .csv data to QGIS

For those of you who are more confident with the basics of using QGIS, here are the steps without screenshots:
> 1. `Layer > Add Layer > Add Delimited Text Layer...`
1. Choose source file - click the `...` button and find *Threats_Evidence.csv*
2. Ensure `Point coordinates` is selected under `Geometry Definition`
3. QGIS should automatically recognise which columns contain the X (Longitude) and Y (Latitude) coordinates
4. Click `Add` and `Close`

<br>

For those of you who want more detail or visual instructions, here are the steps including screenshots: 

:warning: Be aware that the csv file in these screenshots is different from yours

- `Layer > Add Layer > Add Delimited Text Layer...`

<center><img src="{{site.baseurl}}/src/img/add-text-qgis-013.png" alt="QGIS screenshot: Add delimited text layer"></center>

- Choose source file - click the `...` button
<center><img src="{{site.baseurl}}/src/img/add-text-qgis-019.png" alt="QGIS screenshot: Choose text file"></center>

- Ensure `Point coordinates` is selected under `Geometry Definition`, and specify which columns contain the X and Y coordinates 
<center><img src="{{site.baseurl}}/src/img/add-text-qgis-033.png" alt="QGIS screenshot: Specify X and Y columns"></center>

- Click `Add` and `Close`



<!-- ### Add geometry to points

We're going to create a new column in GibbonSightings_Survey1.geojson to illustrate what the X (Longitude) and Y (Latitude) coordinates look like for these data

> Call them Lat-Long
> Then add in a different CRS later in the module -->