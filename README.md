# CIBMTR---Equity-in-post-HCT-Survival-Predictions

This project focuses on developing models to improve the prediction of transplant survival rates for patients undergoing allogeneic Hematopoietic Cell Transplantation (HCT), with an emphasis on ensuring equitable healthcare outcomes across diverse populations. Stratified Concordance Index (C-index) used as evaluation metric.

My final solution ranked in the top **%24 (779/3325)** with the **private score of 0.692** 

# Tech Stack

 - numpy
 - pandas
 - seaborn
 - matplotlib
 - plotly
 - scikit-learn
 - xgboost
 - lightgbm
 - catboost
 - lifelines
 - scipy
 - pytorch

## Solution Approach

 - Event-Masked Pairwise Ranking Network
 - [Yunbase](https://www.kaggle.com/code/yunsuxiaozi/cibmtr-yunbase)
 - XGBoost+LightGBM with Transformed Targets (Cox, Kaplan-Meier, Nelson-Aalen, separating events, log, quantile)

>Ensembled the top ranking models

## Key Findings

 - NN model boosted the final performance
 - Target tranformations -especially Kaplan-Meier, Nelson-Aalen and log- enhanced predictive performance of XGBoost and LightGBM
 - Ensembling ensured better robustness and reduced the risk of overfitting in private data 