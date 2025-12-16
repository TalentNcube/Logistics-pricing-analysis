# Logistics-pricing-analysis
Logistics Pricing Modeling: A Comparative Analysis of Machine Learning Techniques for Tipper Cost Estimation
Introduction

Project Background
The efficient and competitive pricing of logistics services, particularly for bulk material transport using tipper trucks, is crucial for operational profitability. Traditional pricing methods often rely on fixed distance rates, which can fail to capture nuanced market dynamics and result in either lost revenue or lost bids.

Objective

This research project aims to develop a robust, data-driven logistics pricing model for 20-ton (20t) and 30-ton (30t) tipper trucks. The primary goal is to compare the performance of three popular machine learning regression algorithms—Linear Regression, Random Forest, and K-Nearest Neighbors (KNN)—in predicting the Cost per Ton based solely on the  Radius Distance (km). The final outcome is a clear recommendation on the most effective model for future pricing decisions.

Methodology

Data Source and Preparation
The analysis was based on the provided dataset: "Area distances.xlsx - Sheet1.csv".
•	Feature: Radius_km (Distance in kilometers)
•	Target Variables: Cost_20t (Cost/ton for 20t tipper) and Cost_30t (Cost/ton for 30t tipper)
•	Data Cleaning: The initial dataset required cleaning to convert cost and distance columns from string format (with comma separators) to numerical format, and any rows with missing data were removed to ensure model integrity.

Model Selection

Three machine learning models were selected to represent different approaches to regression:
1.	Linear Regression (LR): A simple, interpretable model assuming a linear relationship between distance and cost.
2.	Random Forest Regressor (RF): An ensemble learning method capable of capturing complex, non-linear relationships and interactions.
3.	K-Nearest Neighbors Regressor (KNN): A non-parametric, instance-based learning algorithm that uses local data points to make predictions.


Evaluation Metrics

Model performance was assessed using the following metrics:

1.R-squared (R^2): Represents the proportion of the variance for a dependent variable that's explained by the independent variables. A value closer to 1.0 indicates a better fit.

2.Mean Absolute Error (MAE): The average magnitude of the errors in a set of predictions, without considering their direction. It is expressed in the same units as the target variable (Cost/ton), making it highly interpretable.


Results and Interpretation

Model Performance Comparison

The models were trained and tested on the historical data. The consolidated performance results are presented below:
https://github.com/TalentNcube/Logistics-pricing-analysis/blob/589ef77a40f598cf1bc9e53a1293f7cc4e70f54e/MAE_Comparison-checkpoint.png
















3.1 Model Performance Comparison
The models were trained and tested on the historical data. The consolidated performance results are presented below:
