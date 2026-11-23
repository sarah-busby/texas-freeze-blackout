# Visualizing Houston, Texas blackouts after the 2021 extreme winter storms

This repository contains materials for the fourth assignment for [EDS 223 - Geospatial Analysis & Remote Sensing](https://eds-223-geospatial.github.io/). Full instructions for this assignment can be found on [the course website](https://eds-223-geospatial.github.io/assignments/HW4.html). Per instructions, this repo visualizes Houston homes impacted by power outages after the 2021 severe winter storms. Blackout areas are determined by changes in night time radiance from VIIRS data colleced by NASA's Level-1 and Atmospheric Archive & Distribution System Distributed Active Archive Center (LAADS DAAC)[https://www.earthdata.nasa.gov/data/catalog/laads-vnp46a1-2#toc-description]. Houston roads and buildings data were collected from [OpenStreetMap](https://planet.openstreetmap.org/) and retrieved via [Geofabrik's download site](https://download.geofabrik.de/).

## Repository Structure

```         
texas-freeze-blackout
│   README.md
│   houston-blackout-analysis.qmd               # Analysis quarto doc
│   houston-blackout-analysis.pdf               # Rendered pdf analysis
│
└───.gitignore
     └───data
         └───gis_osm_buildings_a_free_1.gpkg    # Shapefiles for Houston buildings
         └───gis_osm_roads_free_1.gpkg          # Shapefiles for Houston roads
         └───VNP46A1                            # Contains satellite data
             └───VIIRS data files
```

## Data access

The processed data used for analysis can be accessed from Google Drive as a zip file [here](https://drive.google.com/file/d/1bTk62xwOzBqWmmT791SbYbHxnCdjmBtw/view).

## Visualization and Analysis

Script for visualization and analysis for the project can be found in `houston-blackout-analysis.qmd` and rendered as `houston-blackout-analysis.pdf`.

## References

NASA VIIRS Land Science Investigator-Led Processing System. (2024). VIIRS/NPP Daily Gridded Day Night Band 500 m Linear Lat Lon Grid Night \[Data set\]. NASA Level 1 and Atmosphere Archive and Distribution System Distributed Active Archive Center. https://doi.org/10.5067/VIIRS/VNP46A1.002.

OpenStreetMap contributors. (2026). OpenStreetMap data extract for \[Houston\] \[Data set\]. OpenStreetMap Foundation (OSMF). Retrieved from https://download.geofabrik.de/.