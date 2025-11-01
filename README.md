# employee-turnover-analytics
📘 Employee Turnover Analytics

Author: Radiance Redefined
Role: ML Developer (HR Analytics Assignment)
Tools Used: Python, Pandas, Scikit-learn, Seaborn, Matplotlib, SMOTE, KMeans, Random Forest

🧠 Project Overview

This project focuses on analyzing employee turnover data and building machine learning models to predict which employees are most likely to leave the company. The analysis helps HR teams identify at-risk employees early and design proactive retention strategies.

The dataset is sourced from Kaggle’s HR analytics dataset, containing records for 14,999 employees of Portobello Tech with attributes like satisfaction level, last evaluation, projects handled, working hours, tenure, salary, and promotion history.

🎯 Objectives

Perform data quality checks and ensure dataset readiness.

Conduct Exploratory Data Analysis (EDA) to identify key factors influencing turnover.

Apply K-Means clustering to understand groups among employees who left.

Handle class imbalance using SMOTE.

Train and evaluate multiple ML models (Logistic Regression, Random Forest, Gradient Boosting).

Identify the best model using 5-fold cross-validation and ROC/AUC.

Predict turnover probabilities and categorize employees into risk zones.

Suggest data-driven retention strategies for each risk zone.

⚙️ Tech Stack

Python 3.12

Pandas, NumPy — data processing

Matplotlib, Seaborn — visualization

Scikit-learn — ML models (Logistic Regression, Random Forest, Gradient Boosting, KMeans)

Imbalanced-learn (SMOTE) — oversampling technique

📊 Key Findings (EDA Summary)
Feature	Observation
Satisfaction Level	Strongest negative correlation with turnover (low satisfaction → high attrition)
Number of Projects	U-shaped relation — too few or too many projects increase attrition
Average Monthly Hours	Overworked employees (250+ hours/month) more likely to leave
Promotions	Lack of promotions over 5 years correlates with leaving
🧩 Model Performance Summary
Model	Accuracy	ROC AUC	Recall (Left = 1)
Logistic Regression	0.77	0.82	0.74
Gradient Boosting	0.97	0.99	0.93
Random Forest ✅	0.99	0.99	0.98

Best Model: Random Forest Classifier
Chosen Metric: Recall — ensures maximum capture of employees likely to leave.

🚦 Risk Zone Categorization
Zone	Probability Range	Description
🟢 Safe Zone	< 20%	Loyal and satisfied
🟡 Low-Risk Zone	20–60%	Slight dissatisfaction
🟠 Medium-Risk Zone	60–90%	Burnout or stagnation risks
🔴 High-Risk Zone	> 90%	Likely to resign soon
💡 Retention Strategies
Risk Zone	Strategy
🟢 Safe	Continue engagement & skill-building initiatives
🟡 Low Risk	Introduce flexible hours and recognition programs
🟠 Medium Risk	Provide mentorship, career pathing, and fair workload distribution
🔴 High Risk	Immediate review of compensation, promotions, and management feedback
📈 Clustering Insights

K-Means clustering of employees who left revealed three behavioral groups:

Overworked High Performers: High evaluation but low satisfaction → burnout.

Disengaged Low Performers: Low satisfaction & low evaluation → need coaching.

Satisfied High Performers: Still left — likely seeking growth or new challenges.

🧾 How to Run

Clone or download the repo:

git clone https://github.com/yourusername/employee-turnover-analytics.git


Open Employee_Turnover_Analytics_Apurva.ipynb in Google Colab
 or Jupyter.

Upload the dataset HR_comma_sep.csv.

Run all cells in order (Steps 1–11).

Export the notebook as PDF for submission.

🏁 Conclusion

The Random Forest model effectively predicts employee turnover with 99 % accuracy and 0.99 ROC AUC. The insights reveal that satisfaction level, project load, and promotion frequency are the most critical drivers of attrition. The risk zone framework empowers HR leaders to act proactively and reduce turnover through targeted retention initiatives.

📄 Files in Repository
File	Description
Employee_Turnover_Analytics_Apurva.ipynb	Full notebook with analysis and code
HR_comma_sep.csv	Original dataset
README.md	Project summary and documentation
Employee_Turnover_Analytics_Apurva.pdf	Final exported report (for submission)
