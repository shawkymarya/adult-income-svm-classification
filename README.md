# 🧠 Adult Income Classification using SVM

## 📌 Overview

This project predicts whether an individual's annual income exceeds $50K using Support Vector Machine (SVM).

The focus of this project is not only accuracy, but also:
- Handling class imbalance
- Outlier treatment
- Threshold optimization
- Real-world evaluation metrics

---

## 📊 Dataset

Adult Income Dataset (UCI)

Target:
- 0 → <=50K
- 1 → >50K

---

## ⚙️ Preprocessing

### Data Cleaning
- Removed redundant `education` column
- Replaced '?' with NaN
- Dropped missing values

### Outlier Handling
Applied IQR clipping to reduce the impact of extreme values.

### Encoding
Applied One-Hot Encoding to nominal categorical features.

### Class Imbalance
SMOTE was applied on training data only.

---

## 🧠 Model

SVC (RBF Kernel)

- Kernel: RBF
- C = 10
- probability = True
- Threshold optimized to 0.35

---

## 📈 Results

- ROC-AUC ≈ 0.88–0.89
- Improved recall for high-income class
- Balanced precision-recall trade-off

---

## 📊 Visualizations

- ROC Curve
- Confusion Matrix
- Precision-Recall Curve

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
- Matplotlib
- Seaborn

---

> Machine learning is not just about training models —  
> it's about understanding data, imbalance, and decision impact.
