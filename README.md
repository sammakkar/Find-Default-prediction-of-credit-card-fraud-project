# Find-Default-prediction-of-credit-card-fraud-project

## Project Overview
Credit card fraud is a significant problem that affects both financial institutions and customers. This project uses machine learning techniques to build a model that can identify fraudulent credit card transactions, aiming to reduce the impact of fraud.

## Problem Statment 
A credit card is one of the most used financial products to make online purchases and payments. Though the Credit cards can be a convenient way to manage your finances, they can also be risky. Credit card fraud is the unauthorized use of someone else's credit card or credit card information to make purchases or withdraw cash.
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. 
The dataset contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
We have to build a classification model to predict whether a transaction is fraudulent or not.

## Project Structure
- **dataset(s)**: Contains the raw and cleaned datasets.
- **notebooks**: Jupyter notebooks for exploratory data analysis and model development.
- **visula**: Contains performance evaluation reports, visualisations and eda plots.
- **models**: Machine learning models used for modelling.
- **requirements.txt**: This file contains required packages along with their version

## Dataset
The dataset used in this project is a collection of credit card transactions from September 2013. It contains 284,807 transactions, of which 492 are identified as fraudulent. The dataset includes 23 features related to transaction details, excluding sensitive information like card numbers.

**Features**
1. V1, V2, ... V28: PCA-reduced features from the original dataset
2. Time: Time elapsed since the first transaction in the dataset
3. Amount: Transaction amount
4. Class: Target variable (1 for fraudulent, 0 for legitimate)

## Technologies Used
Python
Pandas
NumPy
Scikit-learn
Matplotlib
Seaborn
Jupyter Notebook

## Modeling Techniques
**This project explores several machine learning algorithms, including:**
1. Logistic Regression
2. Decision Trees
3. Random Forest
4. Support Vector Machines (SVM)
5. Gradient Boosting Classifier
6. XGBoost
7. LightGB

## Evaluation Metrics
I used metrics such as accuracy, precision, recall, auc_score, and f1-score to evaluate model performance

## Conclusion
In this project, we developed and evaluated multiple machine learning models to detect fraudulent credit card transactions balancing the imbalanced dataset. Through data preprocessing and feature engineering, we effectively enhanced the model's ability to identify fraud cases. The results indicate that our models achieved satisfactory performance, with some models demonstrating high precision and recall, which are critical in minimizing false negatives. Overall, this project contributes valuable insights into the application of machine learning in fraud detection and provides a framework for further exploration in this domain.

## Future Work
**While the current models have shown promising results, several avenues for future work can enhance their effectiveness:**

1. Advanced Feature Engineering: Investigating additional features, such as customer behavior analysis and transaction patterns, could provide deeper insights into fraudulent activities.
2. Real-Time Detection: Implementing the models in a real-time processing environment could enable instantaneous fraud detection, significantly reducing potential losses.
3. Explainability: Integrating explainable AI methods will help stakeholders understand the decision-making process of the models, thereby building trust and facilitating better business decisions.

## Business Insights
**The implementation of a robust credit card fraud detection system can yield significant benefits for businesses, including:**

1. Reduced Financial Losses: By accurately identifying fraudulent transactions, companies can minimize losses associated with chargebacks and fraud-related costs.
2. Improved Customer Trust: Enhancing security measures helps build customer confidence, leading to increased loyalty and potentially higher transaction volumes.
3. Operational Efficiency: Automating the fraud detection process reduces the need for manual reviews, allowing teams to focus on more strategic initiatives and reducing operational costs.
4. Regulatory Compliance: A strong fraud detection system can assist businesses in adhering to regulatory requirements regarding financial transactions, mitigating compliance risks.
5. Data-Driven Decision Making: Insights gained from the fraud detection system can inform business strategies, marketing efforts, and customer relationship management by identifying patterns in consumer behavior.

By leveraging advanced fraud detection techniques, organizations can not only protect themselves from financial risks but also enhance their overall operational framework and customer experience.
