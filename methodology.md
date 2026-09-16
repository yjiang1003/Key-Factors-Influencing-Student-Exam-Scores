# Methodology

## Analytical objective

The analysis estimates the association between exam scores and weekly study hours, attendance percentage, and peer influence.

## Models

The initial model is:

```r
lm(Exam_Score ~ Hours_Studied + Attendance + Peer_Influence, data = df)
```

`Peer_Influence` is treated as a categorical predictor with `Positive` as the reference group. A second model uses `log(Exam_Score)` as the response to examine whether residual behavior improves.

## Diagnostics

- Residuals versus fitted values assess nonlinearity and nonconstant variance.
- The Durbin-Watson test checks residual autocorrelation.
- Variance inflation factors assess multicollinearity.
- Cook's distance identifies influential observations.

## Reproducibility and validation notes

The R Markdown source reads `StudentPerformanceFactors.csv` from the repository's root directory. The CSV should be downloaded from Kaggle but not included in the GitHub upload.

Recommended improvements include documenting missing-value handling and the complete-case sample size, checking the expected exam-score range, adding normal Q-Q and scale-location plots, using a formal heteroscedasticity test, and evaluating predictions through a test set or cross-validation.

The original-response and log-response models operate on different outcome scales. Their R-squared values and residual standard errors should not be compared directly as proof that one predicts better. Predictions should instead be evaluated on a common exam-score scale using metrics such as RMSE or MAE.

Findings are associative rather than causal, and practical effect sizes and confidence intervals should be considered alongside p-values.
