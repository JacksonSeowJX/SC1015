# SC1015 
SC1015 Project - Premier League Dataset

## Contributions
All 3 members contributed equally to the project - Data Cleaning, Adding of new columns, Multivariate Linear Regression, Gradient Boosting Classification, Anomaly Detection (Isolation Forest), Analysis and Conclusion


# Premier League Football Betting Analysis

## Problem Statement
In the rapidly growing field of sports analytics, predictive modeling for football betting remains a domain of keen interest. The aim of this project is to analyze Premier League data to uncover insights that could inform betting strategies. Through comprehensive data cleaning, exploratory data analysis (EDA), and the application of various machine learning models, this project endeavors to provide a detailed analysis conducive to informed football betting.

## Datasets
The datasets are taken from: 
- https://www.kaggle.com/datasets/zaeemnalla/premier-league/data?select=stats.csv
- https://sports-statistics.com/sports-data/soccer-datasets/

Kaggle provides seasonal statistics from 2006-2018. Includes every club's total points, wins/losses, shots on target etc. <br>
Sports-statistics provides match statistics from 2016-2019. Includes fulltime and halftime statistics with betting odds.

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
| Machine Learning Models | Insights | Accuracy Metrics (Train) | Accuracy Metrics (Test) |
|:-----------------------:|:---------|:------------------------:|:-----------------------:|
| Linear Regression | This multivariate linear regression analysis investigates the ability to predict total football points across various seasons based on game metrics. The model consistently demonstrates high predictive accuracy, as indicated by R² values consistently above 0.90 and low Mean Squared Error (MSE) rates across all 3 test runs, confirming its robustness in both fitting and predicting data. Analysis of coefficients reveals that "goals" and "clean sheets" significantly boost total points, while "goals conceded" detrimentally impacts them. In contrast, "total scoring attempts" and "corners taken" have a more ambiguous influence, suggesting a potential complexity in their relationship with total points that may require deeper exploration. Overall, the model's reliable performance across different seasonal splits, combined with its consistent alignment with the line of perfect prediction in graphical representations, underscores its effectiveness in forecasting team performance based on historical data. | R²: 0.9387, 0.9377, 0.9406 <br>MSE: 17.6396, 17.5724, 17.2457 | R²: 0.9381, 0.9702, 0.9488 <br>MSE: 16.6215, 12.0802, 12.2975 |
| Classification | The decision tree analyses conducted across three Premier League seasons consistently emphasize the significance of halftime results, especially away leads, in predicting full-time outcomes. While the model shows reasonable accuracy in predicting home and away wins, it notably struggles with draws, which are frequently misclassified as wins. This highlights a potential area for improvement, particularly in enhancing the model's ability to distinguish draws by possibly integrating more granular halftime statistics like shots on target or possession percentages. Additionally, preliminary results suggest that incorporating pre-match betting odds could significantly boost accuracy; however, this was not pursued further due to potential concerns of overfitting. Overall, the analyses suggest that while the model forms a solid base for predicting match outcomes using halftime data, further enhancements could be made by expanding the feature set to capture more nuances of the game, potentially improving predictions and the model's overall efficacy. | 64.14%, 61.84%, 64.47% | 65.79%, 57.89%, 68.42% |
| Anomaly Detection | wewerwer | --------- | --------- |


## Conclusion
The analysis not only provides a predictive framework for football betting but also highlights the importance of integrating qualitative insights into quantitative models. The project emphasizes the potential utility of halftime statistics and pre-match odds as predictive features and opens avenues for future research in enhancing model robustness and accuracy.
