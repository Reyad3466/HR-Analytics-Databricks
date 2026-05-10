Project HR_Analytics

1. Project Objective
The main goal of this project is to analyze employee data to understand why people leave the company. By using machine learning, we can predict which employees are likely to resign, allowing the HR department to take action and improve retention rates.
2. Data Processing and Cleaning
The dataset was processed using PySpark in a Databricks environment. I started by removing columns that don't add value to the analysis, such as EmployeeCount and Over18. Categorical data was converted into numerical values to make it compatible with the machine learning models.
3. Feature Engineering
To get better results, I created three new indicators:

* Engagement Score: An average of different satisfaction levels to see how happy the employee is overall.
* Stress Indicator: A flag for employees who work overtime and have a poor work-life balance.
* Promotion Risk: Identifies high-performing employees who haven't been promoted in more than three years.

4. Machine Learning Models
I implemented two types of models for this project:

* Classification: I used Random Forest and Logistic Regression to predict the attrition. The Random Forest model performed the best with an accuracy of around 88%.
* Clustering: I used the K-Means algorithm to group employees into three different categories based on their income and job satisfaction, which helps in identifying "at-risk" groups.

5. Final Results and Insights
The analysis showed that the most important factors leading to resignation are:

* Monthly Income: Lower-paid employees are more likely to leave.
* Overtime: Working long hours is a very high predictor of attrition.
* Age: Younger employees tend to change jobs more frequently than senior staff.

6. How to Use This Project

* Download the .ipynb file and the HR_Dataset.csv.
* Import the notebook into your Databricks workspace.
* Upload the dataset to your DBFS or Catalog.
* Run the cells to see the full analysis, visualizations, and model performance.
