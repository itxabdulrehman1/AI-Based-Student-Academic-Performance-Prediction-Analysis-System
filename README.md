# AI-Based-Student-Academic-Performance-Prediction-Analysis-System

Recommended Execution Order
1️⃣ First Run
01_data_exploration.ipynb

Purpose:

Load dataset
Inspect columns
Check shape
Check datatypes
Check missing values
Check duplicates

Expected output:

Dataset Shape
Column Names
Missing Values Report
Statistical Summary

If this notebook fails, do not continue.

2️⃣ Second Run
02_data_preprocessing.ipynb

Purpose:

Missing value handling
Duplicate removal
Outlier treatment
Encoding
Scaling

Expected output:

df_clean
cleaned dataset
preprocessing summaries

This notebook often creates:

data_cleaned.csv

or

df_clean

which later notebooks use.

3️⃣ Third Run
03_exploratory_data_analysis.ipynb

Purpose:

Visualizations
Correlation analysis
Performance distributions
Feature relationships

Expected output:

Heatmaps
Boxplots
Histograms
Scatterplots

This notebook usually doesn't create data for later notebooks, but it validates that preprocessing worked.

4️⃣ Fourth Run
04_clustering_kmeans.ipynb

Purpose:

K-Means clustering
Elbow Method
Silhouette Score

Expected output:

Optimal K
Cluster Graph
Silhouette Score

This notebook is mostly independent after preprocessing.

5️⃣ Fifth Run
05_regression_linear.ipynb

Purpose:

Linear Regression
RMSE
MAE
R²

Expected output:

RMSE
MAE
R²
Prediction Plot

Check whether the audit fix for target leakage was applied.

6️⃣ Sixth Run
06_classification_models.ipynb

Purpose:

Logistic Regression
Decision Tree
Random Forest

Expected output:

Accuracy
Precision
Recall
F1
Confusion Matrix
Classification Report

This is your most important notebook for the presentation.

7️⃣ Final Run
09_model_comparison.ipynb

Purpose:

Compare all models
Generate final charts
Identify best model

Expected output:

Model Comparison Table

Logistic Regression
Decision Tree
Random Forest
Linear Regression
K-Means
