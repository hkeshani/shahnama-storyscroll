# Shahnama Storyscroll Template

Mobile-friendly, interactive digital image interpretation created using:

* Digital Bodleian Bodleian Library MS. Ouseley Add. 176 fol.3b (https://www.loc.gov/resource/g4164sm.gpm00001/?sp=1](https://digital.bodleian.ox.ac.uk/objects/bcbfd832-086b-4874-80f8-87500e0de704/)

* Jared Nielson's Pictorial St. Louis (https://github.com/nielsenjared/pictorial-st-louis) (http://jarednielsen.com/pictorial-st-louis/index.html)
* Leaflet (http://leafletjs.com/)
* leaflet-rastercoords (https://commenthol.github.io/leaflet-rastercoords/)
* gdal2tiles-leaflet (https://github.com/commenthol/gdal2tiles-leaflet)

## Check It Out
Example Storyscroll: https://hkeshani.github.io/shahnama-storyscroll/

Your Storyscroll: https://(your-username-here).github.io/(your-project-name-here)/

# Instructions

This repository contains a variety of files in various languages and you will update them accordingly to create your project.

Files you will need to change:

* README.md - Markdown script, change the storyscroll link
* index.html - HTML language, creates the overall structure of the web page
* style.css - CSS language, contains styling elements relevant for index.html
* index.js - handles the scripts for the moving elements in index.html
* map.geojson - contains all the elements that will be displayed in the scrolling sidebar
* img (folder) - contains your images to be displayed in the scrolling sidebar
* tiles (folder) - contains the sliced images used to display the manuscript 
* LICENSE - MIT's digital license

Files you do not change:

* rastercoords.js - scripts to handle image zoom
* markers (folder) - contains assets for clickable markers

## 1. Uploading the manuscript image
###  **Slice large-sized replacement image into tiles**

In a Python programming environment, use the gdal2tiles.py script to create image tiles for your replacement image that are stored in a folder on your pc called "tiles". 
Enter:
gdal2tiles.py -l -p raster -z 0-5 -w none <image> <tilesdir>
(e.g. gdal2tiles.py -l -p raster -z 0-8 -w none ../map.png ../tiles)

### **Delete old tiles folder and upload new one.**

**this needs instructions, I would want students to use git to upload tiles for simplicities sake, but I don't know how much you want the students to do.

## 2.  Updating documentation and setting up your project

1. Deploying github pages remote hosting for website: Head to your repository on github.com and go to Settings>Pages>
2. readme link
3. index.html  site title
4. LICENSE - name and year
5. index.js - image size

## 3. Change storyscroll content, image marker coordinates, and zoom level
Edit the map.geoson  file (https://github.com/hkeshani/shahnama-storyscroll/blob/master/map.geojson?short_path=12daef8).

## Credits

* Credit 1