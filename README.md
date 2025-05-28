Dataset Link : https://www.kaggle.com/datasets/chitwanmanchanda/fraudulent-transactions-data

# Fraudulent Transactions Detection

This project aims to develop a model for predicting fraudulent transactions for a financial company. The goal is to use insights from the model to develop an actionable plan for reducing fraud and enhancing the company’s security and customer trust.

---

## 📁 Dataset

- **Source**: Provided CSV file  
- **Size**: 6,362,620 rows and 10 columns  
- **Features**:
  - `step`: Hourly time step (1 step = 1 hour)
  - `type`: Transaction type (CASH-IN, CASH-OUT, DEBIT, PAYMENT, TRANSFER)
  - `amount`: Transaction amount
  - `nameOrig`: Customer initiating the transaction
  - `oldbalanceOrg`: Initial balance of the origin customer
  - `newbalanceOrig`: New balance of the origin customer
  - `nameDest`: Recipient of the transaction
  - `oldbalanceDest`: Initial balance of the recipient
  - `newbalanceDest`: New balance of the recipient
  - `isFraud`: Indicator if the transaction was fraudulent
  - `isFlaggedFraud`: Flag for suspicious high-value transactions (> 200,000)

---

## 🧪 Project Steps

1. **Data Cleaning & Preprocessing**
   - Handled missing values and outliers.
   - Addressed multicollinearity where necessary.

2. **Exploratory Data Analysis (EDA)**
   - Visualized transaction types, amounts, and suspicious patterns.
   - Checked for class imbalance and handled it appropriately.

3. **Feature Engineering & Selection**
   - Created new features (e.g., balance differences).
   - Selected features using feature importance and domain knowledge.

4. **Model Building**
   - Trained multiple models (e.g., Random Forest, XGBoost).
   - Tuned hyperparameters using cross-validation.

5. **Model Evaluation**
   - Evaluated models using recall, precision, F1-score, ROC-AUC.
   - Focused on **recall** due to the cost of missing fraudulent transactions.

6. **Insights & Key Drivers**
   - Identified key factors (transaction type, balance differences, amount).
   - Checked if these insights make business sense.

7. **Recommendations & Action Plan**
   - Proposed fraud prevention actions (e.g., real-time flagging, customer verification).
   - Suggested monitoring plans to measure success.

---

## ⚙️ Technologies Used

- **Python** (pandas, numpy, scikit-learn, XGBoost, matplotlib, seaborn)
- **Jupyter Notebook** for exploratory analysis and model development

---

## 📈 Key Outcomes

- Developed a robust model with good performance on validation data.
- Identified high-risk transaction patterns for targeted fraud prevention.
- Provided actionable recommendations to improve infrastructure and monitoring.

---
