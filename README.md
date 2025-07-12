# NaturalGasPrediction
PredictionDescription
# 🇺🇸 Natural Gas Consumption Forecasting Using ANFIS (MATLAB)

This project presents a fuzzy logic-based approach to forecasting **daily national natural gas consumption** using an **Adaptive Neuro-Fuzzy Inference System (ANFIS)** in MATLAB.

> 🚫 The dataset used in this study is private and **cannot be shared** due to confidentiality agreements. However, all modeling procedures, evaluation methods, and results are shared.

---

## 📊 Project Overview

- **Platform:** MATLAB
- **Model:** ANFIS (Adaptive Neuro-Fuzzy Inference System)
- **Input Features:**
  1. Holiday (binary)
  2. Month (1–12)
  3. Season (1–4)
  4. Gas consumption (2 days ago)
  5. Gas consumption (1 day ago)
- **Output:** Today's gas consumption

> ✅ All features and output were **normalized** before training.

---

## 🧠 Modeling Summary

- **Membership Functions Tested:** `trimf`, `trapmf`, `gbellmf`, `gaussmf`, `primf`
- **Best Configuration:** `trimf (3-3-3-3-3)`
- **Optimization Method:** Hybrid (Backpropagation + Least Squares)
- **Epochs:** 10

---

## ✅ Results

### 🔹 Best Model – Trimf 3-3-3-3-3
- **R²:** 0.8296  
- **RMSE:** 0.0781  
- **MAE:** 0.0545  
- **Rules Generated:** 243

![Linear Regression](Trimf3-3-33.png)
![Actual vs Predicted](figures/actual_vs_predicted_trimf.png)

### 🔹 Performance Comparison Table

![Performance Table](figures/performance_table.png)

---

## 📁 Contents

- `src/`: MATLAB code for training and testing the ANFIS model
- `results/`: Saved `.fis` models
- `figures/`: Plots and performance results

---

)
