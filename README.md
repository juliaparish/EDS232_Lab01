# Environmental Data Science 232 Machine Learning Lab 01 Assignment

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
  - Pairs plot to show correlation between variables and avoid **multicollinearity** (see [8.2 Many predictors in a model](https://openintro-ims.netlify.app/model-mlr.html#many-predictors-in-a-model))
- **Logistic Regression** seen as an evolution of techniques
  - **Linear Model** to show simplest multivariate regression, but predictions can be outside the binary values.
  - **Generalized Linear Model** uses a logit transformation to constrain the outputs to being within two values.
  - **Generalized Additive Model** allows for "wiggle" in predictor terms.
  - **Maxent** (Maximum Entropy) is a presence-only modeling technique that allows for a more complex set of shapes between predictor and response.
  
- Decision Trees
Use **Decision Trees** as a **Classification** technique to the data with the response being categorical (`factor(present)`).
- **Recursive Partitioning** (`rpart()`)\
    Originally called classification & regression trees (CART), but that's copyrighted (Breiman, 1984).
-   **Random Forest** (`RandomForest()`)\
    Actually an ensemble model, ie trees of trees.
- Complete the modeling workflow with the steps to **evaluate** model performance and **calibrate** model parameters.

### Packages

- dismo
- dplyr
- DT
- ggplot2
- here
- htmltools
- leaflet
- mapview
- purrr
- raster
- readr
- rgbif
- rgdal
- rJava
- sdmpredictors
- sf
- spocc
- tidyr

caret,       # m: modeling framework
  dplyr, ggplot2 ,here, readr, 
  pdp,         # X: partial dependence plots
  ranger,      # m: random forest modeling
  rpart,       # m: recursive partition modeling
  rpart.plot,  # m: recursive partition plotting
  rsample,     # d: split train/test data
  skimr,       # d: skim summarize data table
  vip)         # X: varia
  dismo, # species distribution modeling: maxent(), predict(), evaluate(), 
  dplyr, ggplot2, GGally, here, maptools, readr, 
  raster, readr, rsample, sf,
  usdm
  
