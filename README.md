# ENVS-193DS_spring-2025_final
Repository for final assignment for ENV S193DS at UCSB.


# ENVS 193DS Final

Kai Suzuki
06-10-2025

## General information

The data set *SST_update2023.csv* is from Li Kui (2024) sourced from the Santa Barbara Coastal LTER's Data Catalog. [Link to Data](https://portal.edirepository.org/nis/mapbrowse?packageid=knb-lter-sbc.161.3).

The data set *occdist.csv* is from Stojanovic, Dejan et al. (2021) sourced from Dryad. [Link to Data](https://datadryad.org/dataset/doi:10.5061/dryad.83bk3j9sb)

The associated referenced paper is from Stojanovic, D., Owens, G., Young, C.M., Alves, F., and Heinsohn, R. 2021. Do nest boxes breed the target species or its competitors? A case study of a critically endangered bird. Restoration Ecology. [10.1111/rec.13319](https://doi.org/10.1111/rec.13319)

This repository is for the final in Spring 2025 for ENV S193DS, taught by An Bui at the University of California, Santa Barbara. The directions followed can be found [here](https://spring-2025.envs-193ds.com/assignments/final)

### Packages

```
library(tidyverse) # general data tasks
library(here) # managing files
library(janitor) # for data cleaning
library(DHARMa) # for checking model diagnostics
library(MuMIn) # for running AIC models
library(gt) # for table construction
library(xfun) # for troubleshooting
library(ggeffects) # making predictions
sst <- read_csv("../data/SST_update2023.csv") # reading data for problem 2
nest_boxes <- read_csv("../data/occdist.csv") # reading in data from article for problem 3
```

## Data and file information

File structure:

```
.
├── ENVS-193DS_spring-2025_final.Rproj
├── README.md
├── code                                     # code folder
│   ├── answers.qmd                          # qmd file for code and text
│   └── answers.html                         # rendered output from .qmd
├── data                                     # data folder
│   ├── occdist.csv                          # data for problem 2
│   └── SST_update2023.csv                   # data for problem 3
└── images
    ├── sketchHW3.jpg                        # image of sketch
    └── draftHW3.jpg                         # image of draft
```

All code is in the `code` folder. The code analyzes data and creates data visualizations and data tables.

## Rendered output

The rendered output can be found [here](https://kai-s-suzuki.github.io/ENVS-193DS_homework-03/code/homework.html)  