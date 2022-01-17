## EDS232_iNat_species_distribution
Species Distribution Modeling

## Environmental Data Science 232 Machine Learning Lab 01 assignment

### Overview

This machine learning analysis was completed as an assignment for my Master’s program course, Environmental Data Science 232: Machine Learning. It was assigned by our professor, Dr. Ben Best, as an introduction to machine learning by predicting presence of a chosen species from observations and environmental data found on the site [iNaturalist](https://www.inaturalist.org/). It follows guidance found at [Species distribution modeling | R Spatial ](https://rspatial.org/raster/sdm/).

My chosen species is coyote brush (*Baccharis pilularis*). **Baccharis pilularis** is native to the west coast of the United States (Oregon, California, and Baja California, Mexico). It is a shurb in the Asteraceae (Sunflower) family with oblanceolate to obovate toothed leaves, panicle-like inflorescence with staminate flowers that when mature mimic snow, and generally sticky (*not a pun*).

### Learning Objectives {-}

- Explore
  - Fetch species observations from the Global Biodiversity Information Facility (GBIF.org) using an R package that wraps a function around their API.
  - Fetch environmental data for defining environmental relationship in the species distribution model (SDM).
  - Generate pseudo-absences, or background, points with which to differentiate from the species presence points in the SDM.
  - Extract underlying environmental data from points.
  - Plot term plots of each environmental predictor with the species response.
  
### Packages

dismo
dplyr
DT
ggplot2
here
htmltools
leaflet
mapview
purrr
raster
readr
rgbif
rgdal
- rJava
- sdmpredictors
- sf
- spocc
- tidyr
  
