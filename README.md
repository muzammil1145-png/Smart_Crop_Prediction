# Smart_Crop_Prediction
# 🌾 Smart Crop Prediction – End-to-End Regression Modeling Project

This project builds a complete machine learning workflow to predict crop yield using structured agricultural data. The goal is to create a clean, reliable, and interpretable regression pipeline that can support smarter farming decisions.

## 🚀 Project Highlights

### 🧹 Data Preparation & Feature Engineering
- Cleaned and validated the dataset
- Engineered dummy variables for categorical features (irrigation, previous crop, etc.)
- Ensured reproducible train/test splits
- Validated feature distributions and relationships

### 🤖 Baseline Model Development
Implemented and compared:
- Linear Regression
- Random Forest
- Gradient Boosting

### 📈 Baseline Results (Test Set)
- **Linear Regression**
  - MAPE: 3.99%
  - MSE: 25.81
  - R²: 0.9821

- **Random Forest (Baseline)**
  - MAPE: 4.22%
  - MSE: 29.02
  - R²: 0.9799

- **Gradient Boosting (Baseline)**
  - MAPE: 4.09%
  - MSE: 27.05
  - R²: 0.9813

### ⚙️ Hyperparameter Tuning
- Tuned Random Forest and Gradient Boosting using structured parameter grids
- Compared tuned models against baselines to understand the bias–variance tradeoff
- Found that Linear Regression remained the strongest generalizer for this dataset

### 📊 Model Diagnostics & Interpretability
- Residual plots for bias/variance analysis
- Predicted vs Actual plots for generalization assessment
- Linear Regression coefficient-based feature importance

## 📁 Repository Structure
smart-crop-prediction/
│
├── README.md
├── requirements.txt
├── data/
│   └── your_dataset.csv
│
├── notebooks/
│   └── smart_crop_prediction.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── modeling.py
│   ├── evaluation.py
│   └── visualization.py
│
└── images/
    ├── residual_plot.png
    ├── predicted_vs_actual.png
    └── feature_importance.png
