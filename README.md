# longitudinal-count-model-selection-tmb
The zip file contains code for Longitudinal Count Data analysis, with or without missing data. 
It includes two main folders, Simulations and Real Data Analysis, along with the required R scripts and TMB files.

## 1. Simulations
--------------

The Simulations folder includes the TMB (Template Model Builder) codes and data used 
for the simulation studies presented in the paper:

Improving Inference for Longitudinal Count Data with or without Missing Data 
through Model Selection by Ayesha Madhushani Rathnayake, Candemir Cigsar, and Nan Zheng.

It contains two subfolders for different types of simulation studies: Complete Data 
and Missing Data. Each subfolder includes R scripts and TMB files implementing 
the corresponding models.

1.1 Complete Data Simulations

R scripts:
- Simulation_Poisson_AR1_Mixed_Effect_Complete.R
- Simulation_Poisson_MA1_Mixed_Effect_Complete.R
- Simulation_Poisson_EQC_Mixed_Effect_Complete.R

TMB files:
- AR1_Complete.cpp
- MA1_Complete.cpp
- EQC_Complete.cpp

1.2 Missing Data Simulations

R scripts:
- Simulation_Poisson_AR1_Mixed_Effect_Missing.R
- Simulation_Poisson_MA1_Mixed_Effect_Missing.R
- Simulation_Poisson_EQC_Mixed_Effect_Missing.R

TMB files:
- AR1_Missing.cpp
- MA1_Missing.cpp
- EQC_Missing.cpp


Each subfolder contains scripts that:
- Generate simulated data
- Compile the TMB model
- Run parameter estimation
- Save outputs for performance evaluation


## 2. Real Data Analysis
--------------
R scripts: 
- AIDS_Real_Data 


TMB files:
- AR1_real_data.cpp
- MA1_real_data.cpp
- EQC_real_data.cpp

Required Packages
-----------------
R packages: TMB, MASS, JM
System requirements: Ensure that R is installed, then install Rtools (for Windows) 
or the appropriate compiler for your OS, and finally install the required packages.

How to Run the Code
-------------------
For Simulations:
1. Navigate to the desired subfolder under Simulations/Complete Data Simulations 
   or Simulations/Missing Data Simulations.
2. Compile the corresponding C++ file using TMB::compile() in R.
3. Run the simulation script (e.g., Simulation_Poisson_AR1_Mixed_Effect_Complete.R), which will:
   - Generate the simulated data
   - Fit the model
   - Save the results

For Real Data Analysis:
1. Load the AIDS dataset from the JM R package.
2. Compile the corresponding TMB model file as instructed in the R script (e.g., AR1_real_data.cpp).
3. Run the main R script AIDS_Real_Data.R to fit the model to the real-world data.

