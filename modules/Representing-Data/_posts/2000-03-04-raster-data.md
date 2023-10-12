---
title: Raster
---

## Raster data model

The raster data model is best for modeling properties which **vary continuously** across the landscape, and can be measured at any location

Examples of raster features from field surveys or remote sensing:
- Soil type or vegetation class :evergreen_tree: :deciduous_tree:
- Elevation :mountain:
- Plant density :ear_of_rice:
- Ice depth :snowflake:
- Vegetation productivity :seedling: :fallen_leaf:
- Suitability or risk :radioactive:

A raster dataset is composed of a **uniform grid** of identically-sized cells (usually square), with each cell (or pixel) holding a single numeric value

Raster attributes
: Raster attributes are about the variable at that location, stored as a cell value.  Each grid cell can only store a single value, so if multiple attributes need to be stored (e.g. elevation *and* slope), multiple rasters are needed, which are sometimes bound together in a raster stack

Rasters values can be:
- **Quantities** - *continuous* variables such as rainfall or density.  The DEM we'll use below is an example of a continuous raster
- **Thematic** - *categories* such as vegetation class, presence/absence of a species, represented by a numerical code

> The LandCover dataset you downloaded is an example of a thematic raster - each pixel contains a code indicating the landcover class at that location

If you're using the gibbon datasets, these are the land cover classes that occur in and around Che Tao Nature Reserve:[^1] 

Code &nbsp; | &nbsp; Landcover class
---:|---
20 &nbsp; | &nbsp; Shrubs
30 &nbsp; | &nbsp; Herbaceous vegetation
40 &nbsp; | &nbsp; Cropland
50 &nbsp; | &nbsp; Urban
80 &nbsp; | &nbsp; Permanent water bodies
90 &nbsp; | &nbsp; Herbaceous wetland
111 &nbsp; | &nbsp; Closed forest, evergreen needle leaf
112 &nbsp; | &nbsp; Closed forest, evergreen broad leaf
114 &nbsp; | &nbsp; Closed forest, deciduous broad leaf
116 &nbsp; | &nbsp; Closed forest, unknown
122 &nbsp; | &nbsp; Open forest, evergreen broad leaf
126 &nbsp; | &nbsp; Open forest, unknown

<img src="{{site.baseurl}}/src/img/RasterExample.png" alt="Landcover as an example of a thematic raster">

### Quiz: Raster data model

Here's another quick quiz!  :heavy_check_mark:

<div id='h5p-raster-data-types'></div>

<!-- <iframe src="https://verdantlearn.h5p.com/content/1291354595816641297/embed" width="1088" height="637" frameborder="0" allowfullscreen="allowfullscreen" allow="geolocation *; microphone *; camera *; midi *; encrypted-media *"></iframe> -->

[^1]: Download the complete list of <a href="{{site.baseurl}}/src/datasets/LandCover_ClassDefinitions.pdf" download>Copernicus land cover classes</a>

*[pixel]: Single cell in a raster grid
*[DEM]: Digital Elevation Model
*[attribute]: Property of a vector feature, or value in a raster cell


<script type="text/javascript">
    const el = document.getElementById('h5p-raster-data-types');
    const options = {
    // 5pJsonPath:  '/h5p-folder',
    // frameJs: '/assets/frame.bundle.js',
    // frameCss: '/assets/styles/h5p.css',
    h5pJsonPath:  '../../../src/h5p/RasterDataTypes',
    frameJs: '../../../src/h5p/standAlonePlayer/frame.bundle.js',
    frameCss: '../../../src/h5p/standAlonePlayer/styles/h5p.css',
    }
    new H5PStandalone.H5P(el, options);
</script>

<!-- 
<script src="https://verdantlearn.h5p.com/js/h5p-resizer.js" charset="UTF-8"></script>
 -->
