# LP2_CLASSIFICATION-PROJECT
# Customer Churn Prediction Project 

## Introduction

This repository contains a machine learning project focused on predicting customer churn for  Network Service provided. The project aims to analyze the probability of customers leaving the organization, identify crucial indicators of churn, and propose actionable retention strategies.

## Hypotheses

### Null Hypothesis:
The monthly subscription cost has no significant effect on customer churn from the Safari Network Service.

### Alternative Hypothesis:
The monthly subscription cost has a significant effect on customer churn from the Safari Network Service.

## Analytical Questions

1. Do senior citizens have a higher or lower likelihood of churning compared to non-senior customers?
2. What is the relation between gender in predicting churn?
3. What is the distribution of churn across different types of contracts (Month-to-month, One year, Two years)?
4. How does the tenure of customers relate to the likelihood of churn?
5. How does the method of payment impact customer churn?

## Data Understanding

### Libraries Used
- `pyodbc`: for connecting to a SQL Server database.
- `dotenv`: for loading environment variables from a .env file.
- `pandas`, `numpy`: for data manipulation and analysis.
- `seaborn`, `matplotlib`: for data visualization.
- `scikit-learn`: for machine learning tasks.
- `imbalanced-learn` (`imblearn`): for handling imbalanced datasets.

### Data Loading
1. Two datasets were loaded from a SQL Server database using `pyodbc`.
2. Another dataset was loaded from an Excel file.

### Exploratory Data Analysis (EDA)
1. Combined the first and second datasets using `pd.concat`.
2. Checked for missing values, duplicated rows, and unique values.
3. Descriptive statistics and distribution visualizations were performed.
4. Detected and addressed data issues such as standardizing categorical values.

## Data Cleaning and Preprocessing

1. Dropped the 'customerID' column.
2. Standardized categorical values for consistency.
3. Converted 'TotalCharges' to float and handled non-convertible values with NaN.
4. Converted 'SeniorCitizen' to object.
5. Performed univariate analysis and checked for outliers.
6. Inspected the distribution of categorical variables.

## Bivariate and Multivariate Analysis

1. Explored relationships between churn and numerical variables using kernel density plots.
2. Investigated the impact of gender, contract type, tenure, and payment method on customer churn.
3. Conducted multivariate analysis through pair plots and correlation matrices.

## Answering Analytical Questions

1. Explored the likelihood of churn among senior and non-senior customers.
2. Analyzed the relationship between gender and churn.
3. Investigated the distribution of churn across different contract types.
4. Explored the impact of tenure on the likelihood of churn.
5. Examined how the method of payment influences customer churn.

## Hypothesis Testing

1. Tested the hypothesis regarding the significant effect of monthly subscription cost on customer churn using an independent two-sample t-test.

## Data Preparation

1. Split the dataset into features (X) and target variable (y).
2. Split the dataset into training and evaluation sets.
3. Conducted feature processing and engineering using pipelines for numeric and categorical features.

## Recommendations

1. Senior citizens show a higher likelihood of churning, indicating the need for targeted retention strategies for this demographic.
2. Gender has a relatively balanced impact on churn, with slightly higher churn observed among male customers.
3. Customers with month-to-month contracts are more likely to churn compared to those with longer-term contracts.
4. The early months of tenure see a higher churn rate, emphasizing the importance of customer retention efforts during this period.
5. Electronic check users have a higher churn rate, suggesting the need for improving the user experience or offering alternative payment methods.

## Future Work

1. Further investigate the reasons behind the observed churn patterns.
2. Explore additional features that might contribute to churn prediction.
3. Experiment with different machine learning models and hyperparameter tuning for improved predictive performance.
4. Implement a feedback loop to continually update and improve the model based on new data.

## Acknowledgments

This project was conducted as part of a churn analysis in the Azubi Africa Data Analytics course. The  analysis was performed by [Angella_Nakkungu].

## License

This project is licensed under the [Angella_Nakkungu] License - see the [LICENSE](LICENSE) file for details.