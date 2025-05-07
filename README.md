Support Vector Machine (SVM) Classifier – Breast Cancer Detection
Overview
This project demonstrates the implementation of Support Vector Machines (SVMs) for binary classification using the Breast Cancer dataset. The focus is on comparing linear and non-linear classification using SVM kernels, tuning hyperparameters, and visualizing decision boundaries with PCA.

Objectives
Apply SVM for classifying breast cancer tumors as malignant or benign.

Explore both linear and RBF (non-linear) kernels.

Tune SVM hyperparameters (C, gamma) using GridSearchCV.

Use Principal Component Analysis (PCA) to reduce dimensions and visualize decision boundaries.

Dataset
The dataset used in this project is a breast cancer dataset containing features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass.

Features include mean, standard error, and worst value of several cell measurements.

Target column: diagnosis (converted to 1 for malignant and 0 for benign).

Technologies Used
Python 3

NumPy

Pandas

Scikit-learn

Matplotlib

Seaborn

Project Structure
bash
Copy
Edit
.
├── breast-cancer.csv
├── svm_classifier.ipynb       # Main Jupyter notebook with full code
├── README.md                  # Project documentation
Workflow
Load and preprocess the dataset.

Split the data into training and testing sets.

Apply feature scaling using StandardScaler.

Train and evaluate:

SVM with linear kernel

SVM with RBF kernel

Perform hyperparameter tuning with GridSearchCV for the RBF kernel.

Reduce feature dimensions using PCA (2D).

Train SVMs again on PCA-transformed data.

Visualize decision boundaries for both linear and RBF kernels.

Results
The linear kernel achieved high accuracy, especially after standardization.

The RBF kernel performed slightly better on complex patterns.

GridSearchCV helped optimize C and gamma, improving performance.

PCA visualizations provided clear decision boundaries for both models.

Conclusion:
SVMs are powerful models for both linear and non-linear classification tasks. With proper scaling, hyperparameter tuning, and dimensionality reduction, they can deliver high performance even on real-world medical data.
