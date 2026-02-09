# SmartCare AI – Diabetes Risk Prediction & Preventive Analytics Platform

## 📌 Project Overview
SmartCare AI is an end-to-end machine learning project designed to predict diabetes risk using healthcare, lifestyle, and demographic data.  
The system analyzes patient health indicators such as BMI, glucose, blood pressure, insulin levels, cholesterol, sleep patterns, physical activity, diet type, stress level, and other behavioral factors to provide early detection and prevention insights.

This project follows an industry-style workflow including:
- Data validation and cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering and preprocessing
- Machine learning model building and evaluation
- Model comparison using ROC-AUC and confusion matrices
- Agile planning (Jira) and version control (GitHub)

---

## 🎯 Problem Statement
Diabetes is one of the fastest-growing chronic diseases worldwide. Many individuals remain undiagnosed until complications occur.  
Early prediction of diabetes risk can help healthcare providers and individuals take preventive actions such as lifestyle changes, diet control, and regular monitoring.

---

## 💡 Proposed AI Solution
This project uses supervised machine learning models to classify whether an individual is likely to have diabetes based on clinical and lifestyle features.  
The system helps in:
- Identifying high-risk individuals
- Supporting early preventive intervention
- Improving healthcare decision-making

---

## 👥 Target Users / Stakeholders
- Hospitals and healthcare providers
- Public health organizations
- Health insurance companies
- Patients and individuals at risk
- Researchers and healthcare analysts

---

## 📊 Dataset Information
- Dataset File: `Healthcare.csv`
- Total Rows: 18,000
- Total Columns: 30
- Domain: Healthcare / Lifestyle / Demographics

### Target Variable
- **Outcome**
  - `0` = No Diabetes
  - `1` = Diabetes

### Key Features
- Age, Gender, BMI
- Glucose, BloodPressure, Insulin, SkinThickness
- Cholesterol, Fasting_Blood_Sugar
- Diet_Type, Fast_Food_Intake
- PhysicalActivityLevel, Daily_Steps
- Sleep_Hours, Sleep_Quality
- Smoking_Status, Alcohol_Consumption
- Work_Stress_Level, Mental_Health_Status
- Country and Chronic Disease History

---

## 🛠 Tools & Technologies Used
- **Python**
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook
- GitHub (Version Control)
- Jira/Trello (Agile Project Management)

---

## 🔍 Exploratory Data Analysis (EDA)
EDA was performed to understand dataset distribution and identify important risk factors.

### EDA Includes:
- Missing value detection and imputation
- Outlier detection using boxplots
- Distribution analysis (histograms)
- Correlation heatmap
- Lifestyle feature impact analysis (steps, sleep, diet)
- Relationship analysis (BMI vs Glucose, Glucose vs Diabetes outcome)

---

## 🤖 Machine Learning Models Implemented
The following models were trained and evaluated:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

---

## 📈 Model Evaluation Metrics
Each model was evaluated using:
- Confusion Matrix
- Accuracy
- Precision
- Recall
- F1 Score
- ROC Curve
- ROC-AUC Score

The best-performing model was selected based on **ROC-AUC** and **F1 Score**, ensuring strong performance in diabetes detection.

---

## 📌 Project Workflow
1. Load and validate dataset
2. Handle missing values and outliers
3. Perform exploratory data analysis
4. Encode categorical features (OneHotEncoding)
5. Scale numeric features (StandardScaler)
6. Split data into train/test sets
7. Train multiple machine learning models
8. Evaluate models using confusion matrix and ROC curves
9. Compare models and select best model
10. Save trained model for future deployment (optional)

---

## 📂 Project Folder Structure
```bash
SmartCare-AI-Diabetes-Prediction/
│
├── data/
│   └── Healthcare.csv
│
├── notebooks/
│   ├── EDA_Diabetes.ipynb
│   └── ML_Model_Training.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── train_model.py
│   └── evaluate_model.py
│
├── images/
│   ├── correlation_heatmap.png
│   ├── confusion_matrix_rf.png
│   └── roc_curve.png
│
├── reports/
│   ├── Milestone1_Project_Overview.docx
│   └── Milestone2_Jira_UserStories.docx
│
├── requirements.txt
└── README.md
