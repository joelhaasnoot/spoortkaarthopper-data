# Spoorkaarthopper Data

**License:** CC-0

This repository contains the raw OpenStreetMap data for all passenger railway lines in the Netherlands. When combined with [Spoorkaarthopper](https://github.com/joelhaasnoot/spoorkaarthopper), you can automagically preprender paths between points on railway lines to be able to reuse later in a variety of applications.

## Releases
Check the "Releases" link above to find the latest spoorkaarthopper output to form a Dutch railwaymap. Or click here for the __[latest version, 1.5](https://github.com/joelhaasnoot/spoortkaarthopper-data/releases/download/v1.5/output-1.5-20130104.zip)__

## Source
The original shapefile data is copyright Prorail 2013-2014 and is available No Rights Reserved. The shapefile is called "spoorhart" - this represents the "middle" of the tracks. That appears to not always be true: this data was converted to OSM, but then joined and fixed so that there's always just one path between stations. 

## Other files
The folder *routing-input* contains two other files that are important inputs for the output of Spoorkaarthopper (these are the ones used for my version):

- `locations.csv`: contains a list of all train stations in the Netherlands and their GPS/WGS84 locations. Almost the same as the list from the NS API - but with a few additions at the end.

- `pairs.csv`: contains a list of all lines between stations and is used as the input of pairs to route between. Source for this list is manual work by Justin Stook (thanks!). This list is mostly unique, but contains some duplicates to facilitate better routing near Amsterdam Sloterdijk, Duivendrecht and some other exceptions.

## Why on Github?
As part of an open process, this data is completely open. The tools to create path artifacts are available in the seperate [Spoorkaarthopper](https://github.com/joelhaasnoot/spoorkaarthopper) repository. A third respository [spoorkaarthopper-tools](https://github.com/joelhaasnoot/spoorkaarthopper-tools) contains python scripts for conversions.

## Missing / Future expansions
- All the paths are tagged as roads ('highway="primary"') because of the routing being used.
- This is missing railway lines in countries other than the Netherlands. The HSL/high speed line to Belgium ends just before Antwerp. Several train connections originate or terminate in the Netherlands but won't be fully visible. OSM might be able to help here for also routing cross-border trips.