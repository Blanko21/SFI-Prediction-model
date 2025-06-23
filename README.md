# 🧠 Student Fatigue Index (SFI) Prediction Model

A Machine Learning project designed to predict student fatigue levels based on survey data. The model helps educators, counselors, and students proactively identify signs of academic burnout and mental fatigue. Built using Python, cleaned using pandas, modeled using scikit-learn, and deployed with Streamlit.

---

## Project Overview

Student fatigue is a growing concern in academic environments. This project uses survey-based data to build a predictive model for identifying fatigue levels in students, helping institutions take early interventions. The results are made accessible through an interactive Streamlit dashboard.

---

##  Data Cleaning Process

The raw data collected through Google Forms and surveys included inconsistencies and null values. Key cleaning steps:

- **Missing Values**: Imputed using median/mode where applicable.
- **Categorical Encoding**: Converted Likert scale (e.g., "Often", "Sometimes") to numerical scores.
- **Outlier Detection**: Used IQR method to filter out extreme fatigue scores.
- **Normalization**: Applied Min-Max scaling to ensure consistency across features.

---

## Machine Learning

After preprocessing, the cleaned dataset was fed into several classification models to find the best fit.

### Models Tested:
- Logistic Regression  
- Random Forest  
- Decision Tree  
- SVM

### Final Model:
Random Forest (best accuracy and generalization)

- Accuracy: **85%**
- Precision/Recall: Evaluated using classification report
- Cross-Validation used for robustness

---

##  Streamlit Interface

The model is deployed using **Streamlit** to allow real-time fatigue prediction.

### Key Features:
- **User Input Form** for stress, sleep, workload, etc.
- **Real-time Predictions** on fatigue score
- **Recommendation Output**: Tips for fatigue management
