# Spoorkaarthopper Data

This repository contains the raw OpenStreetMap data for all passenger railway lines in the Netherlands. Spoorkaarthopper automagically creates paths between points on railway lines to be able to reuse later in a variety of applications.

## Source
The original shapefile data is copyright Prorail 2013-2014 and is available No Rights Reserved. The shapefile is called "spoorhart" - this represents the "middle" of the railbed. This data was imported, but then joined and fixed so that there's always just one path between stations. 

## Why on Github?
As part of an open process, this data is completely open. The tools to create path artificats will soon be released also.

## Missing / Future expansions
- All the paths are tagged as roads ('highway="primary"') because of the routing protocol being used. 
- This is missing railway lines in countries other than the Netherlands. OSM might be able to help here for also routing cross-border trips.

