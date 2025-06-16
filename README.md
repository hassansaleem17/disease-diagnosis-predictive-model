# 🩺 Disease Diagnosis Predictive Model

This project builds a medical diagnosis model using the PIMA Diabetes Dataset to predict the likelihood of diabetes in patients. It uses supervised machine learning techniques such as Gradient Boosting, SVM, and Neural Networks. The notebook includes EDA, feature selection, model training, and healthcare insights.

---

## 📂 Dataset

- **Source**: [PIMA Indian Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Format**: CSV
- **Target Variable**: `Outcome` (0 = Non-diabetic, 1 = Diabetic)

---

## 🧠 Objective

To create a reliable disease prediction model and extract healthcare insights using clinical data such as glucose levels, BMI, insulin, pregnancies, and more.

---

## 🔍 Exploratory Data Analysis (EDA)

- Dataset structure, types, and null/missing values.
- Distribution of diabetic vs non-diabetic patients.
- Correlation heatmap to visualize relationships.
- Identification of unrealistic zero values in medical attributes.

---

## 🧰 Preprocessing & Feature Engineering

- Replace zeros in key columns (`Glucose`, `BloodPressure`, etc.) with `NaN`, then impute with mean.
- Scale features using `StandardScaler`.
- Use `SelectKBest` with ANOVA F-test to keep most predictive features.

---

## 🤖 Model Training

- **Gradient Boosting Classifier**
- **Support Vector Machine (SVM)**
- **Multilayer Perceptron (Neural Network)**

Models are trained using a stratified train-test split for unbiased evaluation.

---

## 📈 Evaluation Metrics

- **F1 Score**: For balanced performance on precision and recall.
- **AUC-ROC Curve**: To evaluate classifier quality across thresholds.
- **ROC Curves**: Plotted for all models for visual comparison.

---

## ✅ Insights for Healthcare Professionals

- High glucose and BMI values are strong indicators of diabetes.
- Age and insulin also contribute significantly to prediction.
- Early detection can benefit through routine screening and intervention.

---

## 📦 Installation & Usage

```bash
git clone https://github.com/yourusername/disease-diagnosis-predictive-model.git
cd disease-diagnosis-predictive-model
pip install -r requirements.txt
jupyter notebook disease_diagnosis_prediction.ipynb
