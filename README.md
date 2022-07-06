# Over-Sampling Analysis with Classification Metrics Evaluation

### Analysis of over sampling when evaluating Logistic Regression with the following metrics 

* Confusion Matrix 
* ROC and AUC Curve 
* Cross Validation 

From the analysis, I found the accuracy of the over-sampling methods is similar to imbalance data when we increase their threshold to 0.75 instead of the original 0.5.
The results were similar across the board with the confusion matrix, with the Naive Random Over-Sampling method working slightly better than the others 
The results were also similar across the board with ROC & AUC metrics. 

From the analysis, the model is not doing an efficient job in the classification, I assumed this based on the correlation and mutual information scores. 

For this study, I decided to use the Phi-k correlation rather than the correction and mutual information for numerical and categorical values. The Phi-k has the advantage to work across different variables (categorical, ordinal, and interval). It can also capture non-linear relationships (I am just learning about this but will explore more in due time) 

From the Phi-K correlation, I took the top three variables correlated with the target label. The values were 0.46, 0.45, 0.36 (quite low).
I then performed the analysis again with just these variables and came to a very similar accuracy score, which would imply that the other 16 variables do not add significant importance to the model. 

However,  from the results, the model is not that effective.


Code: https://github.com/Akiwacky/Over-Sampling-Metrics-Evaluation-
