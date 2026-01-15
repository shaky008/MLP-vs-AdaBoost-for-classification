# 🎓 Predicting Student Dropout and Academic Success  
**Machine Learning Final Project**  
**Author:** Utsav Shakya  

---

## 📌 Project Overview
This project applies **machine learning techniques** to predict student outcomes — **Dropout**, **Enrolled**, or **Graduate** — using real educational data from the **UCI Machine Learning Repository**.

The goal is to:
- Analyze student performance and socioeconomic factors
- Reduce dimensionality using **PCA**
- Train and compare multiple classification models
- Identify the most effective approach for early risk detection

---

## 🧠 Techniques Used
✔ Data discovery & preprocessing  
✔ Principal Component Analysis (PCA)  
✔ Decision Tree analysis  
✔ Multi-Layer Perceptron (MLP)  
✔ Ensemble methods (AdaBoost & Gradient Boosting)  
✔ Model evaluation with **Macro-F1** and **Stratified Cross-Validation**

---

## 📊 Dataset Information

| Attribute | Description |
|--------|------------|
| **Source** | [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success) |
| **Dataset Name** | Predict Students’ Dropout and Academic Success |
| **Rows** | 4,424 |
| **Features** | 36 (academic, demographic, socioeconomic) |
| **Missing Values** | None |

### 🎯 Target Classes
- **Dropout**
- **Enrolled**
- **Graduate**

---

## 🔍 Exploratory Data Analysis (EDA)

**Key insights discovered:**
- 📈 Academic performance (1st & 2nd semester grades) had the **strongest correlation** with student outcomes.
- 💰 Macroeconomic indicators (GDP, inflation) showed **very weak influence**.
- 🌳 A shallow decision tree revealed:
  - **2nd semester grades**
  - **Tuition fee status**  
  as major predictors of dropout risk.
- 📉 PCA required **27 components to retain 96% variance**, indicating a **high-dimensional dataset**.

---

## 🧪 Models & Performance

### 🔹 Models Evaluated
- **MLP Neural Network**
- **AdaBoost**
- **Gradient Boosting**

### 📈 Performance Comparison (Macro-F1)

| Model | Configuration | Macro-F1 |
|----|----|----|
| MLP | PCA-Reduced Features | 0.63 |
| MLP | Scaled Features (No PCA) | 0.64 |
| AdaBoost | Full Dataset (No Scaling) | 0.65 |
| **Gradient Boosting** ⭐ | Scaled Dataset | **0.68** |

---

## 🏆 Why Gradient Boosting Won
- 🌲 Tree-based ensembles handled **mixed feature types** effectively
- 🔁 Boosting captured **non-linear relationships**
- 🤖 MLP struggled especially with the **Enrolled** class
- ❌ PCA did not significantly improve neural network performance

> **Result:** Gradient Boosting outperformed MLP and AdaBoost, disproving the initial hypothesis that *MLP + PCA* would be the best model.

---

## 🚀 Practical Applications
This system can be used as an **early-warning tool** by educational institutions to:
- Identify at-risk students early
- Provide targeted academic support
- Offer counseling or financial assistance
- Improve retention and graduation rates

---

## 🛠️ How to Run the Project

```bash
# 1. Download Data from UCI Machine Learning Repository

# 2. Launch Jupyter Notebook
```

## 📘 Full Report
Detailed explanation with visualization and results are avaiable in the [📄Full Report](ML_FINAL_REPORT_T00693024.pdf)
