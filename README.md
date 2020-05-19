# Microbiome Temporal Analysis - Impact of the gut microbiota on peripheral immune cells dynamics

## Overview

This project is an enhancement attempt of an existing article, whose aim is to quantify the impact of the gut microbiota on the change rate of three types of white blood cells : neutrophils, lymphocytes and monocytes.

The original article can be found at https://www.biorxiv.org/content/10.1101/618256v2.

Our idea was to refine the linear regression the authors perform by a more complex one, namely a Neural Network regression. To build our model, we used [Keras](https://keras.io).

## Data description

The original data tables are located in the "Supplementary Material" section of the article (see the link above). 
We also saved the data we used for the training of our NNs, after a heavy selection on the original data. These tables can be found in `training_data`, separated according to each stage of the analysis.

## Setup

This project was made on Google Colab, to speed up the training of our NNs, but can be run without it. In that case, please ignore the first section of the notebook.

## Running the notebook

The notebook to be run is ```MTA.ipynb```. You can simply run it cell by cell, from the start to the end. However, the data selection phases can be pretty long to run, so we included an option to directly import the data from the ```training_data``` folder.
The only thing that needs to be changed is the paths used when importing/exporting data.

## Results

The results for the neutrophils change rate can be found in the ```Figs/results``` folder, separated by graft type (PBSC, TCD, BM and cord). 
