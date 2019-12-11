# Ships Tagging

> Version 2019-12-05

## Geometry

This project aims to tag **ships** in satellite images, using Sentinel-2 imagery (spatial resolution of 10 meters for Red, Green and Blue bands).

Records should be annotated as an **oriented bounding-box** (with orientation going from back to front of ship) or as a rectangle i.e. a **4-vertices polygon**. 

<p align="center"> 
    <img src="resources/ships/sentinel2/geom.png" width="200" height="200" title="Examples of ship geometries">
</p>

## Classes

Every record should be tagged has either **ship**, **marina**, **ship** or **unkown** tag. A marina is a dock or basin with moorings and supplies for yachts and small boats.

The tag **unknow** is used when the user is sure that the object is neither a **ship**, nor a **marina**. This one should not be used very often.

Due to the resolution level, the class of the ship can not be determined with confidence. Only large ships can be seen on Sentinel-2 imagery, reducing type of objects to merchant, large military, large passenger vessels and large barges.

**It is not expected to classify the type of ship.**

## Examples

Find below some examples of ships that can be encountered:

<p align="center"> 
    <img src="resources/ships/sentinel2/ship_1.png" height="200" title="Example of a ship on a Sentinel-2 image">
    <img src="resources/ships/sentinel2/ship_2.png" height="200" title="Example of a ship on a Sentinel-2 image">
</p>
<p align="center">
    <img src="resources/ships/sentinel2/ship_3.png" height="200" title="Example of a ship on a Sentinel-2 image">
    <img src="resources/ships/sentinel2/ship_4.png" height="200" title="Example of a ship on a Sentinel-2 image">
</p>
<p align="center">
    <img src="resources/ships/sentinel2/ship_5.png" height="200" title="Example of a ship on a Sentinel-2 image">
    <img src="resources/ships/sentinel2/ship_6.png" height="200" title="Example of a ship on a Sentinel-2 image">
    <img src="resources/ships/sentinel2/ship_7.png" height="200" title="Example of a ship on a Sentinel-2 image">
</p>
