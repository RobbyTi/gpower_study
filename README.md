This repository contains the code, data, and other materials related to the manuscript "An evaluation of reproducibility and errors in statistical power calculations performed using GPower". The purpose of this study was to assess the reproducibility and quality of sample size calculations in published articles and conducted using the GPower software.

# This repository contains 5 folders:

## /code
This folder contains:
- analysis.Rmd : This script intakes main_raw.csv, cleans the data, outputs main_clean.csv, performs all analyses, and outputs all tables and numbers used in the manuscript results section.
- analysis.pdf : This is the output of analysis.Rmd. The tables have been copied from this document and pasted into the manuscript.

## /data
This folder contains: 
- data_dictionary.csv : Explains how to find the information regarding what each variable represents.
- main_raw.csv : The raw data for the main analysis (for all tables)
- main_clean.csv : The clean data for the main analysis. This dataset is output after the code cleans the main_raw.csv file
- anova_raw.csv : The extra data we collected to raise the sample size of the anova analysis (for Table 5 only) 
- /reproductions : This folder contains screenshots of all the power calculation we reproduced. They are saved with the PubMed Central ID as the filename, and can be matched to the associataed paper through that ID.

## /environment
This folder contains
- Dockerfile : This file outlines the environment necessary to execute the analysis.Rmd file

## /materials
This folder contains:
- /protocol : This folder contains: Our preregistered protocol, the code and output we used for this protocol, and the PMCIDs of the articles we sampled
- codingForm_main.pdf : This is a PDF version of the coding form we used on each article.
- codingForm_anova.pdf : This is a shortened version of the coding form that we used only to increase our sample size for the ANOVA analysis.

## /results
- This folder contains all tables from the manuscript in .csv files.

# How to run the analysis code
- The analysis code was written in RMarkdown. The dependencies necessary to run the code are provided in the Dockerfile. The easiest way to re-run the code is by clicking "Reproducible Run" in this manuscript's reproducible container on Code Ocean (https://doi.org/10.24433/CO.4349082.v1). Alternatively, R can be downloaded from www.r-project.org/
