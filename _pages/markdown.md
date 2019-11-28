---
permalink: /markdown/
title: "Open Data for Safety"
author_profile: true
redirect_from: 
  - /md/
  - /markdown.html
---
## Resources 

### These links will provide you with a wealth of (mostly Maryland-specific) data related to safety.
#### Crash data are data for all those police reports that are filled out when someone gets in a crash. The data can be very useful.

Prepped Open Crash Data for Baltimore City
:   I prepped some of [open crash data](https://drive.google.com/file/d/1cuNCBIzq7yR3J6R_taZti_EPfQNUGXb5/view?usp=sharing) for Baltimore City (2015-2018) and added some variables of interest. 
:   There is also a smaller version with variable meanings coded [here](https://drive.google.com/file/d/18pvz3Ax62l-Lq2-L9kg6pyYmmShWmKB_/view?usp=sharing)
:   [Crash Data Dictionary](https://opendata.maryland.gov/download/7xpx-5fte/application%2Fvnd.ms-excel) _beware that the circum_person table is not fully accurate_
:   [Guide to make custom crash variables](https://docs.google.com/document/d/1xPGsFjn665qHBwsYTYPGGF_R69Xu6wWwKNkjHnQfjFA/edit?usp=sharing) such as distracted driver, impaired driver, etc. _variable guide currently down, stay turned_
#### _Note_: One Row in the Open Crash Data = One PERSON (person_id) involved in a crash (denoted by report_no). 
#### A vehicle_id can have multiple person_id, but will be blank for a pedestrian. 
#### I created the variable crash_level to denote the highest injured person per report_no (in the crash). Use this if you need to count the number of crashes occuring somewhere. 

## Prepped Open Crash Data for All of Maryland, 2015-Q22019
:   I merged all the quarters for one large dataset for the whole state.  This only includes some 2019 data, as I made this dataset a few months back. Interpeting these data is tricky as I stated above, consult the [Crash Data Dictionary](https://opendata.maryland.gov/download/7xpx-5fte/application%2Fvnd.ms-excel) and [contact me](mailto:dan.knopp@gmail.com) if you have questions.

Example of Using Open Portal Crash Data to Find Injuries on a Specific Road Without GIS, how to Merge Open Crash Data
:   At my previous job, I had a client that wanted to find injuries on I-495. 
:   I [explain here](https://docs.google.com/document/d/1CE2IBrPvPK2txDBRobUe9P1w8ZlypKkZfHvGl95N4mE/edit?usp=sharing) that the GPS coordinates can be input anywhere the officer chooses - in Baltimore, that is _not always_ at the scene of the crash. 
:   If you are only interested in a specific cooridor, start with this method, then correct the plotted crashes in a GIS tool (such as the free [QGIS](https://www.qgis.org/en/site/index.html))

[Guide I made about linking open portal crash data to roadway data](https://docs.google.com/document/d/1STHvhHh65PwbGeCNNunYOYO58hIwqjxNPzAXXWqgJEc/edit?usp=sharing)
:   The advantage of this method is that in older years of Open Portal Crash data, the XY cooridnates are not the only way to plot crashes. You can use GIS software to better plot the crashes based on other fields in the crash data and in the [publically available roadway data](https://data.imap.maryland.gov/datasets/7d88159091854e55a3e6f237fcd45c1a_0). 

[Roadway Safety Analysis Page](https://safety.fhwa.dot.gov/local_rural/training/fhwasa1210/s3.cfm)
:   Lots of good information here. Learn how to make crash rates for a road segment, and other fundamentals of crash trend analysis. 

Other links
:   [NHTSA State Traffic Information System](https://cdan.nhtsa.gov/stsi.htm) Many figures at the state and jurisdiction level. These are built off the data not publically available, so the counts will be higher than open portal. Includes only fatalities, but is broken down by category (impaired, speeding, distracted, pedestrian, etc.) and by county/city.
:   [Maryland Highway Safety Office Benchmarks](http://www.mva.maryland.gov/safety/mhso/benchmark-reports.htm) Learn for each jurisdiction in Maryland the number of crashes, injuries, and fatalities as the result of motor vehicle crashes of all kinds.

