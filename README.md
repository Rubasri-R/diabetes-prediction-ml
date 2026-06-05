# diabetes-prediction-ml
Machine learning project for diabetes prediction
# 🩺 Diabetes Prediction Using Machine Learning

## 📌 Project Overview
This project focuses on predicting whether a person is diabetic or not using medical diagnostic data. It applies data analysis and machine learning techniques to identify key health factors influencing diabetes.

---

## 🎯 Objective
To build a machine learning model that can classify patients as diabetic or non-diabetic based on health parameters such as glucose level, BMI, age, and other medical attributes.

---

## 📊 Dataset Information
- Source: Pima Indians Diabetes Dataset
- Total Records: 768
- Features: 8 input variables
- Target Variable: Outcome (0 = No Diabetes, 1 = Diabetes)

---

## 🧠 Machine Learning Workflow

### 1. Data Exploration
- Checked dataset structure
- Analyzed missing values and distributions
- Studied class balance

### 2. Data Visualization
- Outcome distribution chart
- Correlation heatmap
- Feature relationship analysis

### 3. Data Preprocessing
- Feature scaling using StandardScaler
- Train-test split (80/20)

### 4. Model Building
- Logistic Regression (primary model)
- Random Forest (comparison model)

### 5. Model Evaluation
- Accuracy Score
- Confusion Matrix
- Precision, Recall, F1-score

---

## 📈 Results

- Best Model: Logistic Regression
- Accuracy: ~75%
- Key Findings:
  - Glucose is the strongest predictor of diabetes
  - BMI and Age also contribute significantly
  - Model performs better on non-diabetic cases

---

## ⚠️ Key Insights
- High glucose levels strongly indicate diabetes risk
- Some diabetic cases are harder to detect (false negatives exist)
- Model can be improved with advanced tuning or ensemble methods

---

## 🛠️ Technologies Used
- Python 🐍
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🚀 Future Improvements
- Hyperparameter tuning
- Try advanced models (XGBoost, SVM)
- Deploy using Streamlit web app
- Improve recall for diabetic cases

---

## 👩‍💻 Author
Created as a beginner-friendly Machine Learning project for learning and academic purposes.

---

## ⭐ If you like this project
Give it a star ⭐ on GitHub!
