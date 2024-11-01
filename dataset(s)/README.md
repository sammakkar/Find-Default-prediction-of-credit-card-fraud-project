# FindDefault (Prediction of Credit Card fraud)

The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
We have to build a classification model to predict whether a transaction is fraudulent or not.

## Dataset Fields

- **Time**: The number of seconds elapsed between this transaction and the first transaction in the dataset.
- **V1 to V28**: These are the anonymized features obtained using PCA (Principal Component Analysis). They represent various characteristics of the transactions.
- **Amount**: The transaction amount.
- **Class**: This is the target variable where `0` indicates a non-fraudulent transaction and `1` indicates a fraudulent transaction.

## Data Cleaning Steps

1. **Loading the Data**: The dataset was loaded from a CSV file.

2. **Understanding the Data**:
   - Making the dataset undersatndable by knowing it's shape, info, columns, statistical values(like mean, median using describe() command), skewness and             kurtosis also.
  
4. **Handling Missing Values**: 
   - Checked for any missing values across the dataset, but there were no missing values. 

5. **Removing Duplicates**:
   - Any duplicate transactions were removed from the dataset to ensure that each entry is unique.
  
6. **Outliers Treatment**:
   - found outliers in both fraudulent and non-fraudulent transactions but capped outliers from non-fraudulent transaction because outliers in fradulent              transactions may be important for modelling.

7. **Standardizing the 'Amount' and 'Time' Column**:
   - The 'Amount' column was standardized using `StandardScaler` to bring the feature to a common scale, which is important for many machine learning algorithms.

8. **Feature Selection(Dropping Unnecessary Columns)**:
   - saw correlation of all columns with target feature 'Class' and removed less correlated columns to reduce data dimensionality.

9. **Saving the Cleaned Data**:
   - The cleaned data was saved into a new CSV file (`cleaned_data.csv`) for further analysis and modeling.

## Conclusion

This cleaned dataset is ready for exploratory data analysis, feature engineering, and machine learning model training.
