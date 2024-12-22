# Credit-Risk-Prediction
Credit Risk Prediction with PCA and Advanced Preprocessing
Overview
This project focuses on predicting credit risk using advanced preprocessing techniques, dimensionality reduction via PCA (Principal Component Analysis), and logistic regression modeling. The goal is to handle imbalanced datasets, encode categorical features, normalize numerical features, and apply PCA for effective feature reduction and predictive modeling.

Project Objectives
Preprocess and clean the dataset by handling missing values and encoding categorical variables.
Normalize numerical features to standardize the dataset.
Address data imbalance using SMOTEENN for improved model performance.
Apply PCA to reduce dimensionality while retaining 95% of the variance.
Implement logistic regression for efficient credit risk prediction.
Data Preprocessing Steps
1. Handling Missing Values
Categorical Variables: Missing values were filled with "Unknown" and encoded using LabelEncoder.
Numerical Variables: Missing values were replaced with the median value of each column.
2. Encoding Features
Binary Columns: Applied binary mappings for features such as Gender, Has a car, and Has a property.
Boolean Columns: Converted features like Has a mobile phone and Has an email into integer representations.
3. Normalization
Standardized numerical columns using StandardScaler to ensure uniform scaling across all features.
Dimensionality Reduction with PCA
1. Standardization
Features were standardized to ensure compatibility with PCA, which is sensitive to feature scales.
2. PCA Implementation
Retained principal components that explained 95% of the variance in the dataset.
Reduced dimensionality while preserving key information for modeling.
3. Explained Variance Analysis
Visualized the variance explained by each principal component and cumulative variance to assess the effectiveness of PCA.
Imbalanced Data Handling
Applied SMOTEENN (Synthetic Minority Oversampling Technique with Edited Nearest Neighbors) to balance the dataset:
Combined oversampling of the minority class with undersampling of the majority class.
Improved the quality of the data and addressed class imbalance effectively.
Visualization
Scatter Plots: Created to understand feature relationships.
Variance Analysis Graphs: Used to visualize the explained variance by PCA components.
Requirements
Libraries
Data Processing: pandas, numpy
Visualization: matplotlib, seaborn
Machine Learning: scikit-learn, imbalanced-learn
Dimensionality Reduction: PCA
Installation
Run the following command to install the required libraries:

bash
Copy code
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
