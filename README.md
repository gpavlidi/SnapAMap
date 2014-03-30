# SnapAMap

SnapAMap is a 1-page app that screenshots a Google Maps map, and saves it locally as a georeferenced JPEG (JPG+aux.xml)

This makes the ortho directly usable with GDAL, QGIS or other GIS software.

This code is provided as is, integrates some popular libraries/html5 features and is meant only as a reference. Use of this code to scrape google Maps imagery, probably violates Google Maps terms of use, and the author holds no responsibility if you choose to do so.

## Usage

- Visit http://rawgithub.com/gpavlidi/SnapAMap/master/snap_singlefile.html
- Pan/Zoom/Change Layer of the map so that it's centered in the desireable location
- Click 'Snap!'
- This will trigger a download of 2 GDAL-compatible files (ortho.jpg and ortho.jpg.aux.xml)

**Tip 1:** If you need a bigger size ortho, you need to make the browser window bigger

**Tip 2:** Use a modern html5-fully compatible browser like latest Chrome, otherwise it might not work

## Goal

The reason behind developing SnapAMap, is that there is no high quality available imagery data for GIS enthusiasts/hobbyists. Some areas in the US are available in USGS website, but it's not convenient since they 're usually grouped into huge half gig image files spanning tenths of kms, making it more difficult to work with, especially if you 're only interested in measuring the roof of your house.


## Not a scraper

SnapAMap is *NOT* a scraper that queries individual map tiles, and mosaics them together, the way most similar software operates.

SnapAMap is using the latest official *Google Maps API* for the imagery access, *canvas* for taking screenshots, *html5 blobs* for saving locally.

Use it at your own risk, and make sure you 're not breaking Google Maps Terms of Use.
