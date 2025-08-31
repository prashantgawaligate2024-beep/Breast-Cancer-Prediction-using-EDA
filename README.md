# Breast-Cancer-Prediction-using-EDA
# Breast Cancer Classification Project

## Overview
This project uses the Wisconsin Breast Cancer dataset to predict malignant vs. benign tumors using machine learning.  
Key steps include data cleaning, feature scaling, exploratory analysis, and building a logistic regression classifier.

## Dataset
- *Size:* 569 rows × 33 columns  
- *Target:* Diagnosis (Malignant / Benign)  
- *Issue:* Unnamed: 32 column with 569 missing values  

## Steps
1. *Data Cleaning:*  
   - Dropped Unnamed: 32 (100% missing).  
   - Encoded diagnosis into binary (0 = Benign, 1 = Malignant).  
   - Final shape: *569 × 32* numeric dataset.  

2. *Feature Scaling & EDA:*  
   - Applied StandardScaler (fit on 455 train samples).  
   - Standardized features to mean=0, std=1.  
   - Identified strong correlations (e.g., radius_mean vs perimeter_mean r≈0.998).  

3. *Modeling:*  
   - Split dataset into 80% train (455) / 20% test (114).  
   - Trained *Logistic Regression (L2 regularization)*.  
   - *Result:* 97.37% test accuracy (111/114 correct).  

## Results
- Logistic Regression achieved *high accuracy and reliable classification*.  
- Demonstrated strong predictive power for medical diagnostics.  

## Next Steps
- Add ROC-AUC, sensitivity, and specificity for medical relevance.  
- Explore dimensionality reduction (PCA) to handle multicollinearity.  
- Compare with advanced models (Random Forest, SVM, Neural Nets).  

---
