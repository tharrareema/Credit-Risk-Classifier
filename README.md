## Credit Risk Classification Model (KNN, Decision Trees, Ensemble)

<details>
<summary>Click to expand</summary>

### 🧠 Project Title
**Comparative Credit Risk Modeling for Loan Default Prediction**

### 📘 Project Description
Built, compared, and optimized **KNN, Decision Trees, Random Forest, and XGBoost** to classify loan applicants by credit risk. Focused on minimizing financial losses with hyperparameter tuning, cross-validation, and metrics like **AUC** and **Precision/Recall**.

### 🎯 Business Task
- Predict loan default probability accurately  
- Compare models to select the most reliable classifier  
- Identify top features influencing creditworthiness  

### 📁 Dataset Summary

| Feature | Description |
|---------|-------------|
| 👤 Applicant Demographics | Age, Income, Employment Status |
| 💳 Credit History | Existing debt, past loan performance, credit score |
| 💰 Loan Details | Requested amount, term, purpose |
| 🎯 Target Variable | Loan Status (Default / Non-Default) |

**Data Source:** German Credit Data / Public Loan Risk Dataset

### 🧰 Tools & Technologies
Python • Pandas • NumPy • Scikit-learn • XGBoost / LightGBM • Matplotlib • Seaborn

### 🧹 Data Cleaning & Preparation
- **Class Imbalance:** SMOTE or class weighting for Default / Non-Default  
- **Feature Encoding:** One-hot encoding for categorical variables  
- **Standard Scaling:** Normalized numeric features for KNN  

### 📊 Model Performance

| Model | Technique | Key Hyperparameters | Best AUC | Best F1 |
|-------|-----------|-------------------|----------|---------|
| KNN | Instance-based | n_neighbors=15, weights='distance' | 0.68 | 0.55 |
| Decision Tree | Single Model | max_depth=7, criterion='gini' | 0.71 | 0.61 |
| Random Forest | Ensemble (Bagging) | n_estimators=200, max_features='sqrt' | 0.77 | 0.69 |
| XGBoost Classifier | Ensemble (Boosting) | learning_rate=0.05, n_estimators=300 | 0.81 | 0.75 |

**Conclusion:** XGBoost had the highest AUC and F1, making it the preferred model for deployment.

### 💡 Strategic Recommendations
- **Ensemble Deployment:** Deploy XGBoost to minimize false negatives  
- **Feature Prioritization:** Use top features (Credit Score, Existing Debt) for early-stage loan filtering  
- **Model Monitoring:** Track drift over time as economic conditions change  

</details>

---
