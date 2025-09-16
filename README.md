# Credit Card Fraud Detection

## Dataset Information
Credit card companies need to identify fraudulent transactions to prevent customers from being charged for purchases they did not make.

The dataset contains transactions made by European cardholders in September 2013. It includes transactions over two days, with **492 fraudulent transactions** out of **284,807 total transactions**. The dataset is highly imbalanced, with the positive class (frauds) accounting for only **0.172% of all transactions**.

All features are numerical and the result of a PCA transformation, except for:
- `Time`: seconds elapsed between each transaction and the first transaction in the dataset.
- `Amount`: transaction amount, which can be used for example-dependent cost-sensitive learning.
- `Class`: response variable, where `1` indicates fraud and `0` otherwise.

**Features:** `V1, V2, ..., V28` (principal components from PCA)  

> Note: Due to confidentiality, the original features are not provided.

Given the high class imbalance, it is recommended to evaluate model performance using **Area Under the Precision-Recall Curve (AUPRC)** rather than traditional accuracy metrics.

**Dataset Link:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)

---

## Libraries Used
- `pandas`  
- `matplotlib`  
- `seaborn`  
- `scikit-learn`  

## Algorithms Implemented
- Logistic Regression  
- Random Forest  
- XGBoost  

## Best Model
- **F1 Score:** 87.00%
