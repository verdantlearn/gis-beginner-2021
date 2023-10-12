---
title: QGIS desktop
---

## QGIS desktop

### GUI
Use this interactive guide to familiarise yourself with the main sections of the QGIS GUI

<div id='h5p-qgis-gui'></div>

<!-- <iframe src="https://verdantlearn.h5p.com/content/1291343455090796897/embed" width="1088" height="637" frameborder="0" allowfullscreen="allowfullscreen" allow="geolocation *; microphone *; camera *; midi *; encrypted-media *"></iframe> -->


### Toolbars

**Open QGIS Desktop** (not Browser) on your own computer.  When you first open QGIS, it has many toolbars visible.  To make it easier to find the tools we'll use in this course, and maximise the area available to view your spatial data, let's reduce the panels and toolbars that are visible:
1. Right-click on any part of the toolbars to view the list of panels and toolbars
2. Select the following (see screenshot below) and ensure everything else is unchecked
   1. Panels: 
      1. Layers Panel
   2. Toolbars: 
      1. Attributes Toolbar
      2. Map Navigation Toolbar
      3. Selection Toolbar


<center><img src="{{site.baseurl}}/src/img/QGIS_ToolbarSelection.png" alt="QGIS selecting toolbars"></center>  


Your QGIS window should now look like this.  Here we've positioned the three toolbars separately to make it easy for you to see them, but yours are probably side-by-side, which is fine  

<center><img src="{{site.baseurl}}/src/img/QGIS_SimpleGUI.png" alt="QGIS simpler interface"></center>


*[GUI]: Graphical User Interface
*[panels]: Areas of the main QGIS window - can be hidden
*[toolbars]: Collection of tool buttons - can be hidden or repositioned


<script type="text/javascript">
    const el = document.getElementById('h5p-qgis-gui');
    const options = {
    // 5pJsonPath:  '/h5p-folder',
    // frameJs: '/assets/frame.bundle.js',
    // frameCss: '/assets/styles/h5p.css',
    h5pJsonPath:  '../../../src/h5p/QGIS_GUI',
    frameJs: '../../../src/h5p/standAlonePlayer/frame.bundle.js',
    frameCss: '../../../src/h5p/standAlonePlayer/styles/h5p.css',
    }
    new H5PStandalone.H5P(el, options);

</script>
