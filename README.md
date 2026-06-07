# 🩺 Diabetes Prediction using Logistic Regression

A machine learning project that predicts whether a patient is likely to have diabetes based on medical diagnostic data. Built using Python and scikit-learn.

---

## 📌 Project Overview

This project uses the **Pima Indians Diabetes Dataset** to train a Logistic Regression model that classifies patients as diabetic or non-diabetic. The pipeline covers everything from data cleaning to model evaluation.

**Goal:** Early prediction of diabetes to support clinical decision-making.

---

## 📊 Dataset

- **Source:** [Pima Indians Diabetes Database – Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Size:** 768 samples, 8 features
- **Target:** `Outcome` — 0 (No Diabetes), 1 (Diabetes)

| Feature | Description |
|---|---|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness (mm) |
| Insulin | 2-Hour serum insulin |
| BMI | Body mass index |
| DiabetesPedigreeFunction | Diabetes hereditary score |
| Age | Age in years |

---

## 🛠️ Tech Stack

- Python 3.x
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## 🔍 Project Pipeline

```
Load Data → Clean Zeros → EDA → Train/Test Split → Scale Features → Train Model → Evaluate
```

Key decisions made in this project:
- **Zero values** in medical columns (Glucose, BMI, etc.) treated as missing and replaced with column medians
- **Train/test split before scaling** to prevent data leakage
- `class_weight='balanced'` used to handle the 65/35 class imbalance
- **5-fold cross-validation** for reliable accuracy estimates

---

## 📈 Results

| Metric | Score |
|---|---|
| Accuracy | ~78% |
| ROC-AUC | ~0.84 |
| Cross-Val Mean | ~77% (±2%) |

> Results may vary slightly due to random state and dataset version.

---

## 📁 Repository Structure

```
diabetes-prediction-ml/
│
├── diabetes_logistic_regression.py   # Main ML pipeline
├── diabetes.csv                      # Dataset
├── README.md                         # Project documentation
│
└── outputs/                          # Generated plots (optional)
    ├── feature_distributions.png
    ├── correlation_heatmap.png
    ├── evaluation_plots.png
    └── feature_importance.png
```

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/Rubasri-R/diabetes-prediction-ml.git
   cd diabetes-prediction-ml
   ```

2. **Install dependencies**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

3. **Run the script**
   ```bash
   python diabetes_logistic_regression.py
   ```

---

## 📸 Sample Output

> *(Add a screenshot of your confusion matrix or ROC curve here once you run the code!)*

---

## 🌱 Future Improvements

- [ ] Try other models — Random Forest, XGBoost
- [ ] Build a web app with Streamlit for live predictions
- [ ] Add Jupyter Notebook version for better visualization
- [ ] Hyperparameter tuning with GridSearchCV

---

## 👩‍💻 Author

**Rubasri R**
- GitHub: [@Rubasri-R](https://github.com/Rubasri-R)

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
