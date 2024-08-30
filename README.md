# Credit Card Fraud Detection Project

This project aims to develop and evaluate machine learning models to detect and prevent credit card fraud using a dataset of transactions made by European cardholders in 2023. The dataset contains over 550,000 records with anonymized features, facilitating the creation of robust fraud detection algorithms.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Models and Evaluation](#models-and-evaluation)
4. [Results](#results)
5. [Potential Use Cases](#potential-use-cases)
6. [Acknowledgements](#acknowledgements)

## Project Overview

The primary goal of this project is to build machine learning models to detect fraudulent transactions in credit card data. By leveraging various algorithms, the project aims to maximize accuracy and minimize false positives and false negatives in fraud detection.

## Dataset

The dataset used in this project was collected from Kaggle and includes the following features:

- **id**: Unique identifier for each transaction.
- **V1 - V28**: Anonymized features derived from the original data.
- **Amount**: The transaction amount.
- **Class**: Binary label indicating whether the transaction is fraudulent (1) or not (0).

### Sample Data

| id | V1      | V2      | ... | V28     | Amount  | Class |
|----|---------|---------|-----|---------|---------|-------|
| 0  | -0.2606 | -0.4696 | ... | -0.1510 | 17982.1 | 0     |
| 1  | 0.9851  | -0.3560 | ... | -0.0645 | 6531.37 | 0     |
| 2  | -0.2602 | -0.9494 | ... | -0.2447 | 2513.54 | 0     |
| 3  | -0.1521 | -0.5090 | ... | 0.0484  | 5384.44 | 0     |
| 4  | -0.2068 | -0.1653 | ... | 0.4191  | 14278.9 | 0     |

## Models and Evaluation

The project explores several machine learning algorithms for fraud detection, including:

- **Random Forest**
- **XGBoost**
- **LightGBM**
- **Gradient Boosting**
- **Decision Tree**
- **Logistic Regression**

### Performance Metrics

Models are evaluated based on the following metrics:

- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **AUC-ROC**

## Results

| Model               | Accuracy  | Precision | Recall   | F1 Score | AUC-ROC  | Training Time (s) |
|---------------------|-----------|-----------|----------|----------|----------|--------------------|
| Random Forest       | 0.999833  | 0.999666  | 1.000000 | 0.999833 | 0.999990 | 462.202911         |
| XGBoost             | 0.999701  | 0.999402  | 1.000000 | 0.999701 | 0.999982 | 12.069369          |
| LightGBM            | 0.999112  | 0.998472  | 0.999754 | 0.999112 | 0.999811 | 14.678621          |
| Gradient Boosting   | 0.979292  | 0.988581  | 0.969787 | 0.979094 | 0.998644 | 1002.004688        |
| Decision Tree       | 0.997775  | 0.996840  | 0.998716 | 0.997777 | 0.997775 | 63.872897          |
| Logistic Regression | 0.964960  | 0.977083  | 0.952254 | 0.964509 | 0.993507 | 7.915467           |

## Potential Use Cases

- **Credit Card Fraud Detection**: Deploy machine learning models in real-time systems to monitor transactions and flag suspicious activities.
- **Merchant Category Analysis**: Examine how different merchant categories are associated with fraud.
- **Transaction Type Analysis**: Analyze whether certain types of transactions are more prone to fraud than others.

## Acknowledgements

- This project utilizes the Credit Card Fraud Detection 2023 dataset from Kaggle. Please find it here: https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023
