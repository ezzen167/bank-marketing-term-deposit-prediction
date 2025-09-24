# 📌 Term Deposit Subscription Prediction (Bank Marketing)

## 📝 Problem Statement

Banks often run marketing campaigns to convince customers to subscribe
to term deposits. The challenge is to predict **whether a customer will
subscribe** (yes/no) based on demographic and behavioral data.

**Objective:**\
- Build classification models to predict customer subscription.\
- Evaluate performance using **Confusion Matrix, F1-score, and ROC
Curve**.\
- Apply **Explainable AI (XAI)** techniques (SHAP) to interpret
predictions.

------------------------------------------------------------------------

## 📂 Dataset

**Source:** [UCI Bank Marketing
Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)

-   **Rows:** 45,211\
-   **Target variable (`y`)**:
    -   `yes` → subscribed (1)\
    -   `no` → not subscribed (0)

------------------------------------------------------------------------

## ⚙️ Approach

1.  **Data Loading & Cleaning**
    -   Handled categorical variables with One-Hot Encoding\
    -   Mapped target variable (`yes` → 1, `no` → 0)\
    -   Checked and handled missing values
2.  **Exploratory Data Analysis (EDA)**
    -   Visualized target class imbalance\
    -   Plotted distributions of key features (`age`, `balance`, etc.)
3.  **Model Building**
    -   Applied **Logistic Regression**\
    -   Applied **Random Forest Classifier**\
    -   Handled imbalance using **SMOTE**
4.  **Model Evaluation**
    -   Confusion Matrix\
    -   Precision, Recall, F1-score\
    -   ROC AUC
5.  **Explainability (XAI)**
    -   Used **SHAP** to explain predictions\
    -   Visualized feature importance

------------------------------------------------------------------------

## 📊 Results

  ---------------------------------------------------------------------------------
  Model             Accuracy   Precision      Recall       F1-Score      ROC AUC
                               (Class 1)      (Class 1)    (Class 1)     
  ----------------- ---------- -------------- ------------ ------------- ----------
  **Random Forest** 90%        0.55           0.64         **0.59**      **0.92**

  **Logistic        86%        0.43           0.73         0.54          0.88
  Regression**                                                           
  ---------------------------------------------------------------------------------

✅ **Random Forest performed better overall**, especially in recall and
ROC AUC.

------------------------------------------------------------------------

## 📈 Visualizations

-   Class distribution plots\
-   ROC curves\
-   SHAP summary and waterfall plots

------------------------------------------------------------------------

## 🧠 Skills Gained

-   **Classification modeling** → Logistic Regression, Random Forest\
-   **Feature encoding** → One-Hot Encoding, handling categorical
    variables\
-   **Model interpretability (XAI)** → SHAP explanations\
-   **Customer behavior analysis** → Identifying key factors influencing
    term deposit subscription

------------------------------------------------------------------------

## 🔍 Conclusion

-   Random Forest is a stronger model compared to Logistic Regression
    for this dataset.\
-   SHAP revealed that **balance** and **age** are highly influential
    features.\
-   Model can help banks **target the right customers** more effectively
    in future campaigns.

------------------------------------------------------------------------

✍️ **Author:** Your Name
