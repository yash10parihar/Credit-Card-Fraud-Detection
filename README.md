# Credit Card Fraud Detection using Machine Learning

This project demonstrates a predictive modeling approach to detect fraudulent credit card transactions using a synthetic dataset. It was completed as part of the *Predictive Modeling (OPIM 5604)* course at the University of Connecticut.

## 🧠 Objective

To build and compare multiple machine learning models that can identify fraudulent transactions based on behavioral and demographic features.

## 📊 Dataset

- Source: [Kaggle - Credit Card Fraud Prediction](https://www.kaggle.com/datasets/kelvinkelue/credit-card-fraudprediction)
- Size: 555,719 transactions with 22 features
- Target: `is_fraud` (1 = fraud, 0 = legitimate)

### Sample Features:
- Transaction amount (`amt`)
- Timestamp (`trans_date_trans_time`)
- Merchant & category info
- Cardholder details (age, job, gender, location)
- Merchant & cardholder geolocation (lat/long)
- Calculated distance between cardholder and merchant

## ⚙️ Modeling Techniques

The following models were trained and evaluated:
- Logistic Regression
- Decision Tree
- Boosted Tree
- Bootstrap Forest
- Neural Network
- Discriminant Analysis
- k-Nearest Neighbors (KNN)
- Naive Bayes

## 🔍 Feature Engineering

- Extracted daytime periods from timestamps
- Categorical grouping of jobs and states based on fraud prevalence
- Calculated distance between cardholder and merchant locations using Great-Circle Distance
- Handled outliers in transaction amounts
- Transformed `dob` to age feature

## 📈 Results

- **Best Model**: Neural Network  
  - Overall Accuracy: 99.8%  
  - True Positive Rate (Fraud Detection): 65.5%  
  - Misclassification Rate: 0.19%

The neural network model showed the highest ability to detect fraud without prior feature selection.

## 🔐 Business Recommendations

- Flag high-value and late-night transactions for extra verification
- Apply targeted fraud detection rules for specific occupations and locations
- Incorporate geolocation-based risk scoring for transactions

## 👨‍💻 Team Members

- Yash Parihar  
- Group 3, OPIM 5604, University of Connecticut

## 📅 Date

June 24, 2025

## 📜 License

This project is academic and for educational purposes only.
