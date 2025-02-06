# Credit Card Fraud Detection

## 📌 Project Overview
This project aims to detect fraudulent transactions in credit card activity using machine learning models. The dataset consists of **100,000 transactions**, including key features like transaction amount, merchant ID, location, and transaction type. The goal is to build a classification model that accurately identifies fraudulent transactions (**IsFraud = 1**) while minimizing false positives and negatives.

## 📊 Dataset Description
The dataset includes the following columns:

- **TransactionID**: Unique identifier for each transaction.
- **TransactionDate**: Timestamp of the transaction.
- **Amount**: Transaction value (monetary amount).
- **MerchantID**: Identifier for the merchant.
- **TransactionType**: Type of transaction (purchase/refund).
- **Location**: Geographic location of the transaction.
- **IsFraud**: Target variable (1 = Fraud, 0 = Legitimate).

## 🚨 Challenge: Data Imbalance
One of the biggest challenges in fraud detection is the **highly imbalanced dataset**, where fraudulent transactions represent only a small percentage of total transactions. This can cause models to favor the majority class (legitimate transactions) and fail to detect fraud accurately.

### 📉 Impact of Imbalance
- **Poor Precision & Recall for Fraud Cases**: The model may predict most transactions as non-fraudulent, leading to **high accuracy but poor fraud detection.**
- **Low AUC-ROC Scores**: The model struggles to distinguish between fraud and non-fraud transactions.
- **Bias Toward Majority Class**: Traditional machine learning models like Random Forest and XGBoost tend to predict fraud cases poorly without resampling techniques.

## 🤖 Model Performance & Evaluation
### 🏆 Best Performing Models
- **Random Forest (Balanced Weights) 🎯**
- **XGBoost (Optimized with Hyperparameter Tuning) 🚀**

### 📈 Metrics Used
- **Confusion Matrix**: To evaluate misclassification.
- **Precision, Recall & F1-Score**: For fraud detection performance.
- **AUC-ROC Score**: To measure overall model effectiveness.

## 🚀 Future Enhancements
- 🔍 **More Advanced Anomaly Detection**: Implement techniques like **Autoencoders, Isolation Forests, or One-Class SVM**.
- ⚡ **Deep Learning Models**: Train **LSTMs or CNNs** to detect fraud patterns in transaction sequences.
- 📅 **Time-Series Analysis**: Identify fraud trends over time using **RNNs or ARIMA models**.
- 📊 **Feature Engineering**: Add more transactional behavior-based features.
- ⚖ **Ensemble Learning**: Combine multiple models (e.g., stacking, boosting) to improve fraud detection accuracy.
- 🏦 **Domain-Specific Rules**: Introduce financial fraud detection heuristics alongside machine learning models.
