# Regression Analysis on Key Factors Influencing Student Exam Scores

## Overview
This project analyzes how various factors such as study hours, attendance, and peer influence affect student exam scores. Utilizing multiple regression analysis, this study aims to understand and quantify the impact of these factors on academic performance.

## Dataset
The dataset includes variables such as Exam_Score, Hours_Studied, Attendance, and Peer_Influence, categorized into positive, neutral, and negative influences. It contains data gathered from student performance metrics.

## Regression Model
The regression model incorporates these variables to predict exam scores. The analysis includes:
- Initial and log-transformed models to address heteroscedascity.
- Diagnostic tests for autocorrelation, multicolinearity, and influential points.

## Model Equation 
Exam_Score = β0 + β1(Hours_Studied) + β2(Attendance) + β3(Peer_Influence_1) + β4(Peer_Influence_2)

## Predictors
- Hours_Studied: Continous variable indicating weekly study hours.
- Attendance: Continous variable representing attendance percentage.
- Peer_Influence: Categorical variable with levels(Positive, Neutral, Negative).

## Results
The log-transformed model improved fit and reduced heteroscedasticity, explaining approximately 59.3% of the variance in exam scores. The study highlights the significant positive impact of study hours and attendance and the negative effects of neutral or negative peer influence.

## Conclusions
The findings emphasize the importance of study habits and the environment on student outcomes. Interventions to promote effective study strategies and positive peer interactions are suggested to enhance academic performance.

## Reference
Data sourced from https://www.kaggle.com/datasets/lainguyn123/student-performance-factors/data.
