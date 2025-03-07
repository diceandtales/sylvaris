---
map_height_y: 4095
map_width_x: 4095
scale_pixels: 250
scale_pixels_range: 2
mapCalc1: 0.008
---

> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`


```leaflet  
id: Oroka ### Must be unique with no spaces  
image: [[oroka_island.png]] ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [4095, 4095]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 600px ### Size of the leaflet embed in px on your screen  
width: 95% ### Size of the leaflet embed in your note  
lat: 2047.5 ### To center the map, make this half of the map height.  
long: 2047.5 ### To center the map, make this half of the map width.  
minZoom: -3 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 1 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -2.75 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.25 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.008 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: false ### marker
```


















# Oroka Island

















### Watabou Link
https://watabou.github.io/perilous-shores/?seed=1378870540&tags=civilized,island,safe,woodland,lawful,lowland&hexes=1


