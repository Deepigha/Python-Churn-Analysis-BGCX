# Analysis of Power Co Client Data for Predicting Churn

This project of this analysis is to explore and understand the factors contributing to client churn in the utility sector. By identifying key trends and patterns in the data, we aim to develop predictive models to forecast customer churn and inform strategic decisions to reduce churn rates.

### Data Cleaning

Converted date columns to datetime format.
Merged datasets on common identifiers.
Handled missing values and outliers through imputation and transformation.
Exploratory Data Analysis (EDA)

### Churn Analysis:

Calculated and plotted the overall churn percentage.
Analyzed churn distribution across different sales channels, consumption patterns, and contract types.
Visualized distributions and boxplots of consumption and forecast variables to identify patterns and outliers.
Consumption Analysis:

Explored the distribution of consumption variables and their relationship with churn.
Identified highly skewed consumption data and applied log transformations to stabilize the variance.
Price Analysis:

Analyzed monthly price changes and their impact on churn.
Created features for average and maximum price changes across different periods and months.
Tenure and Contract Analysis:

Calculated client tenure and analyzed its correlation with churn.
Transformed date columns into meaningful time-based features (e.g., months active, months to end of contract).
Categorical Data Transformation:

Transformed categorical variables into binary flags and dummy variables.
Removed low-frequency categories to improve model performance.
Correlation Analysis:

Calculated and visualized correlations between features to identify multicollinearity and important predictors.
Dropped highly correlated and redundant features to streamline the dataset.
Feature Engineering
Created New Features:

Enhanced existing features by calculating differences in average and maximum prices across different periods.
Developed features to capture the impact of sudden price changes on churn.

### Data Transformation:

Applied log transformations to highly skewed numerical data.
Converted Boolean and categorical data into numerical formats suitable for modeling.
Predictive Modeling
Data Preparation:

Split the dataset into training and testing sets.
Prepared data for modeling by normalizing features and handling class imbalance.
Model Development:

Implemented a Random Forest classifier to predict churn.
Evaluated model performance using accuracy, precision, recall, and ROC-AUC metrics.
Tuned hyperparameters to optimize model performance.
### Insights
## Churn Distribution:

The overall churn rate is relatively low, but certain sales channels and contract types exhibit higher churn rates.
Consumption Patterns:

Consumption data is highly skewed, with a long tail towards higher values.
Clients with higher and lower consumption levels show different churn behaviors, indicating potential outliers.
Price Sensitivity:

Significant price changes, especially sudden increases, are strongly correlated with higher churn rates.
Clients are particularly sensitive to price changes within short periods.
Tenure and Contract Impact:

Clients with shorter tenure (less than 4 months) are more likely to churn.
The type of contract (e.g., gas vs. non-gas) influences churn behavior.
Feature Importance:

Key predictors of churn include consumption patterns, price changes, tenure, and specific sales channels.
Log-transformed consumption features and price change features are highly informative.
Conclusion
This analysis has provided valuable insights into the factors influencing client churn in the utility sector. By identifying key predictors and understanding client behaviors, we can develop targeted strategies to reduce churn rates. The predictive model developed in this study shows promising performance and can be further refined with additional data and feature engineering.

Future work should focus on:

Incorporating more granular consumption data.
Exploring additional external factors (e.g., economic indicators, weather patterns).
Implementing advanced machine learning techniques (e.g., gradient boosting, neural networks) to improve prediction accuracy.
By leveraging these insights and models, the utility company can proactively address churn, enhance client retention, and ultimately improve customer satisfaction and profitability.
