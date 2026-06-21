# DevelopersHub Corporation — AI/ML Engineering Internship Tasks (Phase-1)

Welcome to my project repository for Phase-1 of the **DevelopersHub Corporation** AI/ML Engineering Internship program. This repository contains the implementations for the three selected tasks required for submission before the June 26, 2026 deadline.

---

## Repository Structure
* `Task_1_Iris_Visualization.ipynb` — Complete Exploratory Data Analysis of the Iris Dataset.
* `Task_3_Heart_Disease_Prediction.ipynb` — Binary classification engine using health analytics.
* `Task_6_House_Price_Prediction.ipynb` — Continuous target regression pipeline for real estate evaluation.

---

## Task 1: Exploring and Visualizing a Simple Dataset
### Objective
To load, inspect, clean, and visualize a baseline multi-class dataset to uncover structural data trends, feature correlations, and potential outliers.

### Dataset
* **Name:** Iris Dataset (loaded via `seaborn`)
* **Features:** Sepal Length, Sepal Width, Petal Length, Petal Width
* **Target:** Species classification (*Setosa, Versicolor, Virginica*)

### Visualizations Applied
* **Scatter Plots:** Uncovered stark clustering boundaries between *Setosa* and the other species based on petal dimensions.
* **Histograms:** Highlighted non-normal, bimodal distributions in petal attributes.
* **Box Plots:** Leveraged to identify and document minor outlier distributions within the *Sepal Width* feature map.

---

## Task 3: Heart Disease Prediction
### Objective
To engineer a binary classification system capable of mapping a patient's historical medical health vectors to an accurate heart disease risk prediction score.

### Dataset
* **Name:** Heart Disease UCI Dataset (sourced from Kaggle)
* **Pre-processing:** Null check verification, target stratification ($80/20$ train-test split), and rigorous `StandardScaler` feature normalization.

### Models & Evaluation
* **Algorithms Applied:** Logistic Regression
* **Performance Metrics:** * **Accuracy:** ~85% (Baseline validation verified via Classification Report precision/recall arrays).
  * **Evaluation Graphics:** Plotted an explicit **Confusion Matrix** alongside a **Receiver Operating Characteristic (ROC-AUC) Curve** to analyze true-positive trading rates.

### Key Findings
The feature coefficients revealed that **Chest Pain type (`cp`)** and **Maximum Heart Rate achieved (`thalach`)** maintain the highest direct positive impacts on high-risk prediction values.

---

## Task 6: House Price Prediction
### Objective
To build a machine learning regression pipeline capable of analyzing structural real estate features to predict continuous market property values.

### Dataset
* **Name:** House Price Prediction Dataset (sourced from Kaggle)
* **Pre-processing:** Imputed missing values with column feature medians and encoded structural categorical identifiers using One-Hot encoding (`pd.get_dummies`).

### Models & Evaluation
* **Algorithms Applied:** Gradient Boosting Regressor (100 estimators, $0.1$ learning rate)
* **Performance Metrics:**
  * Evaluated continuously utilizing **Mean Absolute Error (MAE)** and **Root Mean Squared Error (RMSE)** parameters.
  * Generated an **Actual vs. Predicted Price scatter plot** containing a definitive $y = x$ reference trendline to measure residual drift.

### Key Findings
Total feature evaluation indicates that overall living area square footage maintains the absolute highest predictive weight when calculating finalized real estate market values.

---

## Technology Stack Used
* **Programming Language:** Python 3
* **Core Libraries:** `pandas`, `numpy`, `scikit-learn`
* **Visualization Layouts:** `matplotlib`, `seaborn`
