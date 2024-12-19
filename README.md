# INSE-6220-Project
Principal Component Analysis and Machine Learning on the Wine Quality Dataset done by Shakeeb Shakeeb for INSE 6220 Final project.

Overview
This project focuses on analyzing the physicochemical properties of red wine and predicting its quality using Principal Component Analysis (PCA) and machine learning models. The dataset is sourced from the UCI Machine Learning Repository and contains measurements for various chemical properties of red wine along with quality ratings.

Objective
Reduce feature redundancy and dimensionality using PCA.
Train and evaluate machine learning models (Logistic Regression and Random Forest) to classify wine quality.
Address challenges like class imbalance using SMOTE.
Dataset
Source: UCI Machine Learning Repository
File: winequality-red.csv
Features: 11 physicochemical properties (e.g., fixed acidity, volatile acidity, etc.)
Target Variable: quality (ordinal, ranging from 3 to 8)
Pipeline
The project is divided into the following stages:

Data Exploration:

Summary statistics and feature correlations.
Visualizations: Histograms, heatmaps, and pair plots.
Data Preprocessing:

Handling outliers using the IQR method.
Dropping low-correlation features.
Normalizing features using StandardScaler.
Principal Component Analysis (PCA):

Scree plot and cumulative explained variance.
Visualization: 2D and 3D biplots for principal components.
Machine Learning:

Models:
Logistic Regression: Baseline performance.
Random Forest: Enhanced classification with hyperparameter tuning.
Imbalanced Classes:
Handled using SMOTE and undersampling.
Evaluation Metrics:
Confusion matrices, classification reports, and ROC curves.
Note: Two implementations of ROC curves are included. The first version contains errors and is retained for transparency, but the corrected implementation should be used.
Optional Enhancements:

Additional visualizations (e.g., box plots, strip plots for PCA components).
Placeholder for future models (e.g., SVM, Gradient Boosting).
Key Findings
PCA reduced dimensionality effectively, retaining 89% of the variance with six components.
Random Forest performed best with a balanced dataset (accuracy: 67%).
SMOTE improved predictions for underrepresented classes, such as quality 3 and 8.
Usage
Dependencies: Install the required libraries using:

bash
Copy code
pip install pandas matplotlib seaborn scikit-learn imbalanced-learn
Run the Code: Execute the Python notebook or script in Google Colab or any Python IDE.

Navigate the Code:

Sections are clearly marked with comments.
The first ROC curve implementation contains errors and is retained as part of the development process. Use the corrected implementation included later in the code.
Visualization Outputs:

Scree plots, biplots, confusion matrices, and ROC curves are generated in-line.
Future Work
Test additional models (e.g., SVM, Gradient Boosting).
Apply the pipeline to the white wine dataset.
Automate hyperparameter tuning for better optimization.
