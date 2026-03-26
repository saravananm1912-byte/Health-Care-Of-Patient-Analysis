Patient Health Data Analysis
Project Overview
This project involves the generation and analysis of synthetic patient health data. The primary goal is to understand various health metrics, classify patients into different risk categories, and derive meaningful insights that can aid in early detection of health risks, better patient monitoring, and informed healthcare decision-making.

Data Generation
Synthetic patient data for 10,000 individuals was generated using the Faker library, including:

Patient_ID
Age
Gender
Blood_Pressure
Sugar_Level
Cholesterol
Heart_Rate The data was then saved to a CSV file (patient_data.csv) and loaded into a pandas DataFrame.
Data Cleaning and Preprocessing
Inspected DataFrame information (df.info()) to check data types and non-null counts.
Confirmed no missing values (df.isnull().sum()).
Generated descriptive statistics (df.describe()) for numerical features.
Exploratory Data Analysis (EDA)
Visualizations were created to understand the distribution of various health metrics:

Histograms for Age, Blood_Pressure, Sugar_Level, Cholesterol, and Heart_Rate.
Count plot for Gender distribution.
Summary statistics for Blood_Pressure, Sugar_Level, Cholesterol, and Heart_Rate were displayed.
Patient Risk Classification
Patients were classified into 'Low', 'Medium', and 'High' risk categories based on predefined thresholds for Blood_Pressure, Sugar_Level, and Cholesterol. A Risk_Category column was added to the DataFrame, and the distribution of these categories was visualized using a count plot.

Identifying High-Risk Patients
High-risk patients were identified by filtering the DataFrame for Risk_Category == 'High', providing a count and displaying the top few entries for immediate review.

Group-based Analysis
Age Group Analysis: Patients were grouped into age bins (<30, 30-44, 45-59, 60-74, 75+). The distribution of patients by age group and the average health metrics within each age group were analyzed.
Gender-wise Comparison: Average health metrics and risk category distribution were compared across genders.
Visualizations: Count plots were generated to show risk category distribution by both age group and gender.
Relationship Between Variables
Scatter Plots: Visualizations explored relationships between:
Blood Pressure vs Age (colored by Risk_Category)
Cholesterol vs Heart Rate (colored by Risk_Category)
Box Plot: Sugar Level distribution across Risk_Category was analyzed to show the impact of sugar levels on risk.
Correlation Matrix: A heatmap was generated to visualize the correlation between all numerical health metrics (Blood_Pressure, Sugar_Level, Cholesterol, Heart_Rate).
Key Insights and Conclusions
This analysis provides valuable insights for healthcare decision-making:

Early Detection: The risk classification model helps identify high-risk patients who may need immediate attention or preventive care.
Patient Monitoring: Group-based analysis (by age and gender) highlights specific demographics that may require targeted monitoring and interventions.
Understanding Relationships: Correlations between health metrics and their relationship with risk categories can inform diagnostic processes and treatment strategies.
