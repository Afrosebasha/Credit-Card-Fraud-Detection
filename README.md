# Credit-Card-Fraud-Detection
Credit Card Fraud Detection uses machine learning to identify fraudulent transactions. The dataset is preprocessed, balanced with SMOTE, and classified using a Decision Tree model, which outperformed Logistic Regression. Future improvements include hyperparameter tuning and deep learning.

## Project Overview

Credit card fraud is a growing concern for financial institutions and consumers, particularly with the increasing volume of online transactions. Detecting fraudulent activities accurately is essential to minimizing financial losses and ensuring secure transactions. This project focuses on building a fraud detection system using Python and machine learning techniques with scikit-learn.

## Dataset Overview

For security reasons, the column names in the dataset have been modified. However, the dataset includes a class variable, where:
- 0 represents a normal transaction
- 1 represents a fraudulent transaction

## Data Preprocessing

- **Null Values:** No missing values were found in the dataset.
- **Duplicate Records:** Identified and removed approximately 30,000 duplicate records to ensure data integrity.
- **Standardization:** Applied standardization techniques to normalize all numerical features, including the transaction amount, to improve model performance.

## Model Development

- **Train-Test Split:** The dataset was split into 80 percent training data and 20 percent testing data.
- **Initial Models:** Implemented Logistic Regression and Decision Tree Classifier to evaluate classification performance.
- **Performance Metrics:** Measured accuracy, precision, recall, and F1-score for both models.
- **Class Imbalance Handling:**
  - Identified severe class imbalance: 283,252 normal transactions and 473 fraudulent transactions.
  - Used SMOTE (Synthetic Minority Over-Sampling Technique) to balance the dataset, ensuring meaningful predictions.
- **Final Model Selection:** After re-training with the balanced dataset, the Decision Tree model outperformed Logistic Regression, achieving better classification metrics.

## Model Deployment

- **Model Saving:** The trained model was saved using Joblib for future predictions.
- **Prediction Framework:** Created a dataframe-based input system, allowing users to input transaction details and predict whether a transaction is fraudulent or normal using the Decision Tree model.

## Future Enhancements

- Implement additional machine learning models for improved performance.
- Apply hyperparameter tuning to further optimize classification accuracy.
- Explore deep learning techniques for enhanced fraud detection.

