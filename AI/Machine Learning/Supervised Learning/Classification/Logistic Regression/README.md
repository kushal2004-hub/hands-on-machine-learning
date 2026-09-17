# Student Placement Prediction using Logistic Regression

## 📌 Project Overview
This notebook builds a Logistic Regression model to predict whether a student will be placed based on their academic records and demographics. The model achieves 77.78% accuracy on test data.

## 📂 Dataset: Student Placement Data
Source: Campus recruitment dataset

Total samples: 1,050 students

## Features: 11 features including academic scores, skills, and demographics

Target:

0: Not Placed (512 students, 48.8%)

1: Placed (538 students, 51.2%)

## Features
Column	Description
Student_ID	Unique student identifier (dropped)
Gender	Male/Female
Branch	Engineering branch (IT, ECE, ME, CE, CSE)
CGPA	Cumulative Grade Point Average (0-10 scale)
Internships	Number of internships completed
Backlogs	Number of active backlogs
Programming_Skills	Beginner/Intermediate/Advanced
Aptitude_Score	Score in aptitude test (0-100)
Communication_Skills	Poor/Average/Good
Extra_Certifications	Number of additional certifications
Placement_Status	Target: Placed/Not Placed


## 📊 Exploratory Data Analysis
Placement Rate: 51.2% of students placed

Missing Values: No missing values found in dataset

Feature Correlations:

CGPA (0.34) and Internships (0.29) show strongest positive correlation with placement

Backlogs (-0.17) shows negative correlation with placement

## 🔧 Key Steps
Data Loading: Upload CSV file in Google Colab

Exploratory Data Analysis: Visualize distributions and correlations

Data Preprocessing: Drop 'Student_ID', rename target column

Label Encoding: Convert categorical variables to numerical

Feature Scaling: StandardScaler for numerical features

Train-Test Split: 70-30 split with stratification

Model Training: Logistic Regression with lbfgs solver (max_iter=4000)

Evaluation: Accuracy, ROC-AUC, confusion matrix, classification report

Feature Importance: Analyze coefficients

Prediction Function: Predict for new students

Model Comparison: Compare with Random Forest, Decision Tree, SVM

## 📈 Results
Model Performance
Metric	Value
Training Accuracy	73.88%
Testing Accuracy	77.78%
ROC-AUC Score	0.861
5-Fold CV Mean	74.95% (±4.28%)