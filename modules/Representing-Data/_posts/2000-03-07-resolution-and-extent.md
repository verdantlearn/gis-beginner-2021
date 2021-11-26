---
title: Resolution & extent
published: false
---

## Resolution and extent

Let's add some more technical words to our growing vocabulary

Resolution
: The level of detail in the dataset, indicating the size of the smallest object you can detect

Imagine you have a landscape or piece of art made up of tiles.  You could make much more detailed pictures from tiny mosaic tiles (1cm across) than large flagstones.  Resolution in raster data is determined by the size of grid cells.  Resolution in vector data is determined by the precision of x,y coordinates i.e. how many decimal places the coordinate has, and therefore the minimum spacing at which you can place adjacent points or vertices

High resolution datasets contain a lot of detail within a given area, for example interview data from individual households, or aerial or drone photography on which you might be able to see individual zebra or animal burrows.  Low resolution datasets have lower detail, for example national-level population counts, or imagery from early satellites such as Landsat (30m grid cells). 

Also known as *grain*, or *frequency*.  I prefer the terms 'fine grain' (think silt or sand) to indicate high resolution, and 'coarse grain' (think boulders or pebbles) for low resolution, as these phrases are more intuitive and easy to remember

Extent
: The area covered by the dataset, also known as *coverage*

Contrast a global dataset (large extent) with data from a single survey location (small extent)

### Contrasting spatial resolutions

Move the slider across the images below to see how the resolution affects the complexity and precision of spatial data

<iframe src="https://verdantlearn.h5p.com/content/1291357976659369267/embed" width="1088" height="637" frameborder="0" allowfullscreen="allowfullscreen" allow="geolocation *; microphone *; camera *; midi *; encrypted-media *"></iframe><script src="https://verdantlearn.h5p.com/js/h5p-resizer.js" charset="UTF-8"></script>

### Spatial *and* temporal 

The terms resolution and extent can be applied to the **temporal dimension** (time) as well as the spatial.  In other words, you can describe a dataset as having high temporal resolution (e.g. observations repeated every minute), or low temporal resolution (e.g. observations spaced many years apart)

<!-- Sort out the use of non-breaking spaces here -->

Dimension  &nbsp; | Property  &nbsp; | Example of a low value &nbsp; | Example of a high value &nbsp; 
---|---|---
Spatial | Resolution | One value per country | Submetre grid cells
Spatial  | Extent | Single survey location | Entire continent
Temporal &nbsp; | Resolution &nbsp; | Every decade | Every minute
Temporal | Extent | Single point in time | Spanning multiple decades


### See it for yourself

<!-- Add instructions on how to download these different types of layers.  Move all the data download instructions to the Resources section, and link to them from here

Is that the way to isolate out the QGIS exercises?  Moving them to a module called QGIS exercises and ordering/labelling them sensibly? -->

To help you understand these concepts, load the following new datasets to your QGIS project:

> 1. <a href="{{site.baseurl}}/src/datasets/OpenStreetMap_CheTao.osm" download>*OpenStreetMap*</a> fine grain vector data: add using `Add Vector Layer...`
1. Coarse-grained data from the *Digital Chart of the World* - select 'Vietnam' and the following two datasets from the [DivaGIS data download page](https://diva-gis.org/gdata):
   1. Roads (shapefile)
   2. Land cover (virtual raster): add using `Add Raster Layer...` or drag & drop the *.vrt* file into your QGIS map view
2. <a href="{{site.baseurl}}/src/datasets/VNM_cov.qml" download>*VNM_cov.qml* QGIS style file</a> for the DCW landcover layer you just downloaded from DivaGIS - save it in the same folder as the *VNM_cov.vrt* and *VNM_cov.grd* files
3. [Chế Tạo Nature Reserve boundary](https://www.protectedplanet.net/555594126) from *Protected Planet*:
   1. Click the green Download button
   2. Select SHP, then Non-Commercial use
   3. Unzip the downloaded file *WDPA_WDOECM_Jun2021_Public_555594126_shp.zip*
   4. Alongside many other folders/files, you’ll now see *WDPA_WDOECM_Jun2021_Public_555594126_shp**_0**.zip*. Unzip this second *.zip* file to extract the contents
   5. You can now add the *.shp* to your QGIS project

<br>

> 1. Compare the visual detail of the **roads** from OSM and DCW
2. Compare the fine-grain Che Tao **Nature Reserve boundaries** from Protected Planet with the corresponding polygon in the IUCN Redlist's *NomascusConcolor_Distribution* layer
3. Compare the two **landcover** raster layers from Copernicus and DCW - consider both their spatial resolution, and how well their landcover classes (thematic values) overlap with each other


<!-- 2. Natural Earth -->
<!-- Information about [Natural Earth](http://www.naturalearthdata.com/) -->


<!-- ### Discuss

> How would you describe this in your own words?  Share below?  Give examples? -->


*[resolution]: Level of detail
*[Resolution]: Level of detail
*[extent]: Area or time period covered
*[Extent]: Area or time period covered
*[OSM]: OpenStreetMap
*[DCW]: Digital Chart of the World
