---
title: "Red Wine Quality Classification — ML Model Comparison"
collection: portfolio
permalink: /portfolio/2025-05-07-red-wine-quality-classification
excerpt: "Classified UCI red wine quality scores (3–8) using ANN, KNN, and SVM with PCA + standardization, tuned via GridSearchCV + cross-validation. <br/><img src='/images/red_wine.jpg' alt='Red Wine Quality Classification' style='max-width: 100%; height: auto; width: 480px;' >"
date: "2025 May"
created_on: "Spring 2025 ESE 417 Final Project"
venue: "Washington University in St. Louis"
source_code: "https://github.com/andr3wtn/andrewtinajack"
---

Highlights:
- Built an end-to-end classification pipeline on the UCI Red Wine Quality dataset (1599 samples, 11 numerical features) to predict discrete quality scores on an imbalanced label distribution (mostly 5–6). 
- Performed exploratory analysis (histograms + correlation heatmap) to identify skewed feature distributions and multicollinearity (e.g., total vs free sulfur dioxide, pH vs fixed acidity). 
- Trained and tuned ANN (MLPClassifier), KNN, and SVM (SVC) using train/test split + 4-fold GridSearchCV (accuracy as the metric), then compared raw vs PCA-reduced vs standardized feature sets. 
- Evaluated the impact of PCA feature reduction (10 → 5–10 dims) and StandardScaler preprocessing; standardization improved all models, with KNN achieving the strongest overall accuracy after scaling. 

Tech Stack:
- Python (scikit-learn)
- MLPClassifier (ANN), KNeighborsClassifier, SVC (SVM)
- PCA, StandardScaler
- GridSearchCV + Cross-Validation
- Matplotlib (visualizations)

Links:
- Source code: https://github.com/andr3wtn/andrewtinajack