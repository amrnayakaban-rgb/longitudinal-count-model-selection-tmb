
This ZIP file contains the code for longitudinal count data analysis using Poisson and negative binomial mixed-effects models under complete data and missing data settings. It includes two main folders, Simulations and Real Data Analysis, along with the required R scripts and Template Model Builder (TMB) C++ files.


1. Simulations
--------------

The Simulations folder contains the R scripts and TMB C++ files used for the simulation studies presented in the paper:

Improving Inference for Longitudinal Count Data through Model Selection by Ayesha Madhushani Rathnayake, Candemir Cigsar, and Nan Zheng.

It contains three subfolders:

- Complete Data Setting: Simulation studies using fully observed longitudinal count data.
- MCAR Data Setting: Simulation studies under the missing completely at random (MCAR) mechanism.
- Ignorable MAR Data Setting: Simulation studies under the ignorable missing at random (MAR) mechanism.

Each subfolder contains R scripts and TMB C++ files implementing five mixed-effects models:

- Poisson with equicorrelation (EQC).
- Poisson with first-order autoregressive (AR(1)) correlation.
- Poisson with first-order moving-average (MA(1)) correlation.
- Negative binomial with equicorrelation (EQC).
- Negative binomial with first-order moving-average (MA(1)) correlation.


1.1 Complete Data Simulations
-----------------------------

R scripts:
- Simulation_Poisson_EQC_Mixed_Effect_Complete_Data.R
- Simulation_Poisson_AR1_Mixed_Effect_Complete_Data.R
- Simulation_Poisson_MA1_Mixed_Effect_Complete_Data.R
- Simulation_NB_EQC_Mixed_Effect_Complete_Data.R
- Simulation_NB_MA1_Mixed_Effect_Complete_Data.R


TMB files:
- Poisson_EQC_Complete_Data.cpp
- Poisson_AR1_Complete_Data.cpp
- Poisson_MA1_Complete_Data.cpp
- NB_EQC_Complete_Data.cpp
- NB_MA1_Complete_Data.cpp



1.2 MCAR Simulations
--------------------

R scripts:
- Simulation_Poisson_EQC_Mixed_Effect_MCAR_Data.R
- Simulation_Poisson_AR1_Mixed_Effect_MCAR_Data.R
- Simulation_Poisson_MA1_Mixed_Effect_MCAR_Data.R
- Simulation_NB_EQC_Mixed_Effect_MCAR_Data.R
- Simulation_NB_MA1_Mixed_Effect_MCAR_Data.R


TMB files:
- Poisson_EQC_Missing_Data.cpp
- Poisson_AR1_Missing_Data.cpp
- Poisson_MA1_Missing_Data.cpp
- NB_EQC_Missing_Data.cpp
- NB_MA1_Missing_Data.cpp


1.3 Ignorable MAR Simulations
-----------------------------

R scripts:
- Simulation_Poisson_EQC_Mixed_Effect_MAR_Data.R
- Simulation_Poisson_AR1_Mixed_Effect_MAR_Data.R
- Simulation_Poisson_MA1_Mixed_Effect_MAR_Data.R
- Simulation_NB_EQC_Mixed_Effect_MAR_Data.R
- Simulation_NB_MA1_Mixed_Effect_MAR_Data.R


TMB files:
- Poisson_EQC_Missing_Data.cpp
- Poisson_AR1_Missing_Data.cpp
- Poisson_MA1_Missing_Data.cpp
- NB_EQC_Missing_Data.cpp
- NB_MA1_Missing_Data.cpp



Each subfolder contains scripts that:
- Generate simulated longitudinal count data.
- Compile the corresponding TMB model.
- Perform parameter estimation.
- Save the results for performance evaluation.


2. Real Data Analysis
---------------------

This folder contains the R scripts and TMB C++ files used for the analysis of the epileptic seizure count dataset presented in the paper.

R scripts:
- Epil_Real_Data_Model_Selection.R
- Poisson_EQC_Epil_Dataset.R
- Poisson_AR1_Epil_Dataset.R
- Poisson_MA1_Epil_Dataset.R
- NB_EQC_Epil_Dataset.R
- NB_MA1_Epil_Dataset.R


TMB files:
- Poisson_EQC_Epil_Dataset.cpp
- Poisson_AR1_Epil_Dataset.cpp
- Poisson_MA1_Epil_Dataset.cpp
- NB_EQC_Epil_Dataset.cpp
- NB_MA1_Epil_Dataset.cpp


Required Packages
-----------------

R packages: TMB, MASS.

System requirements: Ensure that R is installed, then install Rtools (for Windows) or an appropriate C++ compiler for your operating system, and finally install the required R packages.


How to Run the Code
-------------------

For Simulations:

1. Navigate to the desired subfolder under Simulations/Complete Data Setting, Simulations/MCAR Data Setting, or Simulations/Ignorable MAR Data Setting.

2. Compile the corresponding C++ file using TMB::compile() in R.

3. Run the appropriate simulation script (e.g., Simulation_Poisson_EQC_Mixed_Effect_Complete_Data.R), which will:
   - Generate the simulated data.
   - Fit the model.
   - Save the results.


For Real Data Analysis:

1. Load the epileptic seizure dataset (epil) from the MASS R package.

2. Compile the corresponding TMB C++ files using TMB::compile() in R.

3. Run Epil_Real_Data_Model_Selection.R to perform model selection among the five competing mixed-effects models using information criteria.

4. Run the individual model-specific R scripts (Poisson_EQC_Epil_Dataset.R, Poisson_AR1_Epil_Dataset.R, Poisson_MA1_Epil_Dataset.R, NB_EQC_Epil_Dataset.R, and NB_MA1_Epil_Dataset.R) to obtain parameter estimates for each model and perform residual analysis.



