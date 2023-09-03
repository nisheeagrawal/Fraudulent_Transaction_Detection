# **Transaction Fraud Detection**

## GOAL: **Identify/Predict Fraudulent Transactions**
    Predicting the probability that an online transaction is fraudulent, as denoted by the binary target feature "isFraud"
<br/>

## DEPENDANCIES: Tools used 
    * Python - dynamically-typed and garbage-collected programming language
    * Pandas - software library for data manipulation and analysis
    * Scikit-learn - machine learning library
        - XGBoost (sklearn)
        - SMOTE (sklearn)
        - SimpleImputer (sklearn.impute)
    * LightGBM
<br/>

## STEPS: To Run the project:
1. Run All cells in `1_data_cleaning.ipynb` to clean the dataset and populate the datasets_cleaned directory
2. Run All cells in `2_data_exploration.ipynb` to perform Exploratory data analysis and explore the outliers
3. Run All cells in `3_modeling.ipynb` to run the modeling
<br/><br/>

## ORGANIZATION: Project Folder Structure
```
root folder
│   📜 README.md
│   📜 1_data_cleaning.ipynb
│   📜 2_data_exploration.ipynb
│   📜 3_modeling.ipynb

└───📂 datasets_initial
    │   📜 sample_submission.csv
    │   📜 test_identity.csv
    │   📜 test_transaction.csv
    │   📜 train_identity.csv
    │   📜 train_transaction.csv
    
└───📂 datasets_intermediate
    │   📜 imputed_test.csv
    │   📜 imputed_train.csv
    │   📜 test.csv
    │   📜 train.csv

└───📂 datasets_cleaned
    │   📜 final_test.csv
    │   📜 final_train.csv

└───📂 datasets_modeling
    │   📜 test_dummy.pickle
    │   📜 train_dummy.pickle
    │   📜 X_new.pickle

```
<br/>

## SIZE: Dataset source:
* IEEE-CIS Fraud Detection [Dataset provided by Vesta Corporation](https://www.kaggle.com/c/ieee-fraud-detection)
* **590540 records, 433 features**
* train_transaction, test_transaction, train_identity, test_identity, and sample_submission
* Problem: binary classification
<br/>
<br/>

## ANALYSIS: Steps followed, Challenges faced, Methoddologies used 

**Steps:**
1. Loading data
2. Data Cleaning
3. Data Exploration
4. Feature Selection
5. Model Selection
6. Tuning

**Challenges:**
1. Unbalanced data
2. A lot of missing values
3. Feature selection 
4. Model selection
5. Large dataset

**Methodologies:**
- Imputation methods — SimpleImputer - Imputation transformer for completing missing values.
- Classification methodologies
    - LightGBM - A fast, distributed, high performance gradient boosting (GBT, GBDT, GBRT, GBM or MART) framework based on decision tree algorithms, used for ranking, classification and many other machine learning tasks.
- Feature Engineering (Selection from Model)
    - XGBoost (sklearn)
- Under/Over sampling
    - SMOTE (sklearn) - Synthetic minority over sampling technique — SMOTE - An approach to the construction of classifiers from imbalanced datasets is described
<br/><br/>

## WRITE UP: 
    The goals that we were trying to accomplish, the results obtained are all mentioned in a markdown cell inside each of the notebooks right below the result tables/graphs.

## TEAM: 
    Nishee Agrawal - 827172184
    Manu Srirangarajan - 825830363