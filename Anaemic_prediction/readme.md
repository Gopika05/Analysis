#  Anemia Detection Using Color Pixel Data and Hemoglobin Levels

This project focuses on detecting anemia in individuals using a combination of image-based color pixel data and hemoglobin (Hb) concentration. It explores how RGB percentages and gender can be used in predicting whether a person is anaemic.

---

#  Dataset Overview

- **Rows**: 100+ patient records
- **Columns**:
  - `Sex`: Gender of the individual (M/F)
  - `%Red Pixel`, `%Green Pixel`, `%Blue Pixel`: Color composition extracted from medical image (possibly conjunctiva or tongue)
  - `Hb`: Hemoglobin concentration in g/dL
  - `Anaemic`: Target variable (Yes/No)

---

# Objective

To build a classification model that predicts **anemia status** (`Yes` or `No`) using hemoglobin levels and pixel color information derived from medical images.

---

# Workflow

# 1. Data Cleaning & Preprocessing
- Verified data types and null values
- Encoded categorical variables (`Sex`, `Anaemic`)
- Feature scaling using `StandardScaler`

# 2. Exploratory Data Analysis (EDA)
- Distribution plots of Hemoglobin and color channels
- Box plots to compare RGB values by anemia status
- Correlation heatmap

# 3. Model Building
- Logistic Regression
- Decision Tree Classifier

# 4. Evaluation Metrics
- Accuracy
- Classification Report
- Confusion Matrix
- ROC-AUC Score

---

## 📊 Results

| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | 86%     |
| Decision Tree       | 85.7%     |
| **Logistic Regression**   | **86%** ✅ (Best performer)

> Feature importance shows **Hemoglobin** and **Red Pixel %** are the most predictive features.

---

## 🔬 Feature Importance (Top Predictors)

- Hemoglobin (`Hb`)
- % Red Pixel
- % Blue Pixel
- Sex

---

## 📦 Tech Stack

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Jupyter Notebook / VS Code

---

