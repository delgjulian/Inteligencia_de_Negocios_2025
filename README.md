# Predictive Modeling of Urban Ride Fares

This repository contains an applied data science project focused on the **prediction of ride fares in urban mobility platforms**, using historical trip data and a combination of statistical and machine learning models.

The project integrates **Business Intelligence (BI)** and **supervised learning** techniques to evaluate and compare the predictive performance of linear, ensemble, and neural network models in a real-world pricing problem.

---

## 📄 Project Overview

**Title:**  
*Predictive Modeling of Urban Ride Fares: A Machine Learning Approach*

The study analyzes ride-level data from an urban mobility platform (Uber, New York City) to model and predict trip fares based primarily on **geospatial information** and **trip distance**.

The workflow combines data cleaning, feature engineering, exploratory analysis, and predictive modeling to assess how different approaches perform in estimating fares with minimal input information.

---

## 🎯 Objectives

The main objectives of the project are to:

- Model the relationship between **trip distance** and **fare amount**
- Compare traditional econometric models with modern machine learning algorithms
- Evaluate predictive performance using out-of-sample metrics
- Analyze the trade-off between **interpretability** and **prediction accuracy**

---

## 🧠 Key Results (Executive Summary)

- A strong and stable positive relationship is found between **distance traveled** and **ride fare**.
- The baseline linear regression explains approximately **67% of the variance** in fares.
- Machine learning models significantly outperform linear specifications:
  - **Gradient Boosting** achieves the best overall performance  
    (RMSE ≈ **2.46**, MAE ≈ **1.73**)
  - Random Forest and Neural Networks show comparable accuracy
- High predictive accuracy is achieved using a **small set of features**, highlighting the effectiveness of distance-based pricing models.

---

## 🧪 Methodology

The analytical workflow follows a reproducible end-to-end pipeline:

1. **Data Processing and Feature Engineering**
   - Cleaning of geospatial coordinates
   - Distance computation using the **Haversine formula**
   - Detection and removal of outliers (IQR-based filtering)

2. **Exploratory Data Analysis (EDA)**
   - Distributional analysis of fares and distances
   - Pearson and Spearman correlation matrices
   - Spatial visualizations (scatter, density, hexbin maps)

3. **Predictive Modeling**
   - Ordinary Least Squares (OLS)
   - LASSO regression
   - Random Forest
   - Gradient Boosting
   - Feedforward Neural Networks (Keras)

4. **Model Evaluation**
   - Train/Test split (80/20)
   - Performance metrics: **RMSE** and **MAE**
   - Comparative assessment across models

---

## 📊 Dataset

The analysis uses a public dataset of Uber trips in **New York City**, containing georeferenced pickup and dropoff locations and the final fare amount.

After data cleaning and filtering, the final dataset includes approximately **180,000 valid observations**.

---

## 📁 Repository Structure

predictive-analytics-ride-fare-estimation/
├── README.md
├── requirements.txt
│
├── data/
│   └── uber.csv
│
├── notebooks/
│   └── 00_end_to_end_ride_fare_prediction.ipynb
│
├── figures/
│   ├── correlation_matrices.png
│   ├── spatial_distributions.png
│   ├── model_comparisons.png
│   └── ...
│
└── reports/
    └── predictive-modeling-urban-ride-fares.pdf

---

## ▶️ Reproducibility

The project can be executed locally or in Google Colab using Python 3.10+.

Main dependencies include:

pip install numpy pandas scikit-learn tensorflow matplotlib seaborn


Running the main notebook reproduces all figures, models, and results reported in the final document.

---

## 📚 Background and References

The project builds on standard concepts from:

Business Intelligence and predictive analytics

Econometric regression models

Ensemble learning (Random Forest, Gradient Boosting)

Neural networks for regression tasks

Urban mobility and pricing analytics

---
## 📝 License

This repository is released under the MIT License, allowing free academic and research use, modification, and redistribution.

---

## 👤 Author

Julián Alberto Delgadillo Marín
M.Sc. in Applied Economics (candidate)
University of Buenos Aires (UBA)
