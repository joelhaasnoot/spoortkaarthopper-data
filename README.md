# Spoorkaarthopper Data

**License:** CC-0

This repository contains the raw OpenStreetMap data for all passenger railway lines in the Netherlands. When combined with [Spoorkaarthopper](https://github.com/joelhaasnoot/spoorkaarthopper), you can automagically preprender paths between points on railway lines to be able to reuse later in a variety of applications.

## Source
The original shapefile data is copyright Prorail 2013-2014 and is available No Rights Reserved. The shapefile is called "spoorhart" - this represents the "middle" of the tracks. That appears to not always be true: this data was converted to OSM, but then joined and fixed so that there's always just one path between stations. 

## Why on Github?
As part of an open process, this data is completely open. The tools to create path artifacts are available in the seperate [Spoorkaarthopper](https://github.com/joelhaasnoot/spoorkaarthopper) repository. A third respository [spoorkaarthopper-tools](https://github.com/joelhaasnoot/spoorkaarthopper-tools) contains python scripts for conversions.

## Missing / Future expansions
- All the paths are tagged as roads ('highway="primary"') because of the routing being used.
- This is missing railway lines in countries other than the Netherlands. The HSL/high speed line to Belgium ends just before Antwerp. Several train connections originate or terminate in the Netherlands but won't be fully visuble. OSM might be able to help here for also routing cross-border trips.