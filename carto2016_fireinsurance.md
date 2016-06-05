<div align="Center">
## Making LAC fire insurance plans more easily accessible
<br>
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
![Frustrated](http://cu-library.github.io/carto-2016/images/frustrated.jpg "Frustrated")

--
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_searchresults.jpg "Searching")

--

![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_search.jpg "Search")

---
## Introduction to the problem
Finding FIP's through LAC's website is:
  - slow
  - Incorrect
  - time-consuming
---

## Solution

Create a better index for the FIP collection

---

## Collection

We choose the<br<br> **Insurance plan of the city of Ottawa, Canada, and adjoining suburbs and lumber districts, January 1888, revised January 1901**
<br><br>
It included 114 sheets on LAC's website

---
## Methodology

- Georeference the FIP plans (keymap not accurate)
- This will give us our index + the georeferenced plans
<br><br>
Win Win Situation!! (**image**)

---
## Methodology

- In ArcMAp 10.3, used the georefencing toolbar to add roughly 8-12 ground control points.
- Used multiple referencing layers:
  - 1928 air photos from the city of ottawa
  - Current Ottawa-Gatineau open data streetfile (downloaded from city of Ottawa and ville de Gatineau)
- Georeferenced the FIP to MTM zone 9
---

## Methodology

80 map sheets had fire insurance plans of specific geographic areas
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/regular_sheet.jpg "FIP Regular Sheet")
---
## Methodology

22 map sheets showed multiple fire insurance plans of different areas
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/split_sheet.jpg "FIP Split-up")

We needed to split these up
---
## Methodology

12 sheets that weren't maps (keymaps or street index)
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/keymap_sheet.jpg "FIP keymap")
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/index_sheet.jpg "FIP Index")

---
## Potential Issues

- Source data used is at least 30 years more up-to-date than year of FIP
- No data-frame or coordinate system used in FIP

---

## Methodology
- Once the fire insurance plans were georeferenced, we created the index (**mention the tool**)
- For each area, added a link to that particular sheet on LAC's website
- Used ArcGIS Online for the index