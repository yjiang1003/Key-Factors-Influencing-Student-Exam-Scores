# Key-Factors-Influencing-Student-Exam-Scores
Regression analysis on key factors influencing students' exam scores
This report analyzes factors that influence student exam scores using multiple regression
analysis. The main objective of this project is to determine the impact of Hours_Studied,
Attendance, and Peer_Influence (categorized as positive, neutral, and negative) on exam
performance. We first fit a regression model to understand the significance of these variables and
assess how well they explain variations in exam scores. We found that Hours_Studied and
Attendance seems to be strong positive predictors, while Neutral and Negative Peer_Influence
were found to negatively affect exam scores.
The initial model showed some issues with heteroscedasticity. To address this, we applied a log
transformation to the response variable (Exam_Score), leading to an improved model with better
fit and more consistent error variance. The transformed model explained approximately 59.3% of
the variation in exam scores, compared to 55.1% of the variance explained by the initial model.
Overall, the analysis provides valuable insights into academic performance and suggests where
intervention, such as promoting study habits and positive peer influences, could be effective in
improving students’ performance in exams.
The original dataset contains various factors that contribute to student performance in exams. It
includes information on study habits, attendance, family income, and etc.
We will be looking at the following key attributes:
● Exam_Score : The dependent variable measuring students’ performance in the final
exam.
● Hours_Studied: A continuous variable representing the number of hours a student spends
on studying per week.
● Attendance: A continuous variable capturing a student’s attendance in terms of
percentage.
● Peer_Influence: A categorical variable with three levels (Positive, Neutral, Negative)
indicating the influence of peers on academic performance.
