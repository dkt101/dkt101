---
permalink: /enviro/
title: "Environmental Data"
author_profile: true
---
## Good Sources of Satellite, Terrain, LIDAR, etc. 

One of my favorte things to when making maps is to utilize the wealth of open data that comes from satellites. The team at [iMAP Maryland](https://imap.maryland.gov/Pages/default.aspx) provides so much of this for free.

I use these layers for some technical things and some routine items. I may check how a construction project is progressing back in my hometown with [Sentinel Hub](https://www.sentinel-hub.com/explore/eobrowser)'s daily planet imagery.

![](https://github.com/dkt101/dkt101/blob/master/images/threeinharbor.png)

### [Maryland iMAP imagery layers](https://geodata.md.gov/imap/rest/services/Imagery) 
There are a few options - three inch (not available for all areas but super high resolution), six-inch (great resolution, statewide coverage), and NAIP (historical, pretty good resolution). All these are a great source of high resolution imagery you can use in any way you see fit. For analysis, I prefer the NAIP imagery layers as they usually are taken in Winter (no trees) and have been taken for over a decade (good for measuring change). I also prefer to deal with the "feature layers" instead of the imagery layers. But if you need help deciding how to deal with this stuff, as always [contact me](mailto:dan.knopp@gmail.com).
If you do not feel comfortable downloading the imagery - just click [ArcGIS Online Map Viewer] and then on the map that pops up, click the pushpin, scroll to the bottom of the box that pops up, and click the [map](https://geodata.md.gov/imap/rest/services/Imagery/MD_SixInchImagery/MapServer?f=jsapi) in the box at the bottom. 
### [Maryland iMAP's LIDAR Data](https://imap.maryland.gov/Pages/lidar.aspx) 
is filled with free data on topography, LIDAR for the whole state, and digital elevation models (DEMs)
Think of this data source as your own free "Google Terrain" layer on Maps, but much more detailed. I used this data to advocate for changes in my neighborhood, where I felt drivers could not see pedestrians due to a hill. I also use the DEM layer to "calibrate" satellite imagery so that I can measure changes in impervious surface over time.  [You can also view it online without downloading](https://geodata.md.gov/topoviewer)
### [NASA EarthData](https://earthdata.nasa.gov/earth-observation-data). 
You need to make a free login, but this site has tons of imagery like Maryland iMap, but even more (things like vegitation indexes - where vegetaion is at). Also worldwide. Lower res than Maryland's iMap. 
### [OpenAerialMap](https://openaerialmap.org/) 
Has a bunch of random drone maps produced by people, including in Baltimore. 
### [Maps Made Easy](https://www.mapsmadeeasy.com/)
Another site with the ability to freely process drone imagery. Unlimited storage and resolution for small operations. The commercial drone mapping products (Pix4d, Agisoft, etc.) are hundreds of dollars. 
### [Sentinel Hub](https://www.sentinel-hub.com/explore/eobrowser) 
This is a good resrouce for daily satellite imagery. The nicest part is that with their tool you can view the date range of your choice and use playback controls.  


[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=JNTCNMTCW7PZY)
