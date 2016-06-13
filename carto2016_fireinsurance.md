<div align="Center">
## Making Library and Archives Canada (LAC) fire insurance plans (FIPs) more easily accessible
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/cover.jpg "Cover")<br>
by Rebecca Bartlett & Joel Rivard

Carleton University Library

---
##Outline

 - Introduction to the problem
 - Our amazing (yet time-consuming) solution!!!
 - Moving forward and discussion

---

##Have you ever tried finding and/or using FIPs from the LAC website?

---
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_searchresults.jpg "Searching")

---

![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_search.jpg "Search")

---
![Frustrated](http://cu-library.github.io/carto-2016/images/frustrated.jpg "Frustrated")

Source: https://c2.staticflickr.com/4/3451/3986997574_5aa55585a4.jpg

---

## Introduction to the problem
Finding FIPs through LAC's website is

  - Slow
  - Inaccurate at times
  - Time consuming
---

## Collection

We choose the
<br<br>

**[Insurance plan of the city of Ottawa, Canada, and adjoining suburbs and lumber districts, January 1888, revised January 1901](http://collectionscanada.gc.ca/pam_archives/index.php?fuseaction=genitem.displayEcopies&lang=eng&rec_nbr=3816143&rec_nbr_list=2133082,2132980,3816143,3816060,3827541,3827543,3827534,3824226,3816030,3827571&title=Insurance+plan+of+the+city+of+Ottawa%2C+Canada%2C+and+adjoining+suburbs+and+lumber+districts%2C+January+1888%2C+revised+January+1901.+&ecopy=e010689183-v8&back_url=())**

<br><br>
It included 113 sheets on LAC's website

---

## Solution

Ryder to the rescue!!

![Ryder superhero](http://cu-library.github.io/carto-2016/images/superhero.jpg "Superhero")

Source: https://pixabay.com/static/uploads/photo/2012/04/24/21/21/superhero-40908_960_720.png
---
## Solution

- Georeference the FIP individual sheets (keymap not accurate)
- This will give us our index + the georeferenced plans
<br><br>

Win-Win Situation!!
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

- In ArcMap 10.3, used the georeferencing toolbar to add roughly 8-12 ground control points per FIP
- Used multiple referencing layers:
  - 1928 air photos from the City of Ottawa
  - Current Ottawa-Gatineau open data street files (downloaded from [City of Ottawa](http://data.ottawa.ca/dataset/roads) and [Ville de Gatineau](http://www.gatineau.ca/donneesouvertes/fiche_metadonnees_en.aspx?id=872107914))
- Georeferenced the FIPs to MTM Zone 9
---
## Potential Issues

- Source data used to georeference is at least 30 years more up-to-date than year of FIPs
- No data frame or coordinate system was used in FIPs

---
## Creating the Index
- Once the fire insurance plans were georeferenced, we created the index in ArcMap:
  1. Created a personal geodatabase and added an empty mosaic dataset
  2. Added the FIP rasters to the mosaic dataset (this built footprints, but was not accurate)
  3. Used the [Build Footprints tool](http://desktop.arcgis.com/en/arcmap/10.3/tools/data-management-toolbox/build-footprints.htm) to make the index polygons fit perfectly around each of the rasters
  4. Exported the footprints layer from the mosaic dataset

- In the attribute table, added a URL link for each polygon to the corresponding sheet on LAC's website
- Used ArcGIS Online to host the index
---
![Fire Insurance Plans overlap](http://cu-library.github.io/carto-2016/images/new_index.jpg "FIP Index online")
http://carleton-u.maps.arcgis.com/apps/PublicInformation/index.html?appid=46165bbabf3741f6b9d9427d3d87c22a
---
![Fire Insurance Plans overlap](http://cu-library.github.io/carto-2016/images/fip_overlap.jpg "FIP Index in ArcGIS Pro")

---
![Fire Insurance Plans overlap zoom](http://cu-library.github.io/carto-2016/images/fip_overlapzoom.jpg "FIP Index in ArcGIS Pro zoom")

---
## Next Steps?
  - Allow users to download the georeferenced images
    - ...but there are copyright issues
  - Tackle another year or another geographic area
  - Create KML (Google Earth)

---
## Questions

Rebecca Bartlett - GIS and Digital Resources Librarian

Joel Rivard - Cartographic Specialist

[gis@carleton.ca](@gis@carleton.ca) / [@GIS_Carleton](https://twitter.com/GIS_Carleton)
