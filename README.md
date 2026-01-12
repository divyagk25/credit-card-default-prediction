

# 📊 Credit Card Approval Prediction
## A Comparative Study of Classification Models

---

##  Project Overview
This project applies multiple machine learning classification models to predict whether a credit card application will be **approved or rejected** using applicant demographic and financial attributes. The focus is on **model comparison, interpretability, and risk-aware evaluation**, reflecting real-world financial decision-making constraints.

---

##  Business Context
Credit card approval is a high-impact decision process for financial institutions.

- False approvals increase exposure to default risk  
- False rejections result in lost revenue and customer attrition  

The problem is formulated as a **binary classification task** and evaluated using metrics that account for the **asymmetric cost of misclassification**, rather than accuracy alone.

---

##  Data & Target Definition

### Target Variable
| Value | Meaning |
|------:|--------|
| 0 | Application approved |
| 1 | Application rejected |

### Dataset Characteristics
- Anonymized applicant-level demographic and financial data  
- Strong class imbalance:
  - **Approved:** ~89%  
  - **Rejected:** ~11%  

This imbalance reflects realistic credit approval distributions and directly informs modeling decisions.

---

##  Exploratory Data Analysis (Summary)
Exploratory data analysis was conducted to assess data quality, feature distributions, and early risk patterns. This included missing value treatment, transformation of time-based variables into interpretable features (age and employment duration), and univariate and bivariate analysis. Correlation analysis revealed weak linear relationships with the target variable, motivating the use of non-linear and ensemble models.

---


## 🤖 Modeling & Performance Summary

### Models Evaluated
- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Support Vector Machines (SVM)  
- Decision Trees  
- Random Forests  

### Evaluation Metrics
- Precision  
- Recall  
- F1-score  
- ROC–AUC  
- Confusion Matrix  

---

### Model Behaviour Insights
- **Logistic Regression:** interpretable and stable baseline  
- **KNN & SVM:** sensitive to feature scaling and hyperparameter tuning  
- **Decision Trees:** capture non-linear relationships but are prone to overfitting  
- **Random Forests:** strongest overall performance with reduced variance and improved robustness  

---

##  Limitations & Assumptions
- Limited dataset size and representativeness  
- No temporal or time-based validation  
- No explicit cost-sensitive loss optimisation  

---

##  Conclusion
This project demonstrates that **comparative modeling is essential** in credit risk analytics. While ensemble methods improve predictive performance, simpler models remain critical for transparency and regulatory considerations. Effective credit approval systems must balance accuracy, interpretability, and risk sensitivity.

---

##  Repository Structure
```text
notebooks/   → Jupyter notebook with full analysis  
reports/     → Project report  
images/      → Visual outputs 



