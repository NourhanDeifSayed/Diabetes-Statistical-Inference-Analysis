# 🩺 Diabetes Statistical Inference Analysis 

This repository presents an in-depth statistical analysis of a diabetes dataset using **R**. The objective is to explore and identify key health indicators that contribute to the onset of diabetes, using inferential statistics and visual data exploration.

## 📊 Project Overview

This analysis was performed on a public dataset containing medical records of female patients. The dataset includes features such as glucose concentration, BMI, insulin levels, age, and pregnancy count, among others. The aim is to assess the relationship between these features and the likelihood of developing diabetes.

Key objectives:
- Identify statistically significant features affecting diabetes.
- Explore distributions and trends via data visualization.
- Use hypothesis testing and confidence intervals to support conclusions.
- Derive risk profiles using clustering techniques.

---

## 📁 Dataset

- **Source**: [Kaggle - Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Samples**: 768
- **Features**: 8 health-related attributes + binary `Outcome` (1: diabetic, 0: non-diabetic)

### Main Attributes
- `Pregnancies`
- `Glucose`
- `BloodPressure`
- `SkinThickness`
- `Insulin`
- `BMI`
- `DiabetesPedigreeFunction`
- `Age`
- `Outcome`

---

## ⚙️ Methods Applied

### ✅ Data Preprocessing
- Checked for **missing** and **duplicate** values.
- Replaced **invalid zeros** using:
  - **Mean** for normally distributed columns (e.g., Glucose, BMI)
  - **Median** for skewed columns (e.g., Insulin, SkinThickness)
- Outlier identification using visual thresholds.

### 📈 Exploratory Analysis
- Distribution plots for key attributes
- Pairwise scatter plots and correlation matrix
- Stratified visualizations by diabetes outcome

### 📊 Statistical Inference
- **Confidence Intervals**: Estimated means across different sample sizes.
- **Hypothesis Testing**:
  - Glucose levels differ significantly between diabetic and non-diabetic patients.
  - BMI also shows significant differences.
- **Correlation Analysis** between:
  - Glucose & BMI
  - Insulin & Blood Pressure
  - Glucose & Age

### 🧪 Clustering Analysis
- K-means clustering to identify risk profiles based on Glucose and BMI.

---

## 📌 Key Insights

- Diabetic patients show higher mean glucose and BMI levels.
- Age and number of pregnancies have weak but noticeable influence.
- Family history (Diabetes Pedigree Function) has minor correlation with glucose.
- Glucose and BMI can help define three clear risk groups.
- Confidence intervals shrink with increasing sample size, enhancing statistical reliability.

--
