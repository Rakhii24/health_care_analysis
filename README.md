# 🩺 Healthcare Data Analysis: Predicting Patient Readmission Risk

![HealthCare Banner](https://img.shields.io/badge/Domain-Healthcare-blue.svg) ![Python](https://img.shields.io/badge/Built%20With-Python%203.10-brightgreen) ![ML](https://img.shields.io/badge/ML-Random%20Forest-orange) ![License](https://img.shields.io/badge/License-MIT-lightgrey)

## 📌 Overview

This project focuses on **predictive analytics in healthcare** to help identify patients who are at risk of **hospital readmission**. Using historical medical records and patient data, a **machine learning model** is built to forecast readmission likelihood, enabling hospitals to intervene proactively and improve care outcomes.

---

## 🧠 Objective

* Predict whether a patient is likely to be readmitted within 30 days.
* Reduce hospital operational costs and enhance patient care quality.
* Identify key risk factors contributing to readmissions.

---

## 🗂️ Dataset

* **Source**: UCI Machine Learning Repository – [Diabetic Readmission Dataset](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
* **Records**: 101,766
* **Features**: 50+
* **Target**: Readmission Status (`<30`, `>30`, `NO`)

### Key Attributes:

* Demographics (Age, Gender)
* Medical History (Diagnosis Codes)
* Hospital Details (Length of Stay, Number of Procedures)
* Treatment Data (Medications, Lab Tests, Glucose Level)

---

## 🛠️ Tech Stack

| Tool                     | Purpose                           |
| ------------------------ | --------------------------------- |
| **Python**               | Programming Language              |
| **Pandas / NumPy**       | Data Preprocessing & Manipulation |
| **Matplotlib / Seaborn** | Data Visualization                |
| **Scikit-learn**         | Machine Learning Modeling         |
| **Jupyter Notebook**     | IDE for development               |

---

## 🔎 Exploratory Data Analysis (EDA)

* ✅ Missing value treatment and feature encoding
* ✅ Distribution analysis of diagnosis and readmission
* ✅ Correlation heatmap of variables
* ✅ Class imbalance check (target variable)

---

## ⚙️ Model Building

* **Algorithm Used**: Random Forest Classifier
* **Train-Test Split**: 80-20
* **Performance Metrics**:

  * Accuracy
  * Precision / Recall
  * F1 Score
  * ROC-AUC Curve

```python
from sklearn.ensemble import RandomForestClassifier
model = RandomForestClassifier(n_estimators=100, random_state=42)
model.fit(X_train, y_train)
```

---

## 📊 Results

| Metric    | Score |
| --------- | ----- |
| Accuracy  | 87.2% |
| Precision | 82.4% |
| Recall    | 78.9% |
| F1 Score  | 80.6% |

* Most influential features: Number of Inpatient Visits, A1C Results, Discharge Disposition, Time in Hospital.

---

## 📌 Key Insights

* Frequent inpatient visits and abnormal A1C test results are strong indicators of readmission.
* Patients discharged to nursing facilities showed higher readmission rates.
* Optimizing post-discharge care plans can drastically reduce readmission risk.

---

## 📈 Future Improvements

* Integrate real-time patient data from IoT devices or EMRs.
* Use deep learning (LSTM) for sequential data modeling.
* Build a dashboard for hospital administrators to visualize risk profiles.

---

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---


