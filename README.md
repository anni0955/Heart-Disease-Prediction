# ❤️ Heart Disease Prediction using Machine Learning

🚀 EDA | Feature Scaling | Logistic Regression | KNN | Decision Tree

<p align="center"> <img src="https://img.shields.io/badge/Machine%20Learning-ScikitLearn-blue?style=for-the-badge"> <img src="https://img.shields.io/badge/Model-Classification-green?style=for-the-badge"> <img src="https://img.shields.io/badge/Dataset-Heart%20Disease-red?style=for-the-badge"> <img src="https://img.shields.io/badge/Accuracy-~88%25-orange?style=for-the-badge"> </p>

## 📌 Project Overview

This project predicts whether a patient has Heart Disease based on medical and physiological features using Machine Learning. The notebook includes:

    ✔ Exploratory Data Analysis (EDA)
    ✔ Feature Scaling
    ✔ Multiple ML Models
    ✔ Model Evaluation (Accuracy + Cross-Validation)
    ✔ Distribution, Density & Relationship Plots

## 🩺 Target Variable

    condition
    
    1 → Heart Disease Present
    
    0 → No Heart Disease

## 📦 Dataset Details

### 📂 Dataset: Heart Disease (Cleveland)  
    Rows: 297  
    Columns: 14  
    Features include:  
    - age  
    - sex  
    - cp (chest pain)  
    - trestbps  
    - chol  
    - fbs  
    - restecg  
    - thalach  
    - exang  
    - oldpeak  
    - slope  
    - ca  
    - thal  
    - condition (target)


Loaded using Pandas:

df = pd.read_csv('heart_cleveland_upload.csv')

## 📊 Exploratory Data Analysis

### Included EDA Visualizations:

    ✔ Scatter Plots (age vs chol, colored by condition & fbs)  
    ✔ Pairplot to understand feature relationships  
    ✔ KDE Plots (before scaling)  
    ✔ Density Plots (after Standard Scaling)  
    ✔ Countplots (condition distribution, condition vs sex)

## 🧠 Modeling Approach

Three ML models were trained:

### 1️⃣ Logistic Regression

    Accuracy: 0.88
    
    Cross-validation scores:
    Example → [0.83, 0.87, 0.80, 0.82, 0.76]

### 2️⃣ K-Nearest Neighbors (KNN)

    n_neighbors = 5
    
    Accuracy: 0.88
    
    Cross-validation scores show stable results.

### 3️⃣ Decision Tree Classifier

    Criterion: "gini"
    
    Accuracy: 0.73

## 🧠 Model Performance Summary

| Model                 | Accuracy | Notes |
|----------------------|----------|-------|
| Logistic Regression  | **0.88** | Best performing model |
| KNN (K=5)            | **0.88** | Performs similar to LR |
| Decision Tree        | 0.73     | Underfits compared to others |

Cross-validation scores confirm stability of Logistic Regression & KNN.

## ⚙️ Feature Scaling

    StandardScaler applied to all numerical columns:
    
    - age  
    - trestbps  
    - chol  
    - thalach  
    
    Benefits:
    ✔ Normalized density curves  
    ✔ Improved model stability  
    ✔ Better KNN performance  

## 🧭 Project Structure

    📁 heart-disease-prediction  
    │── 📓 Heart Disease Prediction.ipynb.ipynb  
    │── 📄 README.md          
    │── 📄 heart_cleveland_upload.csv
