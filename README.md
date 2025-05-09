# AI_ML_Model-for-Result-Validation
Developed Ai-ML model for the validation of experimental results 
AI/ML-Based Experimental Validation for 3D Printing Parameters
This project aims to develop robust and accurate Machine Learning models for validating experimental outcomes in micro-extrusion-based 3D printing. Specifically, it focuses on predicting three critical parameters — Green Density, Shrinkage, and Surface Roughness — based on key process inputs like Fe Loading, Layer Thickness, and Infill Density.

The models were trained using a real-world dataset sourced from peer-reviewed experimental work, and validated against actual experimental results to assess their reliability and accuracy.

# Project Objectives
Build AI/ML models that replicate and validate experimental 3D printing results.

Analyze the influence of process parameters on green body characteristics.

Minimize prediction errors through normalization, feature engineering, and hyperparameter tuning.

Compare different algorithms to determine the best model for each output parameter.

Enable predictive modeling for efficient experimental planning and process optimization.

# Dataset Description
Source: Extracted from a published research paper using Central Composite Design (CCD).

Total Samples: 20 experimental runs.

Input Features:

Fe Loading (wt%)

Layer Thickness (mm)

Infill Density (%)

Output Parameters:

Green Density (g/cm³)

Shrinkage (%)

Surface Roughness (μm)

# Technologies Used
Python

Jupyter Notebook

scikit-learn

XGBoost

Optuna

Pandas, NumPy, Matplotlib, Seaborn

# Models Evaluated
Multiple regression models were tested and compared:

Target Parameter	Best Performing Model
Green Density	Random Forest + XGBoost (Ensemble)
Shrinkage	Polynomial Ridge Regression
Surface Roughness	XGBoost

# Performance Summary
Parameter	MSE	R² Score	Avg % Error
Green Density	0.2882	0.3387	2.50%
Shrinkage	0.0252	0.9540	2.86%
Surface Roughness	0.0036	0.9736	2.04%

# Visualizations Included
R² and MSE Comparison Charts

Actual vs Predicted Scatter Plots

% Error per Experimental Run

Model Accuracy Bar Graphs

Input vs Output Relationship Insights

All visuals were created using Matplotlib and integrated to support the interpretation of results.

# Insights & Highlights
Ensemble learning outperformed individual models for Green Density.

Shrinkage prediction achieved near-perfect R² using a 5th-degree Polynomial Ridge Regression.

XGBoost yielded the most accurate results for Surface Roughness.

The approach drastically reduces dependency on physical testing by enabling virtual validation.

# Future Scope
Integrate larger datasets from multiple experiments.

Explore deep learning approaches (e.g., ANN, CNN) for more complex datasets.

Develop a web-based interface for real-time validation predictions.

Extend the methodology to additional AM processes and materials.


