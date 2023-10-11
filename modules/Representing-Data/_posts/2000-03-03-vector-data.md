---
title: Vector
---

## Vector data model

The vector data model is best for modeling **discrete objects** which have clearly defined boundaries and can be counted

Examples of vector features:
- Coral reefs :tropical_fish:
- Point sources of pollution :factory:
- Individual trees or patches of wetland :evergreen_tree:
- Animal movement tracks from GPS collars :paw_prints:
- Areas affected by fire or clear-felling :fire:


Vector data come in three spatial forms: **point, line and polygon**.  Each vector feature can have multiple attributes

Points
: One-dimensional feature with a single x and y coordinate (vertex)
This example contains 3 points

<iframe width="100%" height="395" frameborder="0"
  src="https://observablehq.com/embed/7405053fb2a50cc7?cells=pointsPlot%2CpointsTable"></iframe>


Lines
: Linear two dimensional feature composed of a series of x and y coordinates (vertices)

This example contains a single line made from 4 vertices

<iframe width="100%" height="418" frameborder="0"
  src="https://observablehq.com/embed/7405053fb2a50cc7?cells=linesPlot%2ClinesTable"></iframe>

Polygons
: Two dimensional feature composed of sequence of x and y coordinates (vertices) where the first and last vertex are identical, creating a closed area  

This example contains a single polygon made from 9 vertices

<img src="{{site.baseurl}}/src/img/polygon.svg" alt="Polygon">


Vector attributes
: Information about a feature or record, stored in columns in the attributes table

> If you've followed the instructions to import your own dataset from a text file, you've created vector data - points, which can be connected into lines and or polygons.  You can also add other field observations as attribute information

### Quiz: Vector data model

Test your new knowledge with our mini quiz!  :heavy_check_mark:

<iframe src="https://verdantlearn.h5p.com/content/1291353958466496357/embed" width="1088" height="637" frameborder="0" allowfullscreen="allowfullscreen" allow="geolocation *; microphone *; camera *; midi *; encrypted-media *"></iframe>

<script src="https://verdantlearn.h5p.com/js/h5p-resizer.js" charset="UTF-8"></script>


*[feature]: A record - a single point, line or polygon
*[vertex]: x,y coordinates of the point where two lines meet
*[vertices]: Plural of vertex
*[attribute]: Property of a vector feature, or value in a raster cell
*[attributes]: Properties of a vector feature, or value in a raster cell


<!-- Improve quiz - create Dialog cards 
Use the same examples but find pictures to represent them, and put in point/line/polygon image on back of card
-->

<!-- Observable: Fix polygons, include table of coordinates plus hover-over of coordinates -->

<!-- Can I use sparklines in observable (or Jekyll!?) to illustrate points, lines, polys?
https://observablehq.com/@maxim-k/sparkline
https://observablehq.com/@akngs/sparklines
https://observablehq.com/@kgryte/stdlib-unicode-sparkline-column-chart
https://observablehq.com/@oliviafvane/branching-sparklines-line-graphs -->
