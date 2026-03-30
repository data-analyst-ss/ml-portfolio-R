# 🎓 Harvard Data Science — Machine Learning Portfolio
### HarvardX Data Science Professional Certificate · Machine Learning in R

<div align="center">

![R](https://img.shields.io/badge/R-4.x-9A3F4A?style=for-the-badge&logo=r&logoColor=white)
![caret](https://img.shields.io/badge/caret-ML_Framework-BD6809?style=for-the-badge&logoColor=white)
![tidyverse](https://img.shields.io/badge/tidyverse-Data_Wrangling-9A3F4A?style=for-the-badge&logo=r&logoColor=white)
![ggplot2](https://img.shields.io/badge/ggplot2-Visualization-BD6809?style=for-the-badge&logoColor=white)

[![Live Portfolio](https://img.shields.io/badge/LIVE_PORTFOLIO-9A3F4A?style=for-the-badge&logo=github)](https://data-analyst-ss.github.io/ml-portfolio-R)

</div>

---

## Overview

End-to-end implementation of **12+ machine learning algorithms** on real-world datasets as part of the HarvardX Data Science Professional Certificate. Every model is documented with code, results, and visualizations — from exploratory data analysis to ensemble methods and regularization.

The portfolio covers the full ML lifecycle: data cleaning, feature engineering, model training, cross-validation, hyperparameter tuning, and performance evaluation. All work was done in R using industry-standard packages.

---

## Algorithms Implemented

| Category | Algorithm | Best Result |
|----------|-----------|-------------|
| **Classification** | K-Nearest Neighbors (KNN) | 97.4% accuracy — BRCA cancer diagnosis |
| **Classification** | Random Forest | 88.3% accuracy — Titanic survival |
| **Classification** | Logistic Regression | Baseline model for binary classification |
| **Classification** | Decision Trees | Interpretable rule-based classification |
| **Ensemble** | Model stacking | 96.5% accuracy — combining KNN + RF + GLM |
| **Dimensionality Reduction** | Principal Component Analysis (PCA) | Iris dataset — feature compression |
| **Dimensionality Reduction** | Singular Value Decomposition (SVD) | MovieLens — latent factor extraction |
| **Regularization** | Ridge / LASSO | Schools dataset — optimal alpha = 135 |
| **Inference** | Bayesian Inference | P(disease\|positive test) = 14.78% |
| **Validation** | Cross-Validation (k-fold) | Overfitting prevention across all models |

---

## Key Results

```
🎯 97.4%  — KNN accuracy on BRCA breast cancer diagnosis dataset
🎯 96.5%  — Ensemble model accuracy (Titanic survival prediction)
🎯 88.3%  — Random Forest accuracy (Titanic survival)
🎯  0.96  — KNN training accuracy on Iris (best feature: Petal.Width)
🎯  0.88  — KNN test accuracy on Iris dataset
🎯 14.78% — Posterior probability P(disease | positive test) via Bayes
🎯 135    — Optimal regularization alpha on schools dataset
```

---

## Case Studies

### 🩺 Cancer Diagnosis — BRCA Dataset
Applied KNN, Random Forest, LDA, and an ensemble model to predict malignant vs. benign breast tumours. The ensemble combining all three classifiers achieved **96.5% accuracy**, while KNN alone reached **97.4%** — outperforming the ensemble on this dataset, which highlights the importance of evaluating individual models rather than defaulting to ensemble methods.

```
Model        | Accuracy | Sensitivity | Specificity
-------------|----------|-------------|------------
KNN          | 97.4%    | High        | High
Random Forest| 95.1%    | Medium      | High
Ensemble     | 96.5%    | High        | High
```

### 🚢 Titanic Survival Prediction
Predicted passenger survival using demographic and ticket features. Random Forest achieved **88.3% accuracy**, capturing non-linear relationships between passenger class, sex, and age that linear models missed. The ensemble model reached **96.5%** by combining Random Forest, GLM, and KNN predictions.

```
Key predictors: Sex · Passenger Class · Age
Best model: Ensemble (96.5% accuracy)
```

### 🎬 MovieLens Recommendation System
Built a collaborative filtering system using SVD to decompose the user-item matrix into latent factors. The model captures patterns in movie preferences without requiring explicit feature engineering — the same approach used by Netflix and Spotify at scale.

### 🔬 Bayesian Inference — Disease Testing
Calculated the posterior probability of disease given a positive test result, accounting for base rate (prevalence) and test characteristics (sensitivity/specificity):

```
P(disease) = 0.02 (prevalence)
P(+ | disease) = 0.85 (sensitivity)
P(+ | healthy) = 0.10 (false positive rate)

Result: P(disease | positive test) = 14.78%
→ Risk multiplier vs. untested population: 7.39×
```

This demonstrates why a positive test is not a diagnosis — base rate matters enormously.

### 📊 Regularization — Schools Dataset
Applied Ridge and LASSO regression to predict student performance. The optimal regularization parameter alpha = 135 was found via cross-validation, preventing overfitting on the high-dimensional feature space.

### 🌸 Iris — KNN Feature Analysis
Evaluated all four Iris features individually to find the best predictor for species classification. **Petal.Width** was the single most predictive feature (training accuracy: 0.96, test accuracy: 0.88), outperforming sepal measurements.

---

## Tech Stack & Why R

| Package | Role |
|---------|------|
| **caret** | Unified ML framework — training, cross-validation, tuning |
| **randomForest** | Ensemble tree-based classification and regression |
| **ggplot2** | Publication-quality data visualizations |
| **tidyverse** | Data wrangling and pipeline construction |
| **dslabs** | Harvard course datasets (BRCA, Titanic, heights, etc.) |
| **e1071** | Support Vector Machines and Naive Bayes |

> **Why R for this portfolio?**
> The HarvardX curriculum is R-based, and R remains the language of choice for statistical inference, Bayesian modelling, and academic ML research. The `caret` package provides a consistent interface across 200+ ML algorithms — ideal for rapid experimentation and comparison. For production ML at scale, Python with scikit-learn is the complementary tool.

---

## How to Run Locally

**Requirements:** R 4.x · RStudio (recommended)

```r
# 1. Install required packages
install.packages(c(
  "tidyverse", "caret", "randomForest",
  "dslabs", "ggplot2", "e1071", "matrixStats"
))

# 2. Clone the repository
# git clone https://github.com/data-analyst-ss/ml-portfolio-R.git

# 3. Open any .Rmd or .R file in RStudio and run

# 4. Or visit the live portfolio
# https://data-analyst-ss.github.io/ml-portfolio-R
```

---

## What This Portfolio Demonstrates

**Technical skills:**
- Supervised learning — classification and regression
- Unsupervised learning — dimensionality reduction (PCA, SVD)
- Model evaluation — accuracy, sensitivity, specificity, F1-score
- Cross-validation — k-fold to prevent overfitting
- Ensemble methods — model stacking and majority voting
- Bayesian reasoning — prior, likelihood, and posterior
- Regularization — bias-variance tradeoff in practice

**Analytical thinking:**
- Choosing the right algorithm for each problem type
- Interpreting model outputs in business and clinical context
- Understanding when a single model outperforms an ensemble
- Communicating probabilistic results to non-technical audiences

---

## Certificate

**HarvardX Data Science Professional Certificate**
Course: *Machine Learning* (PH125.8x)
Platform: edX · Harvard University

---

<div align="center">

**Sarah Silva** · Senior Data & AI Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-sarahgleicesilva-9A3F4A?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/sarahgleicesilva)
[![Social Media AI](https://img.shields.io/badge/Social_Media_AI_Dashboard-BD6809?style=flat-square&logo=streamlit&logoColor=white)](https://social-media-ai-ossaocyh4myx8srgsri6up.streamlit.app)
[![Portfolio](https://img.shields.io/badge/Live_Portfolio-9A3F4A?style=flat-square&logo=github&logoColor=white)](https://data-analyst-ss.github.io/ml-portfolio-R)

</div>
