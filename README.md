# Parkinson's Disease Prediction using Machine Learning

##  Overview
This project predicts the presence of Parkinson’s Disease using machine learning techniques based on biomedical voice measurements.

Parkinson’s Disease is a neurodegenerative disorder that affects movement and speech. Early detection is crucial, and this project aims to assist in preliminary diagnosis using data-driven methods

## Tech Stack
- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Matplotlib  
- Seaborn  

##  Workflow
1. Data Collection  
2. Data Preprocessing  
3. Exploratory Data Analysis (EDA)  
4. Feature Scaling using StandardScaler  
5. Train-Test Split  
6. Model Training using Support Vector Machine (SVM)  
7. Model Evaluation  

##  Model Details
- Algorithm: Support Vector Machine (SVM)  
- Kernel: linear 
- Feature Scaling applied for better performance

##  Results
- Accuracy: 88%

The model demonstrates reliable performance in predicting disease presence.

## Visualizations & Analysis

### Correlation Heatmap
The correlation heatmap shows relationships between biomedical voice features used for Parkinson’s prediction.

- Features related to **frequency variation (jitter, shimmer)** and **noise measures (NHR, HNR)** show stronger correlation with the target variable.
- Some features are highly correlated with each other, indicating possible redundancy.
- This helps in understanding which voice characteristics are important indicators of Parkinson’s Disease.

### Class Distribution
The dataset consists of two classes:
- **0 → Healthy**
- **1 → Parkinson’s Disease**

- The distribution plot shows whether the dataset is balanced.
- A balanced dataset helps improve model reliability and avoids bias toward one class.

### Feature Distribution
Feature distribution plots show how different voice measurements are spread across the dataset.

- Many features are slightly skewed due to the nature of biomedical signals.
- Scaling (StandardScaler) is important to normalize these variations before training the model.

### Confusion Matrix
The confusion matrix evaluates the model’s classification performance.

- **True Positives (TP):** Correctly predicted Parkinson’s cases  
- **True Negatives (TN):** Correctly predicted healthy cases  
- **False Positives (FP):** Healthy predicted as Parkinson’s  
- **False Negatives (FN):** Parkinson’s cases missed by the model  

Key insights:
- Minimizing **false negatives** is critical, as missing a Parkinson’s case can delay diagnosis.
- High diagonal values indicate strong model performance.
