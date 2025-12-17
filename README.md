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


Interpretation of Performance

1.	Random Forest Superiority: The Random Forest model clearly outperformed both Linear Regression and KNN for both 20t and 30t costs. An R2 of 0.9347 for the 20t tipper indicates that the model explains over 93% of the cost variability based on distance, confirming its robustness.
   
3.	MAE Significance: The Random Forest's MAE of $1.31/ton for the 20t tipper means that, on average, its prediction is only off by approximately $1.31 per ton, a highly acceptable error margin for a pricing model.
   
4. Linear Relationship Confirmation: Despite Random Forest performing better, Linear Regression still achieved a strong R^2 (above 0.84 for both), confirming a fundamental strong linear correlation between distance and the cost per ton, which is a key principle in logistics pricing.

   

Visual Analysis (Linear Regression Trend)

The scatter plots demonstrate the strong linear trend in the underlying data. The closely fitted line confirms that as distance increases, the cost per ton consistently rises.

https://github.com/TalentNcube/Logistics-pricing-analysis/blob/9fa8c7c0c82ddd39368c2338f115661c7652de9b/30t_Tipper_Linear_Regression_Plot.png

https://github.com/TalentNcube/Logistics-pricing-analysis/blob/158ead3e37ac902926c3142bbbc7bb60c2f64582/20t_Tipper_Linear_Regression_Plot.png

7. New Area Cost Prediction
The developed models were used to predict the cost per ton for a hypothetical new area with a distance of 50.0 km.







Prediction Interpretation

1.Random Forest (Recommended Price): Based on its superior performance metrics (R^2 and MAE), the Random Forest predictions are the most reliable. The suggested price for a 50 km trip would be $6.04/ton for the 20t tipper and $5.93/ton for the 30t tipper.
2.Model Variance: The discrepancy in predictions highlights the models' different approach: KNN's prediction is lower as it averages the costs of the 5 closest historical data points, while Random Forest uses a complex tree structure built on all data to extrapolate, which is generally more accurate.


Conclusion

This research successfully developed and compared three machine learning models for logistics pricing based on distance.
The Random Forest Regressor is the recommended model for real-world deployment due to its superior accuracy (highest  R^2 and lowest MAE) across both tipper capacities. Its ability to account for minor non-linear fluctuations in the distance-cost relationship provides the most reliable price estimates. The project provides a strong foundation for optimizing pricing strategies using predictive analytics, moving beyond fixed rate cards to a dynamic, data-driven approach.

















3.1 Model Performance Comparison
The models were trained and tested on the historical data. The consolidated performance results are presented below:
