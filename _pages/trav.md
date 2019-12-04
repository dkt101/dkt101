---
permalink: /trav/
title: "Travel and Demographic Trends"
author_profile: true
---
## Resources for Open Data on Population and Travel

Learn about the people. These are the "denominators" to any numbers you produce. For example, say you use the [crash data](https://dkt101.github.io/dkt101/markdown/) to find out your street had 10 crashes last year. Is that a lot? Is it a little? We need to use the _travel patterns_ of the people to determine that! 

If 10 crashes happen every 20 cars, that is a lot more than 10 crashes every 200 cars! This is the power of this page. 

Travel data
### [National Household Travel Survey (NHTS)](https://nhts.ornl.gov/)
This is one of the best (free) options we have for estimating multimodal traffic. Most of the best options are paid and/or private. 
The disadvantage of the NHTS is that it only goes down to urban and rural parts of the state, meaning that the trip counts are not at a city-street level. If you are good with modelling, you can turn this data into street-level.
You would need to make sure your data matches the numbers you pull from NHTS. For example, one would need the total crashes for all urban areas in Maryland as an appropriate numerator, or all crashes in Maryland. 
Ingest multiple years of the survey and conduct more powerful data manipulation with the [Weststat R NHTS](https://github.com/Westat-Transportation/summarizeNHTS) package. One of my favorite variables is TRPTRANS - which shows the mode of travel. Please read the [variable documentation](https://nhts.ornl.gov/assets/codebook.pdf) to better unstand the variables and how they are used. 
[More help documentation for the NHTS here](https://nhts.ornl.gov/documentation.shtml). A [compendum](https://nhts.ornl.gov/compendium) of uses shows examples of how this powerful data can be utilized. There is also a web-based analysis tool [here](https://nhts.ornl.gov/tools.shtml).

![](https://raw.githubusercontent.com/dkt101/dkt101/master/images/nhtssample.PNG)


_Maryland Annual Person Trips by Mode for Urban and Rural Areas_

### [Guide I made about making rough estimates of census demographics for non-standard areas](https://docs.google.com/document/d/1kewfYNpu4Phy5iP5wWS39QggiLr670HWjyCBm4FltW0/edit?usp=sharing)
Use this guide to make a rough estimate of a small area (the example I use is a zone around MICA) demographics. The main assumption is that the distribution of a population in a census block is even  (which it is not, there may be 60% of a census block's population in one small corner of the area). But it is a good start to get oriented to modelling. 

### [State of Maryland Traffic Volume Layers](https://www.arcgis.com/home/item.html?id=3f4b959826c34480be3e4740e4ee025f)
Traffic volume for state roads and many local roads. [Extensive documentation](https://www.roads.maryland.gov/oppen/DSED%20Traffic%20Monitoring%20System%20Program.pdf) on how traffic volumes are calculated at this link. 

### [LandScan Population Density](https://landscan.ornl.gov/)
Requires a login, but it provides a high-resolution (1 sq. KM) distribution of global population data. This means within Baltimore City, you can estimate where most people live at a much smaller level then just using census blocks/tracts. Also has the advantage of being more up to date than similar services like this. 

### [Geocorr Geographic Correspondence Engine](http://mcdc.missouri.edu/applications/geocorr2000.html)
For Census 2000, 2010 data, generate population demographics for several types of standard areas (Travel Analysis Zones, County, CBSA, Metropolitan Area, etc.)

### [CensusScope.org](http://www.censusscope.org/)
An easy-to-use tool for investigating U.S. demographic trends, brought to you by the Social Science Data Analysis Network (SSDAN) at the University of Michigan. With eye-catching graphics and exportable trend data, CensusScope is designed for both generalists and specialists.

### [US Census Grids](https://sedac.ciesin.columbia.edu/data/collection/usgrid)
Based on the NASA EarthData platform (requiring login), Census Grids are an estimation of small-area (less than one sq. mile) population demographics. 

### [Census ZCTA layers for Maryland](https://data.imap.maryland.gov/datasets/eb706b48117b43d482c63d02017fc3ff_1) 
This is a bunch of census variables at the zip-code level that you can use as ready made denominators.
With any population data, be careful. There are some intricate details to analyzing these properly. But you will be good just making crude rates (number of incidents divided by population) for now. Ask me for help as always. 
### [Census Block layers for Maryland](https://geodata.md.gov/imap/rest/services/Demographics/MD_CensusBoundaries/MapServer)
Tons of information about from the census, grouped at the census-block level. 

### [Baltimore Neigborhood Indicators Alliance](https://data-bniajfi.opendata.arcgis.com/)
Data resources from the super analysts at BNIA. GIS-based. Arts and culture, health, safety, demographics, all focused on Baltimore City. 

### [Esri Tapestry Map](https://www.esri.com/en-us/arcgis/products/tapestry-segmentation/zip-lookup)
Get a lot of demographic/market-characteristic data points for your zip code, includes a narrative as well. Great example of taking quanitative data and making it qualitative. 

### [Maryland Vital Statistics](https://geodata.md.gov/imap/rest/services/Health/MD_VitalStatistics/FeatureServer)
Listing of mortality rates.

