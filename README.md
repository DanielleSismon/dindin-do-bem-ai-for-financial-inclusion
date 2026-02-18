# 🏦 DinDin do Bem - AI for Financial Inclusion
### *Behavioral Credit Scoring using Deep Learning (Neural Networks)*

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit__learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Deep Learning](https://img.shields.io/badge/Deep_Learning-MLP-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> **The Mission:** Proving that *Behavior* is a better predictor of creditworthiness than just *Income*, enabling financial inclusion for vulnerable women.

---

## 🎯 Project Overview
In the traditional banking system, millions of women (widows, divorced, informal workers) are "invisible" because they lack a formal credit history (the **"Thin File"** problem).

**"DinDin do Bem"** is a machine learning project that builds a **Fair Credit Scoring Engine**. Instead of relying solely on financial history, we use **Alternative Data** (e.g., stability of phone number, housing type, social reputation) to predict repayment risk using a **Multi-Layer Perceptron (Neural Network)**.

### 🧠 The Solution
We built a robust pipeline that:
1. **Processes Alternative Data:** Engineering features like `DAYS_LAST_PHONE_CHANGE` as a proxy for stability.
2. **Mitigates Bias:** Using **SMOTE** (Synthetic Minority Over-sampling Technique) to balance the dataset and ensure the model learns to identify defaulters accurately.
3. **Deep Learning Model:** A Neural Network (MLPClassifier) with a funnel architecture (100 -> 50 neurons) to capture non-linear patterns in behavioral data.

---

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Machine Learning:** Scikit-Learn (`MLPClassifier`, `Pipeline`, `ColumnTransformer`)
* **Data Handling:** Pandas, NumPy, Imbalanced-Learn (`SMOTE`)
* **Evaluation:** Recall (Business Metric), ROC-AUC, Confusion Matrix

### 📊 Key Results
The model was put to the test with two distinct personas:

| Persona | Profile | Traditional View | AI Verdict | Why? |
| :--- | :--- | :--- | :--- | :--- |
| **Dona Maria** | Widow, Low Income, High Stability (8 years same phone number) | ❌ High Risk | **✅ Approved** | Stability & Community Score outweighed low income. |
| **Dona Joana** | Single, High Income, High Instability (New job, new phone) | ✅ Low Risk | **❌ Denied** | Behavioral instability flagged as high risk. |

> *"The behavior and stability are predictors of trust as strong as formal income."*

---

## 🚀 How to Run
1.  Clone this repository.
2.  Install requirements: `pip install pandas numpy scikit-learn imbalanced-learn seaborn`
3.  Run the Jupyter Notebook: `jupyter notebook behavioral_credit_scoring_dl.ipynb`

---

## 👩‍💻 Author
**Danielle Sismon**
*Aspiring AI Engineer & Data Scientist | Transitioning from Law to Tech*
[LinkedIn](wwww.linkedin.com/in/danielle-sismon) | [Portfolio](https://github.com/DanielleSismon)

---
*Developed as part of the Machine Learning course at FATEC (São Paulo State Technology College).*
