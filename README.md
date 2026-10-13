

### Part A — Inspect and Clean
I capped the outlier of 50 study hours at 12 hours to reduce its influence while preserving the student's record. I filled missing study hours with the median and replaced the invalid attendance value of -10 with median attendance. The feature matrix shape is (100, 3). The features are `study_hours`, `attendance`, and `previous_mark`. The target is `final_score`.

### Part B — Summarize
The mean, median, and standard deviation were calculated for all columns.

1. Study hours have a mean of 4.81 and standard deviation of 1.92.
2. Attendance has a mean of 85.23 and standard deviation of 9.54.
3. Final scores have a mean of 42.69 and standard deviation of 6.09.

### Part C — Visualize
The histogram shows the distribution of final scores. The scatter plot compares study hours with final scores. The correlation indicates that their linear relationship is very weak.

### Part D — Correlation and Causality
The Pearson correlation is 0.0692, indicating a very weak positive linear relationship. Studying 10 hours does not guarantee a particular score. Previous academic performance or attendance could be confounding variables.

### Part E — Vectors and Dot Product
The weights determine each feature's contribution to the prediction. The bias is added to the weighted sum to shift the result. The dot product is 46.72, and adding the bias of 5 gives a predicted score of 51.72. These are illustrative weights, not trained model parameters.

### Part F — Scaling
Standardization transforms `study_hours` and `previous_mark` to have means near zero and standard deviations near one. Without scaling, `previous_mark` could dominate KNN distance calculations because its original spread is much larger than that of `study_hours`.
