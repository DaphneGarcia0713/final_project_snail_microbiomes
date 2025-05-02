### README for final_project_snail_microbiomes/code ###

This directory contains two R files:

1. colors.R
2. functions.R

## colors.R
This file contains color palates for the temperature, sex, and temperature-sex experimental groups in this study, as well as phylum taxonomy. These color palates are used for plots in `analysis/06_Ordination.Rmd` and `analysis/07_Composition.Rmd`

## functions.R
This file contains a function `scale_reads` used in `analysis/06_Ordination.Rmd`. This function scales the sequencing reads at the minimum sample size in the study for beta-diversity analysis.