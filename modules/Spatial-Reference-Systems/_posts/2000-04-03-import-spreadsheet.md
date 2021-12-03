---
title: Import a spreadsheet
---

## Import Latitude-Longitude

You may already be familiar with Latitude-Longitude coordinates from your own field data.  If not, you can try inspecting and importing this dataset from the gibbon case study 

The Che Tao NR staff have provided us with new data from their most recent patrol, looking for evidence of **threats to wildlife**

### *.csv* file format
*Threats_Evidence.csv* is in *.csv* format, or *comma-delimited*, with columns separated by a comma.  *.csv* is a non-spatial file format, although as you'll see, it does contain spatial information

Remember that QGIS won't automatically know where to draw data in *.csv* format, so we have to tell it where the location coordinates are stored.  Before we do that, let's take a look at the raw data

> 1. Download <a href="{{site.baseurl}}/src/datasets/Threats_Evidence.csv" download>Threats_Evidence.csv</a>
1. Open up the .csv file in Excel (or a text editor if you prefer)
2. Examine the columns:
   1. Does the information you've been given make sense?
   2. What type of vector data do we have - points, lines or polygons?
   3. Do you understand what the numbers in the coordinate columns mean?

## Add .csv data to QGIS

Here's a reminder of how to add *.csv* files:
> 1. `Layer > Add Layer > Add Delimited Text Layer...` <details> <summary markdown="span">:framed_picture: Screenshot</summary> :warning: Be aware that the csv file in these screenshots is different from yours! <center> <img src="{{site.baseurl}}/src/img/add-text-qgis-013.png" alt="QGIS screenshot: Add delimited text layer"> </center> </details>
> 1. Choose source file - click the `...` button and find *Threats_Evidence.csv* <details> <summary markdown="span">:framed_picture: Screenshot</summary> <center> <img src="{{site.baseurl}}/src/img/add-text-qgis-019.png" alt="QGIS screenshot: Choose text file"> </center> </details>
1. Ensure `Point coordinates` is selected under `Geometry Definition` <details> <summary markdown="span">:framed_picture: Screenshot</summary> <center> <img src="{{site.baseurl}}/src/img/add-text-qgis-033.png" alt="QGIS screenshot: Specify X and Y columns"> </center> </details>
2. QGIS should automatically recognise which columns contain the X (Longitude) and Y (Latitude) coordinates
3. Click `Add` and `Close`

<!-- <br>

<details> <summary markdown= "span" >:radio_button: :framed_picture: Click here for screenshots!</summary> 
<br>

:warning: Be aware that the csv file in these screenshots is different from yours!

- `Layer > Add Layer > Add Delimited Text Layer...`

<center><img src="{{site.baseurl}}/src/img/add-text-qgis-013.png" alt="QGIS screenshot: Add delimited text layer"></center>

- Choose source file - click the `...` button
<center><img src="{{site.baseurl}}/src/img/add-text-qgis-019.png" alt="QGIS screenshot: Choose text file"></center>

- Ensure `Point coordinates` is selected under `Geometry Definition`, and specify which columns contain the X and Y coordinates 
<center><img src="{{site.baseurl}}/src/img/add-text-qgis-033.png" alt="QGIS screenshot: Specify X and Y columns"></center>

- Click `Add` and `Close`

</details> -->


<!-- ### Add geometry to points

We're going to create a new column in GibbonSightings_Survey1.geojson to illustrate what the X (Longitude) and Y (Latitude) coordinates look like for these data

> Call them Lat-Long
> Then add in a different CRS later in the module -->