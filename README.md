# Shahnama Storyscroll Template

Mobile-friendly, interactive digital image interpretation created using:

* Library of Congress Digital Collection 'Pictorial St. Louis' (https://www.loc.gov/resource/g4164sm.gpm00001/?sp=1)

* Jared Nielson's Pictorial St. Louis (https://github.com/nielsenjared/pictorial-st-louis/blob/master/) (http://jarednielsen.com/pictorial-st-louis/index.html)
* Leaflet (http://leafletjs.com/)
* leaflet-rastercoords (https://commenthol.github.io/leaflet-rastercoords/)
* gdal2tiles-leaflet (https://github.com/commenthol/gdal2tiles-leaflet)

## Check It Out
https://hkeshani.github.io/shahnama-storyscroll/


## Instructions

To change the content, image marker coordinates, and zoom level edit the map.geoson (https://github.com/hkeshani/shahnama-storyscroll/blob/master/map.geojson?short_path=12daef8) file

Enter:

`python gdal2tiles.py -l -p raster -z 0-8 -w none ../map.png ../tiles`


## Credits

* Credit 1

## To Do

* Add text attribution link to index.js & map.geojson
* Fix accuracy of marker zoom
