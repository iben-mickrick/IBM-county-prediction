# Predicting Resource Intensive Healthcare (RIHC)

This objective of this study was to develop models predicting 3-outcome metrics of RIHC among U.S. counties using routinely collected governmental data. The 3-outcome metrics of RIHC included: (1) emergency room visits, (2) inpatient days, and (3) hospital expenditures. Data on the outcome metrics was obtained from the American Hospital Association Survey, available from the Health Resources Services Administration. Candidate features came from four broad groups, including: (1) demographics from the U.S. Census Bureau, (2) adult and child health characteristics from the Centers for Disease Control and Prevention, (3) community characteristics from the American Community Survey, and (4) consumer expenditures from the Bureau of Labor Statistics. 

Feature selection methods were undertaken to select the most important features for each of the 3-outcome metrics. A machine learning pipeline was developed where 4 distinct algorithms were applied to unique combinations of selected features. Mean squared error (MSE), calculated using cross-validation on the test-set was the metric used to identify the best performing model. This process was repeated separately for each of the 3-outcome metrics. SHAP value analysis was conducted on the best-performing model for each outcome-metric. 

The code included herein includes the machine learning model development and post-model evaluation. The code is broken into several pieces for organizational ease. The pieces include:<br/>

(1) Model preparation --this covers second order term identification, and feature selection <br/>
(2) Modelling part 1 -- this covers the iterative and systematic machine learning pipeline for iterations 1a, 1b, 1c, 1d, 2a, 2b, 2c, and 2d <br/>
(3) Modelling part 2 -- this covers the iterative and systematic machine learning pipeline for iterations 3a, 3b, 3c, 3d, 3e, and 3f <br/>
(4) Modelling part 3 -- this covers the iterative and systematic machine learning pipeline for iterations 4a, 4b, 4c, and 4d <br/>
(5) Post model evaluation -- this covers post model evaluation, including calibration assessement and SHAP value analysis <br/>
