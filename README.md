# Default_of_credit_card_clients
# Credit Card Default Risk Prediction

> **Data Mining Course Project** | Sharif University of Technology  
> **Authors:** Sajjad Saeedi & Saba Yousefzadeh  
> **Instructor:** Dr. Bostan-ara  

---

##  Overview
This project predicts credit card default risk using a dataset of 30,000 clients from the UCI Repository. We addressed class imbalance (~22.1% default rate) using cost-sensitive learning and evaluated performance primarily via **PR-AUC** and **ROC-AUC**.

##  Main Results

| Model | Accuracy | Recall | F1-Score | ROC-AUC | PR-AUC |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **XGBoost (Best)** 🏆 | **0.7606** | **0.6237** | **0.5354** | **0.7810** | **0.5634** |
| **LightGBM** | 0.7530 | 0.6259 | 0.5287 | 0.7799 | 0.5537 |
| **Random Forest** | 0.7744 | 0.5837 | 0.5321 | 0.7729 | 0.5548 |
| **Logistic Regression** | 0.7640 | 0.5732 | 0.5291 | 0.7742 | 0.5346 |

##  Key Insights
- **Top Risk Factors:** Recent repayment delay (`PAY_0`), credit limit (`LIMIT_BAL`), and credit utilization ratio (`CREDIT_UTILIZATION`).
- **Interpretability:** Evaluated global and local feature impacts using **SHAP** values and confusion matrix error analysis.
