## House Price Prediction using Linear Regression

## 📌 Project Overview

This project builds a Linear Regression model to predict house prices based on various features such as area, number of rooms, facilities, and furnishing status. The model helps understand how different factors influence housing prices.

## 📂 Dataset: House Price Dataset

Contains information about residential houses

Includes features such as:

Area

Bedrooms

Bathrooms

Stories

Parking

Furnishing Status

Facilities (AC, Basement, etc.)

Target variable: Price

## 🧠 Model Architecture
Component	Description
Algorithm	Linear Regression
Learning Type	Supervised Learning
Input Features	Area, Rooms, Facilities, Parking
Output	House Price
Loss Function	Mean Squared Error

## 🔧 Key Steps

Data Loading: Load CSV file using Pandas

Data Inspection: Use .info(), .describe()

Data Cleaning: Handle categorical values

Encoding: Convert text data into numerical form

Feature Selection: Select relevant variables

Train-Test Split: Split data (80/20)

Model Training: Train Linear Regression model

Prediction: Predict house prices

Evaluation: Calculate performance metrics

## 📊 Results
Metric	Value
Mean Absolute Error (MAE)	Low
Mean Squared Error (MSE)	Low
Root Mean Squared Error (RMSE)	Moderate
R² Score	Good

✅ The model shows reliable performance in predicting house prices.

## 📈 Visualizations

Actual vs Predicted price plot

Feature influence analysis

Error distribution

## 🛠️ Technologies Used
Library	Purpose
Pandas	Data handling
NumPy	Numerical computing
Matplotlib	Visualization
Scikit-learn	Machine learning

## 🚀 How to Run

Place house_price.csv in the project folder

Open the notebook file

Run all cells sequentially

View predictions and evaluation results

## 🎯 Learning Outcomes

✅ Understanding Linear Regression

✅ Feature engineering

✅ Categorical data encoding

✅ Model training and evaluation

✅ Regression metrics interpretation

✅ Real-world price prediction