# Wind turbine tagging 

## Geometry


Wind turbines in the imagery should be identified with 3-points polygons. The polygon should be drawn with the following method: 

• Point 1 = top of the wind turbine \
• Point 2 = base of the wind turbine \
• Point 3 = top of the shadow 


<p align="center"> 
<img src="ressources_wt/geom.png" width="200" height="200" title="hover text">
</p>

## Classes

The wind turbine should be classified into the following 3 categories: 

• **Wind Turbine** 

If the object is clearly seen, you should only select the **Wind Turbine** annotation.

<p align="center"> 
<img src="ressources_wt/wt_only.png" width="150" title="hover text">
</p>


<p align="center"> 
<img src="ressources_wt/wt_tag.png" width="400" title="hover text">
</p>

<p align="middle"> 
<img src="ressources_wt/wt2.png" width="200" height="200" title="hover text" >
<img src="ressources_wt/tag.png" width="200" height="200"  title="hover text">

</p>

• **Wind Turbine without shadow** 

<p align="center"> 
<img src="ressources_wt/shadow_tag.png" width="150" title="hover text">
</p>


Sometimes, the shadow does not appear in the imagery (most of the time due to the clouds). You should select two annotations for the object: **Wind Turbine** and **Without shadow**.

Concerning the geometry, you should draw the polygon starting from the top of the object, then the base and guess where should be the last point according to others wind turbines next to the object in the imagery. Indeed all the shadows on an imagery have the same direction. 


<p align="center"> 
<img src="ressources_wt/clouds.png" width="200" height="200" title="hover text">
</p>


• **Wind Turbine without body**

<p align="center"> 
<img src="ressources_wt/wt.png" width="150" title="hover text">
</p>


It is sometimes difficult to see the body of the wind turbine. In this case, you should select two annotations for the object: **Wind Turbine** and **Without body**.

Concerning the geometry, you should guess the first point (even if you are not sure) and complete the polygon with the base and the top of the shadow.
 
 <p align="center"> 
<img src="ressources_wt/body.png" width="200" height="200" title="hover text">
</p>


## Important notes

**Discard** any wind turbine that is truncated at the border of the imagery. **Do not discard** a wind turbine that is not fully visible for other reasons (i.e. partially covered by a cloud).

Sometimes the object is **not completely in the AOI** (Aera Of Interest). If almost one of the three points of the polygon is in the zone, you should annotate it.

 <p align="center"> 
<img src="ressources_wt/aoi.png" width="200" height="200" title="hover text">
<img src="ressources_wt/aoi2.png" width="200" height="200" title="hover text">
</p>


Moreover, the top of the object, the base and the top of the shadow can be aligned. You should draw the polygon with the three points even if it is not a triangle. 

 <p align="center"> 
<img src="ressources_wt/aligned.png" width="200" height="200" title="hover text">

</p>
