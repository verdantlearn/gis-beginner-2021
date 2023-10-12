---
title: Resolution & extent
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

A global dataset (large extent) and data from a single survey location (small extent) are at opposite ends of this spectrum

## Contrasting spatial resolutions

Move the slider across the images below to see how the resolution affects the complexity and precision of spatial data

<div id='h5p-spatial-res-juxtaposition'></div>

### Spatial *and* temporal 

The terms resolution and extent can be applied to the **temporal dimension** (time) as well as the spatial.  In other words, you can describe a dataset as having high temporal resolution (e.g. observations repeated every minute), or low temporal resolution (e.g. observations spaced many years apart)

<!-- Sort out the use of non-breaking spaces here -->

Dimension  &nbsp; | Property  &nbsp; | Example of a low value &nbsp; | Example of a high value &nbsp; 
---|---|---
Spatial | Resolution | One value per country | Submetre grid cells
Spatial  | Extent | Single survey location | Entire continent
Temporal &nbsp; | Resolution &nbsp; | Every decade | Every minute
Temporal | Extent | Single point in time | Spanning multiple decades


## See it for yourself

<!--Move all the data download instructions to the Resources section, and link to them from here

Is that the way to isolate out the QGIS exercises?  Moving them to a module called QGIS exercises and ordering/labelling them sensibly? -->

To help you understand these concepts, add some new datasets to your QGIS project

### OpenStreetMap

You have already added a tiled raster basemap from OpenStreetMap (OSM) to your project.  However, all of the fine grained vector data used to create that basemap can be downloaded and used direct, for example if you wish to only display unsurfaced roads, or particular types of buildings

> 1. Go to [OpenStreetMap](https://www.openstreetmap.org/) and click on the `Export` button at the top left of the screen
1. Type in your bounding coordinates (North, East, South, West) in the top left.  If you have specified small geographic extent, a blue `Export` button will appear
2. If you need a larger area, choose one of the repositories listed in the bottom left of that OpenStreetMap page instead
3. Alternatively, you can download <a href="{{site.baseurl}}/src/datasets/OpenStreetMap_CheTao.osm" download>*OpenStreetMap*</a> fine grain vector data for Che Tao
4. Add the OSM using `Add Vector Layer...`

### Digital Chart of the World
DCW provides coarse grained vector and raster data at country level

> 1. Go to the [DivaGIS data download page](https://diva-gis.org/gdata), select your country of interest and download the layers that are useful to you, for example:
   1. Roads (shapefile)
   2. Land cover (virtual raster): add using `Add Raster Layer...` or drag & drop the *.vrt* file into your QGIS map view
1. You can use the <a href="{{site.baseurl}}/src/datasets/VNM_cov.qml" download>*VNM_cov.qml* QGIS style file</a> for the DCW landcover layer you just downloaded from DivaGIS - save it in the same folder as your *.vrt* and *.grd* files and rename it to match the files you downloaded.  For example, rename it *VNM_cov.qml* if your landcover layer is called *VNM_cov.grd*

### Protected Planet
You can download the boundaries of protected areas from Protected Planet

:warning: The boundaries may not always reflect the situation on the ground.  Protected Planet uses the World Database of Protected Areas (WDPA) as its source, and national or regional governments may not have provided the most detailed or recent information to WDPA  

1. [Chế Tạo Nature Reserve boundary](https://www.protectedplanet.net/555594126) from *Protected Planet*:
   1. Click the green Download button
   2. Select SHP, then Non-Commercial use
   3. Unzip the downloaded file *WDPA_WDOECM_Jun2021_Public_555594126_shp.zip*
   4. Alongside many other folders/files, you’ll now see *WDPA_WDOECM_Jun2021_Public_555594126_shp**_0**.zip*. Unzip this second *.zip* file to extract the contents
   5. You can now add the *.shp* to your QGIS project using `Add Vector Layer...`

<br>

Now you have added a variety of layers to your project, examine the contrast between coarse and fine grain in more detail:

> 1. Compare the visual detail of the **roads** from OSM and DCW
1. Compare the fine grained Che Tao **Nature Reserve boundaries** from Protected Planet with the corresponding polygon in the IUCN Redlist's *NomascusConcolor_Distribution* layer
2. Compare the two **landcover** raster layers from Copernicus and DCW.  Consider both their spatial resolution, and the amount of overlap in their landcover class definitions (thematic values)


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

<script type="text/javascript">
    const el = document.getElementById('h5p-spatial-res-juxtaposition');
    const options = {
    // 5pJsonPath:  '/h5p-folder',
    // frameJs: '/assets/frame.bundle.js',
    // frameCss: '/assets/styles/h5p.css',
    h5pJsonPath:  '../../../src/h5p/SpatialRes_Juxtaposition',
    frameJs: '../../../src/h5p/standAlonePlayer/frame.bundle.js',
    frameCss: '../../../src/h5p/standAlonePlayer/styles/h5p.css',
    }
    new H5PStandalone.H5P(el, options);
</script>