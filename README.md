# Shahnama Storyscroll Template

Mobile-friendly, interactive digital image interpretation created using:

* Digital Bodleian Bodleian Library MS. Ouseley Add. 176 fol.3b (https://www.loc.gov/resource/g4164sm.gpm00001/?sp=1](https://digital.bodleian.ox.ac.uk/objects/bcbfd832-086b-4874-80f8-87500e0de704/)

* Jared Nielson's Pictorial St. Louis (https://github.com/nielsenjared/pictorial-st-louis) (http://jarednielsen.com/pictorial-st-louis/index.html)
* Leaflet (http://leafletjs.com/)
* leaflet-rastercoords (https://commenthol.github.io/leaflet-rastercoords/)
* gdal2tiles-leaflet (https://github.com/commenthol/gdal2tiles-leaflet)

## Check It Out
https://hkeshani.github.io/shahnama-storyscroll/


## Instructions

### Change content, image marker coordinates, and zoom level
Edit the map.geoson  file (https://github.com/hkeshani/shahnama-storyscroll/blob/master/map.geojson?short_path=12daef8).


### Change the image
#### Slice large-sized replacement image into tiles

In a Python programming environment, use the gdal2tiles.py script to create image tiles for your replacement image that are stored in a folder on your pc called "tiles". 
Enter:
gdal2tiles.py -l -p raster -z 0-5 -w none <image> <tilesdir>
(e.g. gdal2tiles.py -l -p raster -z 0-8 -w none ../map.png ../tiles)

#### Delete old tiles folder and upload new one.
## Credits

* Credit 1

## To Do

* Add text attribution link to index.js & map.geojson
* Fix accuracy of marker zoom
