---
title: Import field data
---

# Contents
{:.no_toc}

- TOC
{:toc}

---

# Import your own field data

You may need to work on your own field data before they are ready for QGIS.  These instructions assume that you're working with vector data, and that your observations are associated with point locations.  If you need to create lines (e.g. transects) or polygons (e.g. management areas or veg plots), you can do this from point data, or you may be working with tracks saved in your GPS.  If you can't figure out how to work with your data, post in the [community forum](https://community.verdantlearn.org), tagging your new topic with `help-needed`

    :information_source: You *can* store survey locations and detailed observation data (attributes) in two separate files, and add them to QGIS and combine them in separate stages based on a matching field such as Waypoint ID.  However, for beginners *we recommend* that the coordinates and survey information are combined into a single file for simplicity

## Check your data for errors & consistency

Before adding your field observations to QGIS, you need to ensure they are clean and **consistent**.  A good way to check for problems is to open your data in Excel and use the Filter or Pivot Table tools to examine them

1. If you have data from multiple surveys in different sheets of the same Excel file, and they have identical columns, **combine your data** into a single sheet.  This makes the following checks easier, and you can divide them back into separate layers in QGIS later, if necessary
2. Do you have **missing observations**, and are they indicated in the same way throughout the dataset?  QGIS can cope with empty cells, but you can also use a specific code such as *NoData* or *-999*
3. Check that **categorical** :abcd: data are consistent i.e. species/site names or vegetation types are always spelled the same way.  Do you have the correct number of categories?
4. Check that **quantitative** :1234: data make sense.  Try sorting the data, or filtering to show the 10 highest/lowest values.  Are there any extreme values (much lower or higher than expected) which might indicate a misplaced decimal point or typing error?
5. Check that **dates** :date: and **times** :watch: are recorded in a standardised fashion e.g. yyyy-mm-dd, or hh:mm
6. Check that you know which SRS your location **coordinates** :globe_with_meridians: use.  Can you distinguish whether they are Latitude-Longitude, a projected SRS such as a UTM zone, or other national coordinate system?  We will cover SRSs in more detail in module 3, but if you want to add your field data to QGIS at this stage, you need to know their SRS.  Look in your GPS to see what SRS was used when collecting the waypoints, or talk to your field colleagues if you're not sure 
7. Check that all locations are stored using the **same SRS**.  If not, you will need to split your data into a separate file for each SRS, re-project them in QGIS so that they all use the same SRS, and then merge them
8. Save your work before proceeding to the next step!

## Save your data as a text file
Now your data are clean, consistent, and in a single file where possible, you can export them into a format that QGIS can read

>  :warning: Note that saving your Excel spreadsheet as a text file will only save the active sheet, so make sure you have saved your cleaned data as an Excel spreadsheet before this step
> 1. Save your Excel spreadsheet as a *.txt* or *.csv* file, (not the usual *.xls* or *.xlsx*)

## Import your data to QGIS

Now your data are ready to import into QGIS!  To add the text file to your GIS project, you'll need to use a new method.  QGIS won't automatically know where to draw data in *.csv* or *.txt* format, so we have to tell it where the location coordinates are stored

For those of you who are more confident with the basics of using QGIS, here are the steps without screenshots:
> 1. `Layer > Add Layer > Add Delimited Text Layer...`
1. Choose source file - click the `...` button and find your text file
2. Ensure `Point coordinates` is selected under `Geometry Definition`
3. Provided your location columns are labelled as *X* and *Y* or *Latitude* and *Longitude*, QGIS should automatically recognise that they are where the coordinates are stored.  If you have used different column names, you will need to select the correct columns now
4. Click `Add` and `Close`

<br>

For those of you who want more detail or visual instructions, here are the steps including screenshots: 

:warning: Be aware that the csv file in these screenshots is different from yours!

- `Layer > Add Layer > Add Delimited Text Layer...`

<center><img src="{{site.baseurl}}/src/img/add-text-qgis-013.png" alt="QGIS screenshot: Add delimited text layer"></center>

- Choose source file - click the `...` button
<center><img src="{{site.baseurl}}/src/img/add-text-qgis-019.png" alt="QGIS screenshot: Choose text file"></center>

- Ensure `Point coordinates` is selected under `Geometry Definition`, and specify which columns contain the X and Y coordinates 
<center><img src="{{site.baseurl}}/src/img/add-text-qgis-033.png" alt="QGIS screenshot: Specify X and Y columns"></center>

- Click `Add` and `Close`

## Tackling problems

Lean on your [learning community](https://community.verdantlearn.org) if you encounter difficulties - we can help you diagnose what's wrong and move forward


## Next steps
If you'd like to know what else you can do with your point data now they're in QGIS, look at the *Processing points* page in *Resources*


*[SRS]: Spatial Reference System
