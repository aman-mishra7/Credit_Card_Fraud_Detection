# Credit_Card_Fraud_Detection
This repository develops a fraud detection system using unsupervised learning techniques like KMeans, Isolation Forest, and OneClassSVM to flag suspicious transactions. The solution is scalable, modular, and outputs flagged transactions in flagged_fraud_transactions.csv for further review.

# Fraud Detection System for Company ABC

## Problem Statement

Company ABC, a major credit card company, is facing challenges with its existing fraud detection system, which struggles to quickly recognize new patterns of fraudulent activity. This delay results in significant financial losses. The company has contracted us to design and implement a more efficient algorithm to detect and flag potentially fraudulent transactions for further investigation. The provided data consists of two tables:

- `cc_info`: Contains general credit card and cardholder information.
- `transactions`: Contains detailed records of credit card transactions that occurred between August 1st and October 30th.

## Objective

The objective of this project is to develop an advanced fraud detection system using neural networks to identify unusual and potentially fraudulent transactions. Our aim is to build a scalable and modular solution capable of handling large volumes of data and providing valuable insights to Company ABC.

## Approach

This project focuses on unsupervised machine learning methods to identify anomalous transactions. We utilize various algorithms and techniques to develop the fraud detection model:

1. **Data Preprocessing**: Standardized data using `StandardScaler` to normalize the features.
2. **Clustering**: Applied KMeans clustering for anomaly detection and exploration of data patterns.
3. **Anomaly Detection Algorithms**: Used several unsupervised learning methods to detect outliers, including:
   - `IsolationForest`
   - `LocalOutlierFactor`
   - `OneClassSVM`
4. **Model Evaluation**: Assessed the model's performance using metrics like ROC curves, AUC, precision-recall curves, and silhouette scores. The `KneeLocator` library was used to determine the optimal number of clusters.

## Tools and Libraries

The following Python libraries were used for data manipulation, visualization, modeling, and evaluation:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn` (for clustering, anomaly detection, and model evaluation)
- `kneed` (for determining the optimal number of clusters)

## Output

The result of the model is an output CSV file named `flagged_fraud_transactions.csv` containing transactions that have been flagged as potentially fraudulent, enabling Company ABC to take proactive measures against fraud.

## Conclusion

This repository provides a comprehensive approach to detecting fraudulent transactions using unsupervised learning techniques. It serves as a scalable and efficient solution to enhance the fraud detection capabilities of Company ABC, reducing financial losses and ensuring better customer protection.
