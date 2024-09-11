# Telecom_customer_churn_rate_analysis
This project focuses on analyzing customer churn in a telecom company using machine learning and exploratory data analysis (EDA). The goal is to uncover key factors influencing customer churn and build a predictive model to identify at-risk customers, providing insights for churn reduction strategies.

Table of Contents
Project Overview
Data
Analysis Workflow
Results
Dependencies
Conclusion
Project Overview
Customer churn is a critical issue in the telecom industry. This project utilizes logistic regression to predict churn based on customer attributes, services, and account details. The project follows a structured process of data preparation, EDA, feature engineering, and model building to predict churn effectively.

Data
The dataset contains customer information related to account tenure, service subscriptions, charges, and churn status.

Key Columns:

tenure: The number of months the customer has stayed with the company. Longer tenure often indicates customer loyalty.
MonthlyCharges: The monthly charges for the customer's subscription. Higher charges may be associated with higher churn risk.
TotalCharges: The total amount billed to the customer.
Categorical Variables (e.g., Contract, PaymentMethod, InternetService, TechSupport, etc.): These variables represent the types of services and contracts, which greatly influence churn behavior.
Churn: The target variable indicating whether the customer churned (Yes or No).
Excluded Columns:

customerID: Unique identifier, irrelevant to churn prediction.
gender: Does not show significant impact on churn based on the analysis.
Analysis Workflow
Data Preprocessing:

Handle missing values in TotalCharges.
Convert categorical variables into numerical format using encoding techniques (e.g., One-Hot Encoding).
Exploratory Data Analysis (EDA):

Analyze the distribution of tenure, charges, and churn rates using histograms, bar charts, and box plots.
Visualize the relationship between categorical variables (e.g., Contract, InternetService) and churn with count plots and bar charts.
Investigate correlations between numeric features like tenure, MonthlyCharges, and churn using pair plots and heatmaps.
Feature Engineering:

Create additional features such as tenure groups (to categorize customers based on tenure length).
Use interactions between categorical variables and charges to improve model performance.
Model Building:

Developed a Logistic Regression model to classify churn (Yes/No).
Evaluated model performance using accuracy, precision, recall, and ROC-AUC score.
Visualization:

Developed Tableau dashboards to display key churn metrics, churn rates by customer segments, and service usage patterns.
Results
Key Drivers of Churn:
Contract Type: Month-to-month contracts have the highest churn rates.
Tenure: Shorter tenure customers are more likely to churn.
Monthly Charges: Higher monthly charges are strongly correlated with churn.
Service-related Factors: Lack of additional services (e.g., tech support, streaming services) increases churn risk.
Model Performance:
The logistic regression model achieved an accuracy of X%, with balanced precision and recall metrics, indicating its reliability for binary churn prediction.
Dependencies
To run the code and analysis, the following Python libraries are required:

pandas
numpy
matplotlib
seaborn
scikit-learn
Conclusion
This analysis provides actionable insights for predicting customer churn, with tenure, charges, and contract type being the most influential factors. The logistic regression model serves as a robust baseline for further improvement. Visualizations created in Tableau support deeper understanding of churn patterns and help guide strategic interventions for retention.

