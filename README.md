# Analysis of band iridescence in *Syngnathus scovelli*

This repository documents the analysis of iridescence bands located primarily on female Gulf pipefish, *Syngnathus scovelli*. Iridescence was measured using the Iridescence Detection and Isolation Algorithm (IDIA) and the goals of this study are to:

1. Test the reliability and repeatability of iridescence measurements from the IDIA
2. Determine wether the IDIA could be used to detect geographic variaiton in the iridescent signal on females
3. Investigae the use of the IDIA to measure the development of iridescence on males as a response to exposure to synthetic estrogen

## Data
The code refers to data that is found in the processed_data/ directory at the top of the repo. The datasheets in this directory were made from the orignal raw data (see Data Availability for how to access raw data) with things like Mean Band Iridescence per pipefish included rather than the measurements for each individual band on every pipefish. 

### Data Availability
The raw data files containing the iridescence measurements for each individual band on the pipefish are archived for review purposes on ...

## Navigating this repository
The analysis is documented in a series of Rmarkdown documents.

### Rmarkdown documents
All Rmarkdown documents are located in the folder called docs/. They do the following things:

- `Lighting_condition.Rmd`: Read in the corresponding datasheet, perform some exploratory analysis (including a two-way ANOVA), and performs the two one-way ANOVAs reported in the study along with all proper assumption testing. It also includes the code to create Supplemental Fig. 1 in the manuscript.

- `geo_variation.Rmd`: Read in the datasets and subset for equal sample size, run a series of models looking at variation of traits across location, and performs the correlation testing between band area and band iridescence. This file also includes the code to create Fig. 4, Fig. 5, and Supplemental Fig. 2 in the manuscript.

-`estrogen.Rmd`: Read in the datasets, perform some exploratory analysis and run tests surrouding the development of iridescence on males exposed to estrogen compared to both control males and females. It also includes the code to create Fig. 6 in the manuscript.

## Author Information
All of this code was written by Coley Tosto as a part of her undergraduate work at the University of Tampa
