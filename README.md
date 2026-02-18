# 🌲 Forest Cover Type Classification

<p align="center">
  <b>Multi-Class Forest Cover Prediction using Cartographic and Environmental Features</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Accuracy-95%25-brightgreen" />
  <img src="https://img.shields.io/badge/Model-Random%20Forest-blue" />
  <img src="https://img.shields.io/badge/Problem-Multi--Class%20Classification-orange" />
  <img src="https://img.shields.io/badge/Dataset-UCI%20Covertype-lightgrey" />
  <img src="https://img.shields.io/badge/Python-3.x-yellow" />
</p>

---

## 📌 Project Overview

This project predicts the **type of forest cover** for a 30m × 30m land patch using cartographic and environmental features from the UCI Covertype dataset.

The model achieves **95% accuracy** using ensemble learning techniques.

---

## 🎯 Problem Statement

Given environmental and geographical attributes such as:

- Elevation  
- Slope  
- Aspect  
- Soil Type  
- Wilderness Area  
- Distance to Hydrology  
- Distance to Roadways  

Predict which of the **7 forest cover types** exists in that region.

This is a **multi-class classification problem**.

---

## 📊 Dataset Information

- **Source:** UCI Machine Learning Repository  
- **Total Samples:** 581,012  
- **Total Features:** 54  
- **Target Variable:** `Cover_Type`  
- **Classes:** 7  

Each row represents one geographic land unit.

### Feature Categories

### 1️⃣ Topographic Features
- Elevation  
- Aspect  
- Slope  
- Hillshade (9am, Noon, 3pm)  
- Horizontal & Vertical Distance to Hydrology  
- Horizontal Distance to Roadways  
- Horizontal Distance to Fire Points  

### 2️⃣ Wilderness Area
4 one-hot encoded binary columns

### 3️⃣ Soil Type
40 one-hot encoded binary columns

---

## 🔍 Exploratory Data Analysis (EDA)

The following analysis was performed:

- Target distribution analysis  
- Elevation vs Cover Type comparison  
- Correlation heatmap  
- Feature importance ranking  
- Confusion matrix evaluation  

### 🔎 Key Insights

- Elevation is the most influential feature  
- Soil type strongly affects forest classification  
- Moderate class imbalance exists  
- Hydrology distance features show correlation  

---

## 🤖 Model Development

### Algorithms Used

- Random Forest Classifier  

### Data Splitting

- 80% Training  
- 20% Testing  
- Stratified split  

### Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Cross-Validation  

---

## 📈 Results

| Metric | Score |
|--------|--------|
| Test Accuracy | **95%** |
| Cross-Validation Accuracy | ~94–95% |
| Classes | 7 |

The model demonstrates strong generalization and stable performance across folds.

---

## 📊 Model Evaluation

- Confusion Matrix Analysis  
- Per-Class Precision & Recall  
- Feature Importance Visualization  

### 🔝 Top Influential Features

- Elevation  
- Horizontal Distance to Roadways  
- Soil Type indicators  
- Hillshade at Noon  

---

## 🛠 Tech Stack

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn  

---

## 📂 Project Structure

```
forest-cover-type-classification/
│
├── notebooks/
│   └── model.ipynb
│
├── requirements.txt
└── README.md
```

---

## 🚀 Installation & Usage

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/forest-cover-type-classification.git
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run Notebook

Open `model.ipynb` and execute cells.

---

## 📌 Why This Project Matters

- Demonstrates large-scale dataset handling (581k rows)  
- Applies multi-class classification  
- Shows feature importance interpretation  
- Uses ensemble learning for strong predictive performance  

---

## 🔮 Future Improvements

- Hyperparameter tuning  
- SHAP explainability  
- Deployment using Streamlit  
- Feature reduction experiments  
- Model comparison with XGBoost and LightGBM  

---

## 👨‍💻 Author

**Your Name**

Data Science | Machine Learning | AI Projects

---

## ⭐ If You Found This Useful

Give this repository a star.
