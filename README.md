# Credit Default Mining:  
Build a ML model to predict which customers will default on their credit card payment.
---------------------------------
## Repository Content Outline:
### Data Understanding, Data Preparation, and Exploratory Data Analysis
- **DataUnderstanding+DataPrep**

    - Data cleaning: ID column is removed, duplicate rows are removed. Some of the attribute names are changed for better readability.
      
    - The categories in the categorical variables Education and Marriage are re-adjusted.
      
    - The cleaned dataset is saved as **v2_credit_default.csv**.
      
- **EDA_Panda's_profiling_report**: Open in Colab to see the HTML rendering correctly.
- **EDA_distributions**: Histogram of distribution, mean, median, and mode.
- **EDA_outliers**: Box plots showing outliers.
- **EDA_correlations**: Sorted Pearson's and Spearman correlations between the independent variables and the dependent variable 'Default'.
---------------------------------
### Modeling and Validation
- **Feature_engineering**: Balancing the dataset by under-sampling, over-sampling, and SMOTE Tomek (undersampling + oversampling) + LR.
- **Feature_selection_using_XGBoost**: Using XGBooster classifier and ranking feature importance based on weight (number of times the feature appears in a tree ), and gain (average gain of splits that use the feature).
- **LR_model_CV** : Tuning the logistic regression hyperparameters using Grid Search cross-validation, and running the optimized LR model with selected features from XGBoost.


