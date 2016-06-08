<div align="Center">
## Making Library and Archives Canada (LAC) fire insurance plans (FIP) more easily accessible
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/cover.jpg "Cover")<br>
by Rebecca Bartlett & Joel Rivard

Carleton University Library

---
##Outline

 - Introduction to the problem
 - Our amazing (yet, time-consuming) solution!!!
 - Moving forward and discussion

---

##Have you ever tried finding and/or using FIP from LAC?

---
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_searchresults.jpg "Searching")

---

![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_search.jpg "Search")

---
![Frustrated](http://cu-library.github.io/carto-2016/images/frustrated.jpg "Frustrated")

Source: https://c2.staticflickr.com/4/3451/3986997574_5aa55585a4.jpg

---

## Introduction to the problem
Finding FIP's through LAC's website is

  - Slow
  - At times, inaccurate
  - Time-consuming
---

## Collection

We choose the
<br<br>

**Insurance plan of the city of Ottawa, Canada, and adjoining suburbs and lumber districts, January 1888, revised January 1901**

<br><br>
It included 113 sheets on LAC's website

---

## Solution

Ryder to the rescue!!

![Ryder superhero](http://cu-library.github.io/carto-2016/images/superhero.jpg "Superhero")

source: https://pixabay.com/static/uploads/photo/2012/04/24/21/21/superhero-40908_960_720.png
---
## Solution

- Georeference the FIP individual sheets (keymap not accurate)
- This will give us our index + the georeferenced plans
<br><br>

Win Win Situation!!
---
## Methodology

80 map sheets had fire insurance plans of specific geographic areas
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/regular_sheet.jpg "FIP Regular Sheet")

---
## Methodology

22 map sheets showed multiple fire insurance plans of different areas
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/split_sheet.jpg "FIP Split-up")

These were clipped using Powerpoint and saved as .png. Graphics software we had couldn't freehand clip.
---
## Methodology

11 sheets weren't maps (keymaps or street index)
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/keymap_sheet.jpg "FIP keymap")
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/index_sheet.jpg "FIP Index")

---
## Methodology

- In ArcMAp, used the georefencing toolbar to add roughly 8-12 ground control points.
- Used multiple referencing layers:
  - 1928 air photos from the city of ottawa
  - Current Ottawa-Gatineau open data streetfile (downloaded from city of Ottawa and ville de Gatineau)
- Georeferenced the FIP to MTM zone 9
---
## Potential Issues

- Source data used is at least 30 years more up-to-date than year of FIP
- No data-frame or coordinate system used in FIP

---
## Creating the Index
- Once the fire insurance plans were georeferenced, we created the index in ArcMap:
  1. Created a personal Geodatabase and created an empty mosaic dataset in it
  2. Added the FIP rasters to the mosaic dataset (this built footprints, but not accurate)
  3. Used the build footprints tool to make the index perfectly around each of the rasters
  4. Exported the footprints layer from the mosaic dataset in the table of contents

- For each polygon, added a link to that particular sheet on LAC's website
- Used ArcGIS Online to host the index
---
![Fire Insurance Plans overlap](http://cu-library.github.io/carto-2016/images/new_index.jpg "FIP Index online")
http://carleton-u.maps.arcgis.com/apps/PublicInformation/index.html?appid=46165bbabf3741f6b9d9427d3d87c22a
---
![Fire Insurance Plans overlap](http://cu-library.github.io/carto-2016/images/fip_overlap.jpg "FIP Index in ArcGIS Pro")

---
![Fire Insurance Plans overlap zoom](http://cu-library.github.io/carto-2016/images/fip_overlapzoom.jpg "FIP Index in ArcGIS Pro zoom")

---
## Next Step
  - Allow users to download the georeferenced images (Copyright Issues)
  - Tackle another year or another geographic area for FIP
  - Create kml files

---
## Questions

Rebecca Bartlett - GIS and Digital Resources Librarian

Joel Rivard - Cartographic Specialist

gis@carleton.ca
