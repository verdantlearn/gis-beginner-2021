---
title: Choosing an SRS
---

## Choosing an SRS

So how do you **choose a suitable SRS** for your own geospatial datasets and GIS projects? :thinking:


Some questions to consider:
1. What type of **coordinates** do you use in your fieldwork?  Latitude-Longitude, or a projected coordinate system?
2. If projected, do you know the name of the **map projection** you use?
3. Do you know which **datum** that map projection uses?
4. Are all of your spatial datasets in the **same SRS**?

You can find out about relevant SRSs from a variety of sources:
- Ask colleagues or friends who work in the same geographic area as you
- Local topographic or road maps on paper - see the legend, or look at the coordinate numbers in the map margins
- Search online for information about your geographic area, e.g. national mapping agency
- Look on the [Spatial Reference website](http://www.spatialreference.org/)
- Try the [EPSG map search](https://epsg.org/search/map)
- Try adding your existing geospatial datasets to QGIS - open the layer `Properties` to see what QGIS thinks their SRS is

For more advice on appropriate map projections for different areas of the world, see ESRI's help page [Choosing a map projection](https://desktop.arcgis.com/en/arcmap/latest/tools/coverage-toolbox/choosing-a-map-projection.htm)

Now think about why you use that SRS.  For example:
- You've been advised to by others more knowledgeable in GIS :nerd_face:
- Simplicity of understanding coordinates :thought_balloon:
- Easier to estimate distances between locations on the ground :straight_ruler:
- For compatibility with legacy geospatial data such as old survey records :triangular_ruler:
- For compatibility with online data sources :desktop_computer:
- To allow spatial analysis :eight_spoked_asterisk:

Post a response in the community forum:
1. What spatial reference system(s) do you use, and why?
2. Will you change the SRS you're using based on what you've learned in this module?

<div id='discourse-comments'></div>

<script type="text/javascript">
  window.DiscourseEmbed = { discourseUrl: 'https://community.verdantlearn.org/', topicId: 721 };

  (function() {
    var d = document.createElement('script'); d.type = 'text/javascript'; d.async = true;
    d.src = window.DiscourseEmbed.discourseUrl + 'javascripts/embed.js';
    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(d);
  })();
</script>


*[coordinates]: pair of numbers indicating distance along x and y axes
*[projection]: 
*[datum]: model of the earth's shape
*[SRS]: Spatial Reference System

<!-- Theory/comparisons/resources e.g. EPSG -->
<!-- Use <EPSG org?> to find out the EPSG code -->
