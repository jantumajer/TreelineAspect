# Data and scripts associated with the manuscript “Radial growth of Picea abies is controlled by joint effects of temperature and nutrient availability at the lower part of treeline ecotone”
By Hana Kuželová, Tomáš Chuman, Jelena Lange, Jan Tumajer, Václav Treml

## Inputs
Input data involve (i) `south-north-clim.xlsx` - site microclimatic data and soil data characteristics of sites used to draw figures 1,2, 3 and Supplementary figure 1. (ii) `blabxylf2.csv` – raw wood phenology data. (iii) `bsf.rwl`, `blj.rwl` tree-ring width measurements used for derivation of tree-ring with chronologies. (iv) `tempbl.csv`, `precbl.csv` files containing station climatic data used for climate-growth analysis.
## R scripts
#### Wood formation
This script was used to fit the Gompertz curves and derive critical dates of wood formation. As input the `blabxylf2.csv` file is used.
#### Climate-growth response
Script builds tree-ring chronologies and calculates growth-climate correlations at daily level. As inputs the rwl files (`bsf.rwl`, `blj.rwl`) and station climatic data are used.

