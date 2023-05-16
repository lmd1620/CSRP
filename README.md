May 2023 Update: the official paper is to be published online!  If you find the source code useful in your research work, please cite: M. Liu, Y. Zhao and X. Xie “Continuity-skill-restricted scheduling and routing problem: Formulation, optimization and implications” IISE Transactions (2023). 

# CSRP
Continuity-skill-restricted Scheduling and Routing Problem: Formulation, Optimization and Implications

The main repository contains code and make files to computationally minimize the costs of a caregiver routing problem with time windows. 

## Overview
We investigate a deterministic continuity-skill-restricted scheduling and routing problem (CSRP) and its stochastic variant (SCSRP) to address attended home healthcare (AHH) problem, which is a variant of classical vehicle routing problem with time windows (VRPTW). We propose a branch-price-and-cut (BPC) algorithm to solve the CSRP and a discrete-approximation-method adaption for the SCSRP.

## Input
The data used in this study is publicly available at the following website* https://doi.org/10.5281/zenodo.7928388

## Content
* cplex - solve the compact formulation with the CPLEX
  * global_variables.cpp
  * global_functions.cpp
  * cplexptree.cpp 
* CSRP_out_of_performance - includes supporting BPC code for solving the CSRP 
  * global_variables.cpp
  * global_functions.cpp
  * heuristic.cpp - includes supporting code for warm-up heuristic algorithm
  * bp_form.cpp - includes supporting code for branch-and-bound algorithm
  * labelcor.cpp - includes supporting code for label-setting algorithm to solve the pricing problem
  * tabu.cpp - includes supporting code for heuristic pricing algorithm 
  * main.cpp 
* SCSRP_out_of_performance - includes supporting BPC code for solving the SCSRP 
  * global_variables.cpp
  * global_functions.cpp
  * heuristic.cpp - includes supporting code for warm-up heuristic algorithm
  * bp_form.cpp - includes supporting code for branch-and-bound algorithm
  * labelcor.cpp - includes supporting code for label-setting algorithm to solve the pricing problem
  * tabu.cpp - includes supporting code for heuristic pricing algorithm 
  * main.cpp 

## Requirements
A CPLEX solver is necessary for solving the LP and MIP models. 

## Contributors
Mingda Liu, Tsinghua University, ydtmingda16@163.com

Yanlu Zhao, Durham University, yanlu.zhao@durham.ac.uk

Xiaolei Xie, Tsinghua Univeristy, xxie@tsinghua.edu.cn
