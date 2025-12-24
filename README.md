# Satellite Collision Avoidance Prediction
**Project developed during Internship at the Egyptian Space Agency (EGSA)**

## 🚀 Overview
This repository contains a machine learning pipeline to predict the risk of collision between space objects. Using real-world Conjunction Data Messages (CDMs) from the **ESA Kelvins Collision Avoidance Challenge**, I developed a system to automate the risk assessment of orbital conjunctions.

## 📊 Dataset & Features
The project analyzes over 160,000 orbital updates with 100+ features, focusing on:
- **Orbital State Vectors:** Position and velocity in the RTN frame.
- **Covariance Matrices:** Positional and velocity uncertainty.
- **Space Weather Indices:** Solar Radio Flux (F10.7), Sunspot Number (SSN), and Geomagnetic Index (AP).



## 🛠️ Repository Structure
I have organized the notebooks to follow the logical flow of a data science project:

* **EDA_and_Cleaning.ipynb**: Initial data processing and handling of orbital event IDs.
* **correlation for feature selection.ipynb**: Mathematical analysis to identify the features most predictive of collision risk.
* **Collision_Risk_RandomForest.ipynb**: The primary model achieving high-precision results (Baseline).
* **random_forest_pca.ipynb / random_forest_ica.ipynb**: Experiments using dimensionality reduction to optimize model training.
* **random_forest_fd.ipynb**: Feature extraction using Factor Analysis.
* **svr_sigmoid.ipynb (and variants)**: Comparative study of Support Vector Regression against tree-based models.



## 📈 Key Findings
- **Winning Model:** Random Forest performed significantly better than SVR, as it effectively captured the non-linear relationship between space weather and satellite drag.
- **Feature Importance:** Positional covariance features (uncertainty) showed the highest correlation with final collision risk.

## ⚙️ Requirements
- Python 3.x
- Scikit-Learn
- Pandas, NumPy, Matplotlib, Seaborn