# Problem Statement

The primary objective of this project is to analyze and predict the default risk of credit card clients. Specifically, the task is to determine the factors that influence whether a client will default on their credit card payment in the next month and make a prediction for future clients with similar features. The target variable in this dataset is default payment next month, which indicates whether a customer has defaulted or not.
 
The notebook starts with loading the dataset and performing an initial inspection, including displaying the first few rows of data and identifying binary columns to check imbalances.
- Descriptive Statistics: Summary statistics are calculated to understand the distribution and central tendencies and spread of the features.
- Missing Values: None

Visualization:
- Target Variable Distribution: The distribution of the target variable (default payment next month) is visualized using a count plot to understand the balance of the classes.
- Correlation Matrix: A correlation matrix heatmap is plotted to identify relationships between features and the target variable.
- Scatter Plots: Scatter plots of bill amounts and payment amounts over time are created to visualize patterns and relationships between these features and the target variable.
- Box Plots: Box plots are used to visualize the distribution of credit limits by education level and marital status, segmented by default status. This helps in identifying potential      differences in default rates across different demographic groups.
- Outlier Analysis: Outlier treatment is applied to handle extreme values that could skew the analysis and model performance.

Feature Engineering:

- Handling Outliers: A function is defined to identify and remove outliers based on a specified threshold (mean ± 3 standard deviations). This step is crucial to ensure that the model is not adversely affected by extreme values. Dimensionality reduction approaches will also be evaluated to confimr if it will improve the overall performance of the model.
- Standardization: The dataset consist of features that contain short ranges and long ranges that can potentially affect the performance of the model, we will attempt to confirm this difference by running models with model scaled features and non-scaled features as well.
- Imbalance: The target class has a large imbalance. An approach to address this issue is to using SMOTE incase our model does not learn with new data during testing.

Justification:

- The process of understanding the data, visualizing key relationships, handling data quality issues such as outliers, and preparing the data for modeling are key components to buiding any predictive model. By exploring the dataset thoroughly and visualizing different aspects of the data, the analysis can uncover important patterns and relationships that will inform the modeling process. Handling outliers ensures that the model is robust as well as properly splitting and training the data, along with it's corresponding hyperparameter tuning, class imbalnce and standardization will be fundamental for the perfromance of our model.
