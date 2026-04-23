# PortugueseBankDataAnalysis-
A comparative study of 4 machine learning algorithms to predict whether a bank customer will subscribe to a term deposit.
Bank Marketing Campaign: Predicting Term Deposit Subscriptions
A comparative study of 4 machine learning algorithms to predict whether a bank customer will subscribe to a term deposit.

# Overview
This project applies and compares four classification algorithms on the UCI Bank Marketing Dataset (11,162 customer records, 16 features) to predict deposit subscription (yes/no). The goal is to help marketing teams prioritize high-potential customers and optimize campaign ROI.

# Algorithms Implemented
### 🌲 Decision Tree – Interpretable if-then rules

### 🧮 Naive Bayes – Probabilistic approach assuming feature independence

### 📍 K-Nearest Neighbors (KNN) – Distance-based similarity voting

### 🧠 Artificial Neural Network (ANN) – Multi-layer perceptron with ReLU/Sigmoid activations

## Key Preprocessing Steps
1. Removed duration (prevents target leakage – call length unknown before calling)

2. Label Encoding for ordinal features (education, month)

3. One-Hot Encoding for nominal features (job, marital, contact, etc.)

4. Feature scaling (StandardScaler) for KNN and ANN

# Key Insight on Results 
Naive Bayes achieved the highest accuracy (67.13%) and best overall balance. ANN caught the most actual "yes" customers (highest recall: 67%) but made more false positive calls. Decision Tree was most precise (72%) but missed half of potential depositors.

## Technologies Used
1. Python 3.13

2. pandas, numpy – Data manipulation

2. scikit-learn – All 4 algorithms, preprocessing, evaluation metrics

3. matplotlib, seaborn – Confusion matrix heatmaps


### Future Improvements
Hyperparameter tuning with GridSearchCV

Cross-validation for more robust evaluation

Random Forest and Gradient Boosting ensembles

ROC curves and AUC scoring
