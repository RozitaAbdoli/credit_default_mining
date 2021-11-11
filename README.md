# Credit Default Mining  
Risk management is one of the fastest growing areas in the financial industry. Financial institutions increasingly use Machine Learning (ML) to capture the relevant risks that have been encountered in the past, as well as to predict the probability of loss in the future. In this project, the goal is to build a ML model to predict which customers will default on their credit card payment.The data used is the demographic and payment history of credit card holders in one of the major Taiwanese banks that was collected in October 2005. The [dataset](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) was retrieved from the Machine Learning Repository of the University of California’s School of Information and Computer Science.

The tentative stages of the project can be summarized as data preparation, exploratory data analysis (EDA), feature engineering, feature selection, modeling, and evaluation. However, this is an iterative process and these stages are not to suggest a linear, one-way process. Rather, different stages are interconnected and one needs to go back and forth between stages during the lifecycle of the data science project. What follows is the repository content outline following the stages listed above.
## Repository Content Outline:
This repository contains a set of technical reports in Python/JupyterNotebook format that are listed below. The compilation of the technical reports in PDF format can be found in the folder named 'PDF'. This repository also contains the original dataset named 'credit_default.xls', and the cleaned dataset called '**v2_credit_default.csv**'.
### 1) Data Understanding, Data Cleaning, and Exploratory Data Analysis
- [**DataCleaning+EDA**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/DataCleaning%2BEDA.ipynb)  
- [**EDA_Panda's_profiling_report**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/EDA_Panda's_profiling_report.ipynb): Open in Colab to view the HTML rendering correctly, or see the noninteractive pdf format [here](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/PDF/Pandas_profiling_report.pdf).
- [**EDA_frequent_patterns**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/EDA_frequent_patterns.ipynb)
### 2) Feature Engineering (FE), and Feature Selection (FS)
- [**FE_scaling+balancing**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/FE_scaling%2Bbalancing.ipynb)
- [**FE_normalize+remove_outliers**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/FE_normalize%2Bremove_outliers.ipynb)
- [**FS_correlations**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/FS_correlations.ipynb): Filter method of feature selection. Embbeded methods of feature selection are explored in the next section such as using XGBooster classifier to rank feature importance based on weight (number of times the feature appears in a tree ), or gain (average gain of splits that use the feature). 
### 3) Modeling, and Evaluation
- [**Logistic_regression**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/Logistic_regression.ipynb) : Tuning the logistic regression hyperparameters using Grid Search cross-validation, and running the optimized LR model with selected features from XGBoost.
- [**SVM**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/SVM.ipynb)
- [**XGBoost**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/XGBoost.ipynb)
- [**Model_comparison**](https://github.com/RozitaAbdoli/credit_default_mining/blob/main/Model_comparison.ipynb): This notebook compares the performance of multiple ML algorithms, while the other notebooks go into more details about individual algorithms, such as hyperparameters tuning.


