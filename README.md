# SC1015 
SC1015 Project - Premier League Dataset


# Premier League Football Betting Analysis

## Problem Statement
In the rapidly growing field of sports analytics, predictive modeling for football betting remains a domain of keen interest. The aim of this project is to analyze Premier League data to uncover insights that could inform betting strategies. Through comprehensive data cleaning, exploratory data analysis (EDA), and the application of various machine learning models, this project endeavors to provide a detailed analysis conducive to informed football betting.

## Datasets
The datasets is taken from: 
- https://www.kaggle.com/datasets/zaeemnalla/premier-league/data?select=stats.csv
- https://sports-statistics.com/sports-data/soccer-datasets/

## Data Cleaning
The initial phase of the project involves rigorous data cleaning to ensure the quality and integrity of the datasets. This process includes:

Handling missing values by imputation or removal.
Ensuring consistency in data types across columns.
Filtering relevant features from a wide array of statistical data while excluding data that could lead to potential leakage.
Exploratory Data Analysis (EDA)
A crucial step preceding any modeling, EDA in this project involves:

Visualizing key statistical distributions through histograms and boxplots to understand the distribution of goals, shots, and other relevant match statistics.
Using correlation matrices to identify potential predictive relationships between features.
Machine Learning Models
Three primary machine learning approaches are employed:

## Multivariate Linear Regression
Utilized to forecast end-of-season points based on various in-match statistics.
Interpretation of regression coefficients to quantify the impact of different features on the total points accrued by a team.

## Classification
Prediction of Full-Time Results (FTR) using halftime data.
Employment of decision trees to discern the features that most significantly influence match outcomes.
Assessment of model performance through accuracy rates and confusion matrix analysis.

## Anomaly Detection
Application of Isolation Forest to detect outlier seasons that deviate significantly from a team’s typical performance.
Linking anomalies to notable events such as managerial changes or other off-pitch factors that may influence on-pitch results.

## Project Insights
The half-time score is a significant predictor of the full-time result.
Challenges in accurately predicting draws, indicating potential for further feature engineering.
Anomalies in team performance aligned with key events like managerial changes, providing a qualitative overlay to the quantitative analysis.

## Conclusion
The analysis not only provides a predictive framework for football betting but also highlights the importance of integrating qualitative insights into quantitative models. The project emphasizes the potential utility of halftime statistics and pre-match odds as predictive features and opens avenues for future research in enhancing model robustness and accuracy.
