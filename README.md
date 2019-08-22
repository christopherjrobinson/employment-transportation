# This repository contains the replication materials for the project Public Transit and Private Car Ownership: How to Best Help Low-Income, Urban Workers by CJ Robinson

## Setup and Benchmarks

Original code run on MAC OSX 10.14.4, 8gb RAM, 1.8 GHz Intel Core i5. R version 1.1.456 

Required packages:
* tidyverse
* ggplot2
* stargazer

Benchmarks: Code takes few seconds to run

## Instructions in Brief

1. Run data.processing.RData to produce the clean master data
frame for the analysis.
2. Run main.analysis.RData to produce the regression models.
3. Run tables.RData to produce the LATEX code for Tables.
4. Run figures.RData to produce figures.


## Data

The ./data/ directory
contains the necessary data to replicate the analysis and analytical
figures and tables in the paper. Below, I describe each of the
datasets in this directory.

bivar_model_car1.RData: Bivariate model of effect of car ownership in dataset 1

bivar_model_car2.RData: Bivariate model of effect of car ownership in dataset 2

bivar_model_pt1.RData: Bivariate model of effect of public transit in dataset 1

bivar_model_pt2.RData: Bivariate model of effect of public transit in dataset 2

gss1.csv: first dataset of respondents that are both employed and unemployed measuring employment status

gss2.csv: second dataset of respondents that are employed measuring perceived mobility

multivar_model_car1.RData: Multivariate model of effect of car ownership in dataset 1

multivar_model_car2.RData: Multivariate model of effect of car ownership in dataset 2

multivar_model_pt1.RData: Multivariate model of effect of public transit in dataset 1

multivar_model_pt2.RData: Multivariate model of effect of public transit in dataset 2

survey_master.csv: original dataset pulled from GSS Data Explorer

## Code

The ./code/ directory
contains the code to replicate the analysis and analytical figures
and tables in the paper. Below, I describe each code script in this
directory. The ./figures/ directory contains a copy of each of
the figures generated by these scripts; the ./tables/ directory
contains a copy of the LATEX table code generated by these
scripts.

* data.processing.RData: Code to produce the clean datasets
used to fit the regression models; generates and outputs the
data file for the analysis, figures, and tables in the paper.
* main.analysis.RData: Code that factors several variables in each dataset and runs several bivariate and multivariate regressions.
* tables.RData: Code to write LaTeX code using the package "stargazer" to describe regressions and correlations.
* figures.RData: Code to generate several figures to help interpret data and regressions including bar graphs and predict plots.
