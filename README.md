# Healthcare-Patient-Risk-Analysis
AIML project for patient risk prediction, anomaly detection, and AI doctor recommendations.
# 🏥 Healthcare Patient Risk Analysis – AIML Project

This project performs **Exploratory Data Analysis (EDA)**, **Supervised Learning**,  
**Unsupervised Anomaly Detection**, and an **LLM-based AI Doctor Recommendation**  
using a healthcare dataset. The goal is to understand patient risk patterns,  
predict test results, detect billing anomalies, and generate AI-powered  
personalized medical recommendations.

---

## 📌 Dataset
Source: https://www.kaggle.com/datasets/prasad22/healthcare-dataset

**Columns Included:**

- Name  
- Age  
- Gender  
- Blood Type  
- Medical Condition  
- Date of Admission  
- Doctor  
- Hospital  
- Insurance Provider  
- Billing Amount  
- Room Number  
- Admission Type  
- Discharge Date  
- Medication  
- Test Results  

---

# 📘 Project Tasks

This project is divided into **four major tasks**.

---

# 🧪 **Task 1 — Exploratory Data Analysis (EDA)**

### ✔ Performed:
- Distribution plots for:  
  - Age  
  - Billing Amount  
  - Room Number  
- Frequency analysis for:  
  - Medical Condition  
  - Admission Type  
  - Medication  
- Missing value checks  
- Outlier detection  
- Statistical summary  

### 📊 Key Insights:
- Age distribution is centered around mid-adult age.
- Billing Amount contains strong outliers (useful for anomaly detection).
- Some medical conditions and medications appear more frequently.
- Dataset has mixed categorical & numerical features requiring preprocessing.

---

# 🤖 **Task 2 — Supervised Learning (Predicting Test Results)**

### ✔ Steps Done:
- Preprocessing: Label encoding for categorical columns  
- Train-test split  
- Model training using:
  - Logistic Regression (for Positive/Negative prediction)  
  - Random Forest / Linear Regression (for numerical score prediction, optional)  
- Evaluation Metrics:
  - Accuracy  
  - Classification report  
  - Predicted vs Actual comparison  

### 🎯 Output:
A machine learning model capable of predicting a patient’s **Test Result**  
either as:
- **Categorical:** Positive / Negative  
- **Numerical:** Test score prediction  

---

# 🧩 **Task 3 — Unsupervised Learning (Anomaly Detection in Billing Amounts)**

### ✔ Steps Done:
1. Identified unusually **high/low billing amounts**  
2. Used **Isolation Forest** for anomaly detection  
3. Marked anomalies with:
4. Interpreted anomaly causes

### 📈 Interpretation:
- Most anomalies correspond to **very high billing amounts**  
→ Possible rare procedures, long hospital stays, or incorrect entries  
- Some anomalies have unusually low values  
→ Outpatient visits or incomplete records  

---

# 🧠 **Task 4 — AI Task (LLM-Based Doctor Recommendation)**

### ✔ Model Used:
**Google Gemini 2.0 Flash (API)**  
→ Provides ChatGPT-level natural language output

### ✔ Input Parameters:
- Age  
- Medical Condition  
- Medication  
- Predicted Test Result  

### ✔ Output:
A **doctor-style recommendation** with the following structure:

- **Clinical Summary**  
- **Doctor Recommendation**  
- **Medication Advice**  
- **Red-flag Warnings**  
- **Follow-up Instructions**

