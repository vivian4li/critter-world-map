critter-world-map
=================

This is the zoomable map used in the Crittercism Geo Performance pages. Users can
click to zoom down from world level to a country displaying first level province
boundaries. In the US an additional zoom level permits zooming in to each state
displaying each county in the states.

Map data is supplied by a number of pre-prepared topojson files for the world,
each country and each US state. These may be built using the Makefile in the
natural-earth directory. Included shapefiles have been downloaded from
http://www.naturalearthdata.com/ and the us-atlas npm project.

The map is intended to be used as a choropleth, permitting each region at each
zoom level to be coloured based on quantized scale.

To test, you'll need to serve the index and json files from an http server
to avoid CORS issues:

python -m SimpleHTTPServer 8000

