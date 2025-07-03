# PredictingDiabetes

For my IST 418: Big Data Analytics project, we had to use PySpark to create a machine learning model that we could use to help solve a problem. My group and I decided we wanted to build a model that would be able to predict if a person had diabetes based on general health metrics and additional factors such as education level or income. 

## About the Data
This data was taken from the CDC Diabetes Health Indicators dataset which we accessed through the University of California - Irvine (UCI) Machine Learning Repository.

[UCI-Machine Learning Repository - CDC Diabetes Health Indicators](https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators)


## Model Performance Summary
The best model that we chose to submit was our Gradient Boosting Tree. 

Results Metrics: 
- **AUC:** `0.8272` — Strong performance in distinguishing diabetic vs. non-diabetic individuals.
- **True Negatives (42,897):** Correctly identifies most non-diabetic cases.
- **False Positives (786):** Occasionally predicts diabetes when it’s not actually present.
- **False Negatives (5,937):** Misses some diabetic individuals — a common trade-off in boosting models.
- **True Positives (1,118):** Correctly detects many true diabetes cases.

**Insight:** GBT delivers the best performance among all models, handling feature interactions and nonlinearity well. There's still a risk of underdiagnosing some cases (false negatives).