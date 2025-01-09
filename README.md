# Data and scripts associated with the manuscript “Radial growth of Picea abies is controlled by joint effects of temperature and nutrient availability at the lower part of treeline ecotone”

## Inputs
Input data involve (i) `south-north-clim.xlsx` - site microclimatic data and soil data characteristics of sites from the [TreeDataClim database](www.treedataclim.cz/en). This file is also used to match sites with rwl files. Several rwl files are attached for testing. The remaining rwl files are available upon request through the TreeDataClim website. (ii) Input data also includes climatic surfaces used for extraction of climatic data for each site (precipitation – `sra_wgs_month.nc` , temperature – `t_wgs_month.nc`). For a detailed description see [Mašek et al. 2024](https://linkinghub.elsevier.com/retrieve/pii/S0048969723069024) in Science of the Total Environment.
## R scripts
### Age structure adjustment
This script was used to adjust the age structures of samples to create datasets 1990 and 2015. As inputs, the `treedataclim.csv` and rwl files are used.
### Climatic response calculation
The script reads data from climatic surfaces (`t_wgs_month.nc`, `sra_wgs_month.nc`) for each site, builds tree-ring chronology, detrend SPEI time-series and calculates correlations between tree-ring chronology and SPEI for two periods before and after 1990. As inputs the treedataclim.csv, rwl files and climatic surfaces are used.
### Fitting structural equations models
Script fits first linear models, tests for their autocorrelation and then fits structural equations models either using linear models (autocorrelation insignificant) or spatial lag, spatial error models (autocorrelation significant). The input data are in table `seminput.csv`. 
## Table outputs used for fitting models and plotting figures
File `seminput.csv` was derived as the output of the Age structure adjustment script (stem diameters, stem diameter change, mean site basal area increments, mean site age, number of trees) connected with site environmental data (climatic water balance, topography wetness index, soil chemistry variables and their principal components).

File `coreltable.csv` represents an output from the Climatic response calculation script. This file was used as a source of correlation coefficients between growth and SPEI.
