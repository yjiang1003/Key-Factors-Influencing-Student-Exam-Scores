# Data dictionary

The Kaggle dataset contains 20 columns. The four variables used directly in this project are identified below.

| Variable | Type | Description | Used directly |
|---|---|---|---|
| `Hours_Studied` | Numeric | Hours spent studying per week | Yes |
| `Attendance` | Numeric | Attendance percentage | Yes |
| `Parental_Involvement` | Categorical | Level of parental involvement | No |
| `Access_to_Resources` | Categorical | Level of access to educational resources | No |
| `Extracurricular_Activities` | Categorical | Participation in extracurricular activities | No |
| `Sleep_Hours` | Numeric | Average hours of sleep | No |
| `Previous_Scores` | Numeric | Prior academic score | No |
| `Motivation_Level` | Categorical | Student motivation level | No |
| `Internet_Access` | Categorical | Whether the student has internet access | No |
| `Tutoring_Sessions` | Numeric | Number of tutoring sessions | No |
| `Family_Income` | Categorical | Family-income category | No |
| `Teacher_Quality` | Categorical | Reported teacher-quality level | No |
| `School_Type` | Categorical | Type of school | No |
| `Peer_Influence` | Categorical | Positive, neutral, or negative peer influence | Yes |
| `Physical_Activity` | Numeric | Level or frequency of physical activity | No |
| `Learning_Disabilities` | Categorical | Whether a learning disability is reported | No |
| `Parental_Education_Level` | Categorical | Highest parental education category | No |
| `Distance_from_Home` | Categorical | Distance-to-school category | No |
| `Gender` | Categorical | Student gender | No |
| `Exam_Score` | Numeric | Exam-performance outcome | Yes - response |

Definitions summarize the [Kaggle dataset description](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors). Confirm exact category labels, units, missing values, and score ranges from the downloaded CSV before extending the model.
