Startup Destiny Predictor: Predicting Acquired vs. Closed Status

Project Summary

This capstone project focuses on solving a fundamental challenge in Venture Capital (VC) and financial analysis: accurately forecasting the final outcome of a startup (its "destiny"). Using a comprehensive dataset of over 48,000 global startup funding histories, we developed and benchmarked several classical machine learning models to build a high-precision classification system.

The core difficulty addressed is extreme class imbalance, as the 'Acquired' and 'Closed' statuses represent rare events compared to the majority 'Operating' status.

 Key Objective
 
 To identify the most robust and predictive classical model that maximizes the F1-Score for the minority classes, 
 thereby providing a reliable early-warning signal for investors to allocate capital and mitigate portfolio risk.
 
  Final Model Performance 
  (The Winner)Through rigorous comparative testing and hyperparameter tuning, the Tuned LightGBM Classifier was selected as the optimal modela six-fold improvement over random chance in finding rare outcomes.
  
 Methodology & Techniques
 
 The project follows a strategic, production-ready machine learning pipeline:
 
 1-Data Integrity: Implemented checks to drop Target-Leaking columns (e.g., post-event dates) and Identifier columns.
 2-Feature Engineering: Created high-signal features essential for time-series and financial prediction, including Startup Age, Funding Velocity, and Log Transformation of financial features.
 3-Imbalance Handling: Utilized a Stratified Train/Test Split and Balanced Class Weights across all models to specifically counter the $\approx 8:1 class imbalance.
 4-Comparative Analysis: Benchmarked Logistic Regression, Decision Tree, Random Forest (Bagging), and LightGBM (Boosting) to prove the necessity of ensemble methods.
 5-Deployment Ready: The entire preprocessing and model are encapsulated in a single scikit-learn pipeline for easy deployment and future testing.
 
  Repository Contents
  
  status_prediction_notebook.ipynb: Core ML workflow demonstrating data cleaning, pipeline construction, comparative modeling, and evaluation.
  EDA_Finalized_Documented_SICAI.ipynb: Comprehensive Exploratory Data Analysis (EDA) of the startup funding landscape and data distributions.
  df_sample.csv: Sample of the raw dataset used for demonstration.
  README.md (This file): Project summary and key results.
 
