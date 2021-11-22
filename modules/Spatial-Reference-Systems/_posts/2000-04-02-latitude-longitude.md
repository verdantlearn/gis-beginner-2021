---
title: Latitude-Longitude
published: false
---

<center><a title="Latitude-Longitude by Djexplo, CC0, via Wikimedia Commons"><img width="512" alt="Latitude and Longitude of the Earth" src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/62/Latitude_and_Longitude_of_the_Earth.svg/512px-Latitude_and_Longitude_of_the_Earth.svg.png"></a></center>

## Angular coordinates: Latitude-Longitude

X,Y coordinates underpin all GIS work, as they encode the location information in all geospatial datasets.  Here we explain Latitude-Longitude coordinates, also known as geographical or angular coordinates

Angular coordinates
: The natural way to specify a location on the surface of a sphere is by using **angles**.  Angular coordinates are the difference in *degrees* from a known reference point (0,0) to the location of interest


### Latitude-Longitude
Latitude and longitude are angular coordinates, with a 0,0 reference point where the prime meridian (through Greenwich in London, England) and the equator intersect.  Hanoi, the capital of Vietnam, is located at 21.03&#176;N, 105.85&#176;E, or roughly 21 degrees north of the equator and 105 degrees east of Greenwich

<!-- 21°01′42″N 105°51′15″E -->

<center><a title="Latitude-Longitude by unknown author, Public domain, via Wikimedia Commons"><img width="400" alt="Latitude-longitude diagram" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ef/FedStats_Lat_long.svg/256px-FedStats_Lat_long.svg.png"></a></center>

Latitude
: Lines of **latitude** form circles drawn at even intervals around the earth, parallel with the equator.  They are known as **parallels**.  The equator is at 0&#176; latitude, the south pole is at 90&#176;S. The distance between parallels is identical everywhere on the earth's surface: about 111km for every 1 degree of latitude

<a title="Latitude parallels by Pearson Scott Foresman, Public domain, via Wikimedia Commons"><img width="300" alt="Latitude parallels" src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/13/Latitude_%28PSF%29.png/512px-Latitude_%28PSF%29.png"></a>

Longitude
: Lines of **longitude** form semi-circles drawn between the poles, like the segments of an orange or the lines on a basketball :basketball:  They are called **meridians**.  The prime meridian is drawn through Greenwich, east London, and other meridians are measured by their angle east or west of the prime meridian, from 180&#176;W (near Hawaii) to 180&#176;E (New Zealand).  Meridians are not parallel; they *converge* at the poles. This means that the straight-line distance between two meridians depends on how close you are to the equator.  For example. 1 degree of longitude is c. 110km at the equator, but only c. 42km at the Antarctic circle (66&#176;30'S).

<a title="Longitude meridians by Pearson Scott Foresman, Public domain, via Wikimedia Commons" ><img width="300" alt="Longitude meridians" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f4/Longitude_%28PSF%29.png/512px-Longitude_%28PSF%29.png"></a>

Note that when you state Latitude-Longitude coordinates, the 'y' coordinate (north/south = Latitude) comes *before* the 'x' coordinate (east/west = Longitude).  This is for historic reasons - the ability to measure latitude from the position of the stars was developed long before people could accurately measure longitude because of the complication of the earth's rotation

<!-- ### H5P quiz
- Use lat-long coordinates to find feature on map - what type of features (click on OSM layer - category in a particular field)
- Give me coordinates of point identified by its attributes (Select by attributes, Zoom to selection)
 -->

*[coordinates]: pair of numbers indicating distance along x and y axes
*[latitude]: north-south angular coordinate measured from equator
*[longitude]: east-west angular coordinate measured from prime meridian
*[SRS]: Spatial Reference System
