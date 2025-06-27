Breast Cancer Logistic Regression
Task Overview
This repository contains the solution for Task 4 of the Elevate AI & ML Internship. The objective is to implement a binary classifier using logistic regression on the Breast Cancer Wisconsin Dataset to predict diagnosis (Malignant/Benign).
Steps Performed

Data Preprocessing:
Loaded data.csv and encoded diagnosis (M=1, B=0).
Dropped id column.
Standardized numerical features.


Exploratory Data Analysis:
Generated summary statistics and visualized class distribution.
Created a correlation matrix for key features.


Logistic Regression:
Split data into train (80%) and test (20%) sets.
Trained a logistic regression model.
Evaluated using confusion matrix, precision, recall, and ROC-AUC.
Tuned classification thresholds (0.3, 0.5, 0.7).
Visualized the sigmoid function to explain probability outputs.



Files

breast_cancer_logistic_regression.ipynb: Jupyter Notebook with preprocessing, EDA, and logistic regression code.
data.csv: Original Breast Cancer Wisconsin Dataset.
Breast_Cancer_Cleaned.csv: Preprocessed dataset.
class_distribution.png: Bar plot of class distribution.
correlation_matrix.png: Correlation matrix heatmap.
confusion_matrix.png: Confusion matrix heatmap.
roc_curve.png: ROC curve plot.
sigmoid_function.png: Sigmoid function plot.
interview_questions.md: Answers to provided interview questions.
README.md: This documentation file.

Tools Used

Python 3
Jupyter Notebook
Pandas
NumPy
Matplotlib
Seaborn
scikit-learn

How to Run

Clone this repository:git clone https://github.com/Amaljithuk/AI-ML-INTERNSHIP-TASK4.git


Install required dependencies:pip install pandas numpy matplotlib seaborn scikit-learn jupyter


Launch Jupyter Notebook:jupyter notebook


Open breast_cancer_logistic_regression.ipynb and run all cells to:
Generate the cleaned dataset (Breast_Cancer_Cleaned.csv).
Save visualizations (class_distribution.png, correlation_matrix.png, confusion_matrix.png, roc_curve.png, sigmoid_function.png).
Display model metrics and threshold tuning results.



Observations

EDA: Class distribution shows more Benign (0) than Malignant (1) cases. Features like radius_mean, perimeter_mean, and area_mean are strongly correlated with diagnosis.
Model Performance: High precision, recall, and ROC-AUC indicate a robust model. The ROC curve shows excellent class separation (AUC ≈ 1).
Threshold Tuning: A lower threshold (0.3) increases recall, reducing missed Malignant cases, which is critical for medical applications.
Sigmoid Function: Maps model outputs to probabilities, with 0.5 as the default classification threshold.
Inferences: The model is effective for binary classification, but class imbalance could be addressed with techniques like SMOTE if performance degrades.

Notes

The notebook suppresses warnings for cleaner output.
The cleaned dataset is suitable for classification tasks.
Visualizations and metrics provide insights into model performance and feature importance.

Submission
This repository is submitted for Task 4 of the Elevate AI & ML Internship, completed on June 27, 2025, within the 10:00 AM to 10:00 PM submission window.
