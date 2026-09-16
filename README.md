# Student Performance Regression Analysis

An R-based multiple regression analysis of how study time, attendance, and peer influence are associated with student exam scores.

## Project overview

This project evaluates weekly hours studied, attendance percentage, and peer influence as predictors of exam performance. It compares an initial multiple linear regression with a model using a log-transformed exam score and examines residual behavior, autocorrelation, multicollinearity, and influential observations.

## Dataset

The project uses the [Student Performance Factors dataset on Kaggle](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors). The published dataset contains 6,607 observations and 20 variables covering study habits, attendance, family and school context, lifestyle factors, and exam performance.

The data file is not included. Download `StudentPerformanceFactors.csv` from Kaggle and place it in the repository's root directory before running the analysis. Keep the CSV out of the GitHub upload and direct users to the original source.

## Research question

How are hours studied, attendance, and peer influence associated with student exam scores?

## Selected findings

In the initial model:

- each additional weekly study hour was associated with an estimated **0.29-point increase** in exam score;
- each additional attendance percentage point was associated with an estimated **0.20-point increase** in exam score;
- neutral peer influence was associated with an estimated **0.52-point lower** score than positive peer influence; and
- negative peer influence was associated with an estimated **1.03-point lower** score than positive peer influence.

All included predictors were reported as statistically significant. The initial model had an R-squared of approximately **0.551**, while the log-response model had an R-squared of approximately **0.593**. Because the outcomes are measured on different scales, these R-squared values should not be treated as a direct predictive-performance comparison.

These findings are associations and should not be interpreted as causal effects.

## Repository contents

```text
student-performance-regression-analysis/
├── README.md
├── student-performance-regression.Rmd
├── student-performance-regression-report.pdf
├── methodology.md
└── data-dictionary.md
```

## Reproduce the analysis

1. Download `StudentPerformanceFactors.csv` from the [Kaggle dataset page](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors).
2. Place the CSV in the repository's root directory.
3. Open `student-performance-regression.Rmd` in RStudio.
4. Install the required packages if needed:

```r
install.packages(c("tidyverse", "lmtest", "car", "MASS"))
```

5. Knit the R Markdown file to HTML or PDF.

## GitHub repository description

> Multiple regression analysis of how study time, attendance, and peer influence are associated with student exam scores using R.

## Responsible use

This project is intended for educational analysis. Student performance is shaped by many observed and unobserved factors, and results should not be used to label students or make high-stakes educational decisions.

## Author

Yingqi Jiang
