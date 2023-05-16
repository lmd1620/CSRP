May 2023 Update: the official paper is to be published online!  If you find the source code useful in your research work, please cite: M. Liu, Y. Zhao and X. Xie “Continuity-skill-restricted scheduling and routing problem: Formulation, optimization and implications” IISE Transactions (2023). 

# CSRP
Continuity-skill-restricted Scheduling and Routing Problem: Formulation, Optimization and Implications

The main repository contains code and make files to computationally minimize the costs of a caregiver routing problem with time windows. 

## Overview
We investigate a deterministic continuity-skill-restricted scheduling and routing problem (CSRP) and its stochastic variant (SCSRP) to address attended home healthcare (AHH) problem, which is a variant of classical vehicle routing problem with time windows (VRPTW). We propose a branch-price-and-cut (BPC) algorithm to solve the CSRP and a discrete-approximation-method adaption for the SCSRP.

## Input
The data used in this study is publicly available at the following website* https://doi.org/10.5281/zenodo.7928388

## Content
* simulate.py - defines new scenarios, runs the simulation, and saves the simulation's output as a single .xlsx file in the output/ subfolder
supporting.py - includes supporting code such as functions to execute routing algorithms and calculate transportation costs
combine_outputs.py - combines simulation output files from the /output subfolder into a single summary .xlsx sheet
create_figures.R - reads in all files in the output/ subfolder and generates summary graphs
Also, the Jupyter notebook routing_examples.ipynb is a supplemental file that allows users to generate a random customer and demand instance and see the resulting routes and costs under the different routing strategies.
