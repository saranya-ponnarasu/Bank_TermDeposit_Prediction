# Predicting Bank Term Deposit Subscriptions

### Problem Statement:

Perform data cleaning and exploratory analysis on the bank marketing dataset from a Portuguese banking institution. Analyze the data to develop a Decision Tree model that predicts whether a client will subscribe to a term deposit based on various features.

### Objective:

To build a predictive model for term deposit subscriptions by performing data cleaning, exploratory data analysis (EDA), and hyperparameter tuning. The goal is to develop a high-performing model optimized to achieve the best possible recall and accuracy.

### Libraries Used:
- **Numpy:** For data manipulation and handling missing values.
- **Pandas:** For data manipulation and cleaning.
- **Matplotlib:** For data visualization.
- **Seaborn:** For data visualization.
- **Scikit-learn:** For building and evaluating machine learning models.

### Steps Involved:

1. Importing the Libraries
2. Importing the Dataset
3. Data Understanding
   - Description of dataset features and their definitions.
   - Initial exploration of data distribution and statistics.
4. Data Cleaning
   - **4.1. Handling Missing Values - Dropping:** Dropping rows or columns with excessive missing values.
   - **4.2. Handling Missing Values - Imputing:** Imputing missing values with appropriate methods (e.g., mode for categorical variables).
   - **4.3. Outliers :** Finding the outliers in the data and treating them appropriately
5. **Exploratory Data Analysis**
   - 5.1. Bivariate analysis
   - 5.2. Multivariate analysis
     - Recommendation
6. **Data Preparation for Modeling**
   - **6.1. One-Hot Encoding :** Encoding categorical variables.
   - **6.2. Label Encoding :** Encoding categorical variables.
   - **6.3. Train-Test Split :** Spliting the data for training and test purposes.
   - **6.4. Resampling Class_Imbalance :** Identifying the class imbalance in the training data.
     - 6.4.1. SMOTE Algorithm
7. **Building decision Tree**
   - 7.1. Visualizing Decision Tree
   - 7.2. Hyperparameter Tuning using GridSearchCV
   - 7.3. Precision-Recall Curve
8. **Evaluating the Model**
   - Prediction and Metrics
9. **Conclusion**
