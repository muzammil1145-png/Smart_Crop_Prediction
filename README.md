# Smart Crop Yield Prediction — Machine Learning Regression

**Python · Pandas · Scikit-learn · Regression · Model Evaluation**

This project builds and compares regression models to predict crop yield from structured agricultural data. The focus is on clean preprocessing, reproducible model comparison, diagnostic evaluation, and communicating why a simpler model can sometimes outperform more complex algorithms.

---

## Executive Summary

I developed a complete regression workflow using agricultural features such as irrigation, previous crop, and other structured predictors. The analysis compared Linear Regression, Random Forest, and Gradient Boosting models, followed by tuning and diagnostic evaluation.

The strongest result came from **Linear Regression**, which achieved the best test-set performance among the compared models. This project demonstrates model selection based on evidence rather than model complexity.

### Model Results

| Model | MAPE | MSE | R² |
| --- | ---: | ---: | ---: |
| Linear Regression | **3.99%** | **25.81** | **0.9821** |
| Random Forest | 4.22% | 29.02 | 0.9799 |
| Gradient Boosting | 4.09% | 27.05 | 0.9813 |

---

## Analytical Workflow

```text
Crop Yield Dataset
       │
       ▼
Data Cleaning & Validation
       │
       ▼
Feature Engineering
       │
       ▼
Train / Test Split
       │
       ▼
Model Comparison
• Linear Regression
• Random Forest
• Gradient Boosting
       │
       ▼
Hyperparameter Tuning
       │
       ▼
Diagnostics & Interpretation
```

---

## Key Steps

### Data Preparation
- Cleaned and validated structured agricultural data.
- Encoded categorical features for modeling.
- Created reproducible train/test splits.
- Reviewed feature distributions and relationships before model training.

### Model Development
- Built a Linear Regression baseline.
- Compared tree-based Random Forest and Gradient Boosting regressors.
- Tuned ensemble models using structured parameter grids.
- Evaluated models using MAPE, MSE, and R².

### Model Diagnostics
- Reviewed residual behavior.
- Compared predicted versus actual outcomes.
- Interpreted Linear Regression coefficients for feature influence.

---

## Key Takeaway

The main lesson from this project is that **more complex does not automatically mean better**. Although Random Forest and Gradient Boosting were strong performers, Linear Regression generalized best on the test set.

That result reinforced the importance of:

- establishing a baseline;
- comparing multiple models;
- using test-set metrics rather than intuition;
- checking residuals and prediction quality;
- preferring the simplest model that performs well.

---

## Visual Analysis

The repository includes exported exploratory and model-diagnostic visuals such as:

- histograms;
- bar plots;
- count plots;
- correlation heatmap;
- predicted vs. actual results.

These visuals support both exploratory analysis and model interpretation.

---

## Technologies & Skills

- Python
- Pandas
- Scikit-learn
- Regression modeling
- Feature engineering
- Hyperparameter tuning
- Model evaluation
- Residual analysis
- Data visualization
- Statistical interpretation

---

## Repository Structure

```text
Smart_Crop_Prediction/
├── Smart Crop Prediction.ipynb
├── crop_yield_dataset.csv
├── Barplot.png
├── Counplots.png
├── Heatmap.png
├── Histograms.png
├── Predicted vs Actual.png
├── dataset-cover.png
└── README.md
```

---

## What This Project Demonstrates

This project demonstrates a practical machine-learning workflow from raw structured data through model evaluation and interpretation:

**Data → Features → Models → Evaluation → Diagnostics → Insight**

It is especially relevant as supporting evidence for Data Analyst and entry-level Data Science roles because it shows Python modeling skills alongside the BI and SQL work in my broader portfolio.
