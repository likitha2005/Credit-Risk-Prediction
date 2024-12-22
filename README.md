

# Credit Risk Prediction with PCA and Advanced Preprocessing

This project focuses on predicting credit risk using advanced preprocessing techniques, dimensionality reduction with PCA (Principal Component Analysis), and logistic regression modeling. It aims to handle imbalanced datasets, encode categorical features, normalize numerical features, and apply PCA for effective feature reduction and predictive modeling.

## Project Objectives
- **Preprocess and clean the dataset** by handling missing values and encoding categorical variables.
- **Normalize numerical features** to standardize the dataset.
- **Address data imbalance** using SMOTEENN for improved model performance.
- **Apply PCA** to reduce dimensionality while retaining 95% of the variance.
- **Implement logistic regression** for efficient credit risk prediction.

## Data Preprocessing Steps
1. **Handling Missing Values**
   - **Categorical Variables**: Missing values filled with "Unknown" and encoded using LabelEncoder.
   - **Numerical Variables**: Missing values replaced with the median value of each column.

2. **Encoding Features**
   - **Binary Columns**: Features such as Gender, Has a car, and Has a property are mapped to binary values.
   - **Boolean Columns**: Features like Has a mobile phone and Has an email are converted to integer representations.

3. **Normalization**
   - Numerical columns are standardized using StandardScaler to ensure uniform scaling across all features.

## Dimensionality Reduction with PCA
1. **Standardization**
   - Features were standardized to ensure compatibility with PCA, which is sensitive to feature scales.

2. **PCA Implementation**
   - Retained principal components that explained 95% of the variance in the dataset.
   - Reduced dimensionality while preserving key information for modeling.

3. **Explained Variance Analysis**
   - Visualized the variance explained by each principal component and cumulative variance to assess the effectiveness of PCA.

## Imbalanced Data Handling
- **SMOTEENN (Synthetic Minority Oversampling Technique with Edited Nearest Neighbors)** was applied to balance the dataset:
  - Combined oversampling of the minority class with undersampling of the majority class to improve the quality of the data.

## Visualization
- **Scatter Plots**: To understand feature relationships.
- **Variance Analysis Graphs**: Visualized the explained variance by PCA components.

## Requirements
### Libraries
- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, seaborn
- **Machine Learning**: scikit-learn, imbalanced-learn
- **Dimensionality Reduction**: PCA

## Installation
To install the required libraries, run the following command:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

## How to Run
### Clone the Repository:
```bash
git clone https://github.com/likitha2005/Credit-Risk-Prediction
cd credit-risk-prediction
```

### Install Dependencies:
```bash
pip install -r requirements.txt
```

### Prepare Dataset:
Ensure the dataset `train_mini.csv` is placed in the working directory.

### Run the Script:
Open the Jupyter Notebook or Python script provided and execute the cells sequentially to preprocess the data, apply PCA, balance the data, and visualize the results.

---


