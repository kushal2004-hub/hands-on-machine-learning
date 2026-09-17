## Customer Segmentation using K-Means Clustering

## 📌 Project Overview

This project performs customer segmentation using K-Means clustering on the Mall Customers dataset. The model groups customers based on their annual income and spending behavior to help businesses understand different customer types.

## 📂 Dataset: Mall Customers

200 customers

Features Used:

Annual Income (k$)

Spending Score (1–100)

Dataset collected from shopping mall customers

## 🧠 Model Architecture
Component	Description
Algorithm	K-Means Clustering
Distance Metric	Euclidean Distance
Clusters	5
Optimization	Elbow Method
Evaluation	Silhouette Score

## 🔧 Key Steps

Data Loading: Load CSV using Pandas

Exploration: View customer distribution

Feature Selection: Select income and spending score

Optimization: Apply Elbow Method

Model Training: Train K-Means model

Evaluation: Calculate silhouette score

Visualization: Plot clusters and centroids

Saving Model: Store trained model using Pickle

## 📊 Results
Metric	Value
Optimal Clusters	5
Silhouette Score	~0.55
Customer Groups	5 Segments
Sample Output

Each customer is assigned a cluster label from 0 to 4 based on spending behavior.

✅ Clear segmentation of customer groups achieved!

## 📈 Visualizations

Customer distribution scatter plot

Elbow method curve

Cluster visualization with centroids

## 🛠️ Technologies Used
Library	Purpose
Pandas	Data handling
Matplotlib	Visualization
Scikit-learn	Clustering & metrics
Pickle	Model saving

## 🚀 How to Run

Place Mall_Customers.csv in project folder

Open notebook

Run all cells

View cluster visualizations

Model will be saved automatically

## 🎯 Learning Outcomes

✅ Understanding unsupervised learning

✅ Implementing K-Means clustering

✅ Using Elbow method

✅ Evaluating clusters

✅ Visualizing customer segments

✅ Saving ML models