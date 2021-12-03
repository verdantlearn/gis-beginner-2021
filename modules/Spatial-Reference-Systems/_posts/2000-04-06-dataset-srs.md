---
title: Dataset SRS
---

### Specify a dataset's CRS in QGIS

To understand better how QGIS deals with data collected using a different SRS, let's add another new file to our QGIS project

The team leader of the gibbon surveys, Phuong, has received new data from her colleague Binh from a **second gibbon survey** in the westernmost edge of the nature reserve.  Binh has provided data as a *.csv*.  Let's look at the raw data before we add it to our GIS project

> 1. Download <a href="{{site.baseurl}}/src/datasets/GibbonSightings_Survey2.csv" download>GibbonSightings_Survey2.csv</a>
1. Open up *GibbonSightings_Survey2.csv* in Excel or your text editor
2. Examine the columns and identify those which contain the location information.  Compare them to the coordinate columns in *Threats_Evidence.csv*
3. Do you think the sighting locations are in Latitude-Longitude, or a different SRS? <details> <summary markdown="span">:grey_question: Answer</summary> You're right!  :heavy_check_mark:  Binh's observations were collected in a different SRS, known as *NSIDC EASE-Grid Global*, EPSG code *3410* </details>



Now we know a little more about the dataset, we can add it to our project.  The process is similar to adding *Threats_Evidence.csv*, but this time we need to tell QGIS **which map projection** the dataset uses

> 1. `Layer > Add Layer > Add Delimited Text Layer...`
1. Choose source file - click the `...` button and find *GibbonSightings_Survey2.csv*
2. Ensure `Point coordinates` is selected under `Geometry Definition`
3. QGIS will automatically recognise which columns contain the X and Y coordinates from the column names, but we need to **specify the CRS**.  Under `Geometry Definition`, click on the tiny `Select CRS` button on the right-hand edge of the window<details> <summary markdown="span">:framed_picture: Screenshot</summary> <center><a title="Specify CRS when adding Delimited text layer"><img alt="CRS of delimited text layer" src="{{site.baseurl}}/src/img/QGIS_DelimitedText_CRS_em.png"></a></center> </details>
4. Search for *NSIDC* in the `Coordinate Reference System Selector` window - select it and click `OK` <details> <summary markdown="span">:framed_picture: Screenshot</summary> <center><a title="QGIS CRS selector"><img alt="QGIS CRS selector" src="{{site.baseurl}}/src/img/QGIS_CRSSelector_NSIDC-EASE.png"></a></center> </details>
5. Click `Add` and `Close`
6. Check that the new sightings have appeared in the correct place on your map <details> <summary markdown="span">:framed_picture: Screenshot</summary> <center><a title="Sightings from second survey added to QGIS project"><img alt="Sightings from second survey added to QGIS project" src="{{site.baseurl}}/src/img/QGIS_AddSurvey2.png"></a></center> </details>



*[SRS]: Spatial Reference System
*[CRS]: Coordinate Reference System
*[WGS84]: World Geodetic System 1984