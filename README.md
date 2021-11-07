# Credit Default Mining  
Risk management is one of the fastest growing areas in the financial industry. Financial institutions increasingly use Machine Learning (ML) to capture the relevant risks that have been encountered in the past, as well as to predict the probability of loss in the future. In this project, the goal is to build a ML model to predict which customers will default on their credit card payment.The data used is the demographic and payment history of credit card holders in one of the major Taiwanese banks that was collected in October 2005. The [dataset](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) was retrieved from the Machine Learning Repository of the University of California’s School of Information and Computer Science.

The tentative stages of the project can be summarized as data preparation, exploratory data analysis (EDA), feature engineering, feature selection, modeling, and evaluation. However, this is an iterative process and these stages are not to suggest a linear, one-way process. Rather, different stages are interconnected and one needs to go back and forth between stages during the lifecycle of the data science project. What follows is the repository content outline following the stages listed above.
## Repository Content Outline:
This repository contains a set of technical reports in Python/JupyterNotebook format that are listed below. The compilation of the technical reports in PDF format can be found in the folder named 'PDF'. This repository also contains the original dataset named 'credit_default.xls', and the cleaned dataset called '**v2_credit_default.csv**'.
### 1) Data Understanding, Data Cleaning, and Exploratory Data Analysis
- **DataCleaning+EDA**  
- **EDA_Panda's_profiling_report**: Open in Colab to see the HTML rendering correctly.
- **EDA_frequent_patterns**
### 2) Feature Engineering (FE), and Feature Selection (FS)
- **FE_scaling+balancing**
- **FE_normaliza+remove_outliers**
- **FS_correlations**: Filter method of feature selection. Embbeded methods of feature selection are explored in the next section such as using XGBooster classifier to rank feature importance based on weight (number of times the feature appears in a tree ), or gain (average gain of splits that use the feature). 
### 3) Modeling, and Evaluation
- **Logistic_regression** : Tuning the logistic regression hyperparameters using Grid Search cross-validation, and running the optimized LR model with selected features from XGBoost.
- **SVM**
- **XGBoost**


