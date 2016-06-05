<div align="Center">
## Making LAC fire insurance plans (FIP) more easily accessible
<br>
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/cover.jpg "Cover")
by Rebecca Bartlett & Joel Rivard

Rebecca.bartlett@carleton.ca

joel.rivard@carleton.ca

---
##Outline

 - Introduction to the problem
 - Our amazing (yet, time-consuming) solution!!!
 - Moving forward and discussion

---

#Have you ever tried finding and/or using FIP from LAC?

---
![Frustrated](http://cu-library.github.io/carto-2016/images/frustrated.jpg "Frustrated")

## searching

![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_searchresults.jpg "Searching")

---

![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/lac_search.jpg "Search")

---
## Introduction to the problem
Finding FIP's through LAC's website is:
- slow
- Incorrect
- time-consuming
---

## solution

Create a better index for the FIP collection

---

## collection

We choose the **Insurance plan of the city of Ottawa, Canada, and adjoining suburbs and lumber districts, January 1888, revised January 1901**
It included 114 sheets on LAC's website

---
## Methodology

- Georeference the FIP plans (keymap not accurate)
- This will give us our index + the georeferenced plans

Win Win Situation!! (**image**)

---
## Methodology

- In ArcMAp 10.3, used the georefencing toolbar to add roughly 8-12 ground control points.
- Used multiple referencing layers:
  - 1928 air photos from the city of ottawa
  - Current Ottawa-Gatineau open data streetfile (downloaded from city of Ottawa and ville de Gatineau)
- Georeferenced the FIP to MTM zone 9.
---

## Methodology

80 map sheets had fire insurance plans of specific geographic areas
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/regular_sheet.jpg "FIP Regular Sheet")
---
## Methodology

22 map sheets showed multiple fire insurance plans of different areas
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/split_sheet.jpg "FIP Split-up")

We needed to split these up.
---
## Methodology

12 sheets that weren't maps (keymaps or street index)
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/split_keymap.jpg "FIP Split-up")
![Fire Insurance Plans](http://cu-library.github.io/carto-2016/images/split_index.jpg "FIP Split-up")

---
## Potential Issues

- Source data used is at least 30 years more up-to-date than year of FIP
- No data-frame or coordinate system used in FIP

---

## Methodology
- Once the fire insurance plans were georeferenced, we created the index (**mention the tool**)
- For each area, added a link to that particular sheet on LAC's website
-Used ArcGIS Online for the index
