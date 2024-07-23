# Summary
This is an analysis of a Portuguese bank's direct marketing campaigns aimed at predicting client subscriptions to term deposits using the marketing campaign data. Here's a concise summary of the findings and actions:

### Objective:
The goal is to classify whether a client will subscribe to a term deposit based on various features.

### Dataset Overview:

- **Features:** Includes age, job, marital status, education, credit default, balance, loan status, contact type, last contact day and month, call duration, number of contacts, and previous campaign outcome.
- **Key Statistics:**
  - Average annual balance ranges from -8k to 100k.
  - Call durations vary significantly, with a maximum of 4918 seconds.

### Data Cleaning:

- Converted "unknown" values and -1 in 'pdays' to NaN.
- Imputed missing values in the 'contact' variable with the mode.

### Exploratory Analysis:

- **Age:** Outliers observed above age 70; data remains valid.
- **Balance:** High balances are rare but legitimate; retained for model input.
- **Subscription Rate:** Generally low at 11%, but higher for call durations over 2000 seconds.

### Key Insights:

- **Age & Balance:** Older clients and those with higher balances are more likely to subscribe.
- **Job & Marital Status:** Married individuals have a higher total number of subscriptions, but single clients are more likely to subscribe relative to their group size.
- **Call Duration:** Longer calls (over 300 seconds) are strongly associated with higher subscription rates.
- **Monthly Variation:** Subscription rates remain stable throughout the year, but non-subscription rejections peak in April and May.

### Model Evaluation:

- **Class Imbalance:** Addressed using SMOTE.
- **Objective:** Maximized recall and accuracy by finding the optimal threshold using the precision-recall curve.
- **Performance Metrics (Test Set):**
- **Precision:** 0.95 for class 0, 0.33 for class 1.
- **Recall:** 0.82 for class 0, 0.66 for class 1.
- **F1-Score:** 0.88 for class 0, 0.44 for class 1.
- **Accuracy:** 80%
- **Weighted Average:** Precision: 0.88, Recall: 0.80, F1-Score: 0.83

### Recommendations:

- Focus marketing efforts on individuals with higher bank balances, students, and retirees, especially those who are single or divorced.
- Extend conversations with potential customers beyond 300 seconds to increase subscription likelihood.

---

This concludes the analysis. The model is good in terms of recall and overall accuracy, particularly for identifying subscribers, which aligns with the business objective, it could be enhanced to better balance precision and recall, thereby improving its utility in practical scenarios. But for now, the model has been finalized and is ready for deployment based on the identified optimal threshold.

