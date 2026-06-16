# 🤖 MLEA: Machine Learning

Welcome to the repository for **MLEA_M** (Machine Learning) at the *Escuela Colombiana de Ingeniería Julio Garavito* — Master's in Data Science program.
This collection documents the complete journey through machine learning fundamentals, from Python foundations and supervised learning to advanced ensemble methods, unsupervised learning, and a full end-to-end ML project applied to real-world data.

---

## 📚 Topics Covered

### 🐍 Python & Data Science Foundations

* Python data types, control flow, functions, and lambda expressions
* NumPy arrays, vectorized operations, and statistical functions
* Pandas DataFrames, data wrangling, and exploratory analysis
* Matplotlib & Seaborn for data visualization

### 📈 Supervised Learning — Regression

* Simple and multiple linear regression
* One-Hot Encoding for categorical variables
* Train / Validation / Test split strategy and data leakage prevention
* Evaluation metrics: MAE, MSE, RMSE, R²
* SVR, Random Forest Regressor, Gradient Boosting Regressor, XGBoost Regressor

### 🎯 Supervised Learning — Classification

* Binary classification with Logistic Regression
* Stratified partitioning for imbalanced datasets
* Multi-class classification with MNIST (digits)
* Decision Trees, SVM, Random Forest, Gradient Boosting, XGBoost
* Neural Networks (MLP) for classification and regression
* Decision boundary visualization

### 📊 Model Evaluation & Optimization

* Confusion matrix, Accuracy, Precision, Recall, F1-Score, ROC-AUC
* Cross-Validation (CV) and StratifiedKFold
* Hyperparameter tuning: GridSearchCV and RandomizedSearchCV
* Feature selection: SelectKBest, RFE, SelectFromModel
* Threshold optimization and business-driven metric selection
* SHAP values for model interpretability

### 🔍 Unsupervised Learning & Dimensionality Reduction

* K-Means clustering and the elbow method
* Gaussian Mixture Models (GMM) with BIC/AIC selection
* Principal Component Analysis (PCA) and explained variance
* t-SNE for non-linear visualization
* UMAP for structure-preserving projections
* Autoencoders (MLP-based) for representation learning
* Anomaly detection: Isolation Forest, One-Class SVM, Local Outlier Factor

### ⚡ AutoML with PyCaret

* Automated model comparison and hyperparameter tuning
* Classification, regression, clustering, and anomaly detection pipelines
* SHAP-based model interpretation
* Model stacking and ensemble strategies

---

## 🚀 Final Project — Exoplanet ML Classifier

The final course project is a complete, end-to-end Machine Learning application built on real NASA data. Below are the two repositories that make up the full deliverable:

### 🔹 1. ML Pipeline — Exoplanet Classifier

A reproducible machine learning workspace that automates the vetting of NASA Kepler Objects of Interest (KOIs) to determine whether candidate signals represent true exoplanets or false positives. Built for the MLEA course as the final project submission.

**Key highlights:**

* Problem: Binary classification (CANDIDATE vs. FALSE POSITIVE) on NASA Kepler KOI data
* Dataset: NASA Cumulative KOI Table — thousands of observations with 40+ stellar and transit features
* EDA: Descriptive statistics, class imbalance analysis, correlation heatmaps, and feature distributions
* Models: Logistic Regression, Random Forest, Gradient Boosting, and XGBoost (minimum 4 approaches)
* Hyperparameter tuning via GridSearchCV and RandomizedSearchCV
* Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC, Confusion Matrix
* Reproducible Jupyter Notebook with markdown-documented cells

[🔗 View Repository — Exoplanet ML Pipeline](https://github.com/AnderssonProgramming/exoplanet-ml-classifier)

---

### 🔹 2. Design System — Presentation Deck

A zero-dependency visual vocabulary and 20-slide responsive presentation deck built with vanilla JavaScript, pure HTML/CSS, and atomic design tokens. Covers the full project narrative from problem motivation through conclusions.

**Key highlights:**

* 13 pure HTML/CSS academic components (cards, badges, tables, charts, code blocks)
* Atomic design tokens for consistent visual language
* 20-slide responsive deck presenting: problem, data, EDA, models, metrics, application, and conclusions
* No external dependencies — works offline in any modern browser

[🔗 View Repository — Exoplanet ML Design System](https://github.com/AnderssonProgramming/exoplanet-ml-classifier-design-system)

---

## 📁 Repository Structure

### 📘 Session 01 — Python & Data Science Foundations

**Focus**: Python fundamentals and NumPy as preparation for ML workflows

* Python types, strings, lists, dictionaries, control flow, and functions
* Lambda expressions and list comprehensions
* NumPy arrays, matrix operations, and statistical functions
* Matplotlib visualization basics

**Key Notebooks:**
* [clase1a.ipynb](01%20-%20Class/clase1a.ipynb) — Python fundamentals tutorial (types, structures, NumPy intro)
* [clase1b.ipynb](01%20-%20Class/clase1b.ipynb) — Extended Python exercises
* [clase1c.ipynb](01%20-%20Class/clase1c.ipynb) — Data science foundations

**Reference Slides:**
* [Session 1 - Machine Learning Overview.pdf](01%20-%20Class/Session%201%20-%20Machine%20Learning%20Overview.pdf)

---

### 📗 Session 02 — Linear Models & Regression

**Focus**: Scikit-Learn API, linear regression (simple, multiple, with categoricals), and evaluation metrics

* Train / Validation / Test split and the golden rule of holdout sets
* Stratified partitioning for imbalanced datasets
* Simple and multiple linear regression with Scikit-Learn
* One-Hot Encoding for categorical variables (avoiding the dummy variable trap)
* Regression metrics: MAE, MSE, RMSE, R²
* Binary classification with Logistic Regression
* Sigmoid function, confusion matrix, ROC-AUC, and threshold optimization
* Precision/Recall trade-off and F1-Score
* Multi-class classification with MNIST (Logistic Regression vs. MLP)

**Key Notebooks:**
* [clase2a.ipynb](02%20-%20Class/clase2a.ipynb) — Linear regression: simple, multiple, with categorical features
* [clase2b.ipynb](02%20-%20Class/clase2b.ipynb) — Binary classification, metrics, ROC curve, threshold tuning

**Reference Slides:**
* [Session 2 – Linear Models.pdf](02%20-%20Class/Session%202%20–%20Linear%20Models.pdf)

---

### 📙 Session 03 — Artificial Neural Networks

**Focus**: MLPClassifier and MLPRegressor as bridges between linear models and deep learning

* Linear regression revisited through the lens of a single-neuron MLP
* Binary and multi-class classification (MNIST) with MLP
* Decision boundary visualization for Logistic Regression vs. MLP
* Learning curves and early stopping
* Comparing Logistic Regression accuracy vs. MLP accuracy on MNIST

**Key Notebooks:**
* [clase3a.ipynb](03%20-%20Class/clase3a.ipynb) — Classification & regression with ANNs, MNIST multi-class

**Reference Slides:**
* [Session 03 - ANNs.pdf](03%20-%20Class/Session%2003%20-%20ANNs.pdf)

---

### 📕 Session 04 — Ensemble Methods & Tree-Based Models

**Focus**: Tree models, ensembles, and boosting for both classification and regression

**Classification (clase4a):**
* Decision Tree Classifier with `plot_tree` visualization
* SVM (RBF kernel) with feature scaling
* Random Forest Classifier and feature importance
* Gradient Boosting Classifier
* XGBoost Classifier
* PyCaret automated model comparison (sorted by Recall)

**Regression (clase4b):**
* Decision Tree Regressor
* SVR with RBF kernel
* Random Forest Regressor
* Gradient Boosting Regressor
* XGBoost Regressor
* PyCaret for regression pipeline automation

**Key Notebooks:**
* [clase4a.ipynb](04%20-%20Class/clase4a.ipynb) — SVM, Random Forest, Gradient Boosting, XGBoost (classification)
* [clase4b.ipynb](04%20-%20Class/clase4b.ipynb) — SVR, Random Forest, Gradient Boosting, XGBoost (regression)

**Reference Slides:**
* [Supervised Learning_2026.pdf](04%20-%20Class/Supervised%20Learning_2026.pdf)

---

### 📓 Session 05 — Cross-Validation, Feature Selection & Hyperparameter Tuning

**Focus**: Robust model evaluation and optimization using the Pima Indians Diabetes dataset

* Cross-validation concepts and StratifiedKFold
* GridSearchCV and RandomizedSearchCV with CV
* Feature selection methods:
  * SelectKBest (ANOVA F-score)
  * Recursive Feature Elimination (RFE)
  * SelectFromModel (Random Forest importances)
* LogisticRegressionCV for automatic regularization tuning
* SVM, Random Forest, and Gradient Boosting with combined CV + feature selection
* PyCaret AutoML: setup, compare_models, tune_model, ensemble (Bagging/Boosting/Stacking)
* SHAP values via LightGBM interpretability
* Bayesian hyperparameter optimization

**Key Notebooks:**
* [Copia_de_clase5.ipynb](05%20-%20Class/Copia_de_clase5.ipynb) — Full CV, feature selection, and hyperparameter tuning workflow

**Reference Slides:**
* [Session 05_2026.pdf](05%20-%20Class/Session%2005_2026.pdf)

---

### 📒 Session 06 — Unsupervised Learning & Dimensionality Reduction

**Focus**: Clustering, dimensionality reduction, anomaly detection on Iris and MNIST

* **K-Means**: elbow method, silhouette score
* **Gaussian Mixture Models**: BIC/AIC model selection, probabilistic assignment
* **PCA**: explained variance, 2D/nD projections
* **t-SNE**: perplexity parameter, non-linear neighborhood preservation
* **UMAP**: faster alternative to t-SNE, preserves global structure
* **Autoencoders**: MLPRegressor bottleneck for representation learning and digit generation
* **Anomaly Detection**: Isolation Forest, One-Class SVM, Local Outlier Factor
* Autoencoder-based anomaly detection via reconstruction error (ROC-AUC)
* PyCaret clustering and anomaly detection pipelines

**Key Notebooks:**
* [clase6.ipynb](06%20-%20Class/clase6.ipynb) — Clustering, PCA, t-SNE, UMAP, Autoencoders, Anomaly Detection
* [Sesión_6b.ipynb](06%20-%20Class/Sesión_6b.ipynb) — PyCaret clustering and anomaly detection automation

**Reference Slides:**
* [Session 06 - unsupervised learning_2026.pdf](06%20-%20Class/Session%2006%20-%20unsupervised%20learning_2026.pdf)

---

## 🧪 Key Learning Components

### 📓 Jupyter Notebooks
Interactive Python notebooks implementing every concept step-by-step, with markdown documentation, inline visualizations, and guided exercises.

### 🔬 Comparative Model Analysis
Each session systematically compares multiple algorithms on the same dataset, making it easy to understand trade-offs in accuracy, interpretability, and computational cost.

### 📊 Evaluation-First Approach
Every model is evaluated with the appropriate metric set: regression uses MAE/RMSE/R², classification uses the full confusion matrix family, and unsupervised learning uses silhouette scores and visual projections.

### 🎓 End-to-End Final Project
The capstone project (linked above) follows the full ML lifecycle: problem framing → data → EDA → modeling → evaluation → application context → conclusions, matching the course rubric requirements exactly.

---

## 🧰 Tech Stack & Tools

* `Python 3.13 🐍` — Primary programming language
* `NumPy 🔢` — Numerical computing and array operations
* `Pandas 🗂️` — Data manipulation and analysis
* `Scikit-Learn 1.6 ⚙️` — Core ML algorithms, preprocessing, and evaluation
* `XGBoost ⚡` — Extreme Gradient Boosting
* `PyCaret 3 🔮` — AutoML: classification, regression, clustering, anomaly detection
* `Matplotlib & Seaborn 📊` — Data and model visualization
* `UMAP 🌐` — Non-linear dimensionality reduction
* `Jupyter Notebooks 📓` — Interactive development environment

---

## 🖼️ Visuals

<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" width="65px"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="NumPy" width="65px" style="margin-left: 20px;"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" alt="Pandas" width="65px" style="margin-left: 20px;"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original-wordmark.svg" alt="Jupyter" width="65px" style="margin-left: 20px;"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" alt="Scikit-Learn" width="65px" style="margin-left: 20px;"/>
</p>

---

## 🎓 Course Progression

```
Session 01 — Python & NumPy Foundations
    ↓
Session 02 — Linear & Logistic Regression · Evaluation Metrics
    ↓
Session 03 — Artificial Neural Networks (MLP)
    ↓
Session 04 — Trees · SVM · Random Forest · Gradient Boosting · XGBoost
    ↓
Session 05 — Cross-Validation · Feature Selection · Hyperparameter Tuning
    ↓
Session 06 — Clustering · PCA · t-SNE · UMAP · Anomaly Detection
    ↓
Final Project — End-to-End ML on Real NASA Exoplanet Data
```

---

## 📋 Final Project Requirements (MLEA_M 2026-1)

The course final project (graded out of 50 points) requires:

| Section | Points | Description |
|---|---|---|
| Problem & Motivation | 4 | Clear real-world problem framing, relevance, and ML justification |
| Data | 4 | Source description, variable count, missing values, class imbalance |
| EDA | 8 | Descriptive stats, visualizations, pattern identification |
| Models | 14 | Minimum 3 models (ideally 4+), justified selection, diverse approaches |
| Comparative Metrics | 6 | Accuracy, Precision, Recall, F1, confusion matrix, cross-model comparison |
| Hyperparameters | 4 | GridSearch / RandomSearch application and selection justification |
| Application | 4 | Real-world deployment context, end users, decision impact |
| Code | 3 | Organized, documented, reproducible Jupyter Notebook |
| Presentation | 3 | Clarity, timing (12 min), all members participating |
| **Total** | **50** | |

---

## 📖 Additional Resources

* [Accurate Predictions on Small Data (PDF)](Accurate%20predictions%20on%20small%20data.pdf) — Supplementary reading on small-data ML strategies

---

## 📬 Contact

Explore the mathematics behind the models, experiment with hyperparameters, and push the boundaries of what machine learning can predict.

💌 **[andersson.sanchez-m@mail.escuelaing.edu.co](mailto:andersson.sanchez-m@mail.escuelaing.edu.co)** — Let's build intelligent systems together!

---

> *"In God we trust. All others must bring data."* — W. Edwards Deming
>
> Learn the models. Understand the data. Ship something that works. 🤖📊
