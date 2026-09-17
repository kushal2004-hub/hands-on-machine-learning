## Dimensionality Reduction using Principal Component Analysis (PCA)

## 📌 Project Overview

This project demonstrates how Principal Component Analysis (PCA) is used to reduce high-dimensional data into fewer components while preserving most of the important information. The technique is applied on a real-world medical dataset to improve visualization and computational efficiency.

## 📂 Dataset: Breast Cancer Dataset (Scikit-learn)

Built-in dataset from Scikit-learn

Contains 569 samples and 30 numerical features

Features represent characteristics of cell nuclei

Target: Benign / Malignant (optional)

## 🧠 Model Architecture
Component	Description
Technique	Principal Component Analysis
Learning Type	Unsupervised Learning
Preprocessing	StandardScaler
Input Features	30 Numerical Features
Output	Principal Components (PC1, PC2)

## 🔧 Key Steps

Dataset Loading: Load dataset using sklearn

Data Inspection: Analyze structure and statistics

Standardization: Scale features

Apply PCA: Compute principal components

Variance Analysis: Plot explained variance

Dimensionality Reduction: Reduce to 2 dimensions

Visualization: Plot reduced data

## 📊 Results
Metric	Value
Original Features	30
Reduced Features	2
Samples	569
Variance Retained	~95%

✅ Effective dimensionality reduction achieved.

## 📈 Visualizations

Explained variance (scree plot)

2D PCA projection

Feature variance analysis

## 🛠️ Technologies Used
Library	Purpose
Pandas	Data handling
NumPy	Numerical computing
Matplotlib	Visualization
Scikit-learn	PCA & preprocessing

## 🚀 How to Run

Open the notebook file

Run all cells sequentially

View variance plot

Analyze PCA projection

## 🎯 Learning Outcomes

✅ Understanding PCA fundamentals

✅ Feature scaling

✅ Dimensionality reduction

✅ Variance preservation

✅ Data visualization

✅ Working with high-dimensional data