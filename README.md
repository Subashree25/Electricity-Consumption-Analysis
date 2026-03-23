Electricity Consumption Analysis (AI/ML Project)

This project focuses on analyzing and predicting household electricity consumption using Machine Learning techniques. It combines EDA, time-series forecasting, clustering, anomaly detection, and rule-based AI to understand usage patterns and generate insights.

Dataset
Source: UCI Machine Learning Repository
Records: 2,075,259 rows
Time Period: Dec 2006 → Nov 2010
Features:
Date
Time
Global Active Power
Global Reactive Power
Voltage
Global Intensity
Sub-metering values


Task 1 — Exploratory Data Analysis (EDA)

Missing values: 25,979 per column
Outliers detected: 14,376
Key Insights:
Peak usage: 8 PM (1.899 kW)
Lowest usage: 4 AM (0.444 kW)
Weekends (Saturday and Sunday) show higher electricity consumption than weekdays
Task 2 — Time-Series Forecasting
Train data: 27,315 samples
Test data: 6,829 samples
Model Performance:
MAE: 0.3712 kW
RMSE: 0.5213 kW
MAPE: 49.16%
Observation:

The predicted vs actual graph shows good trend alignment, meaning the model captures overall patterns effectively.

Task 3 — Unsupervised Learning
Anomaly Detection
Total anomalies detected: 20,492
Clustering Results
Cluster	Type	Days	Avg Usage (kWh/day)	Peak Time
0	High Use	671	32.43	8 PM
1	Low Use	676	18.37	9 PM
2	High Use	70	42.11	8 PM
Insights:
Most days fall into moderate or high usage categories
A small number of days show extremely high consumption patterns
Task 4 — Rule-Based AI System
Usage Classification Rules:
Low: < 0.563 kW
Medium: 0.563 – 1.620 kW
High: > 1.620 kW
Distribution:
Medium: 3,994 hours
Low: 1,800 hours
High: 1,035 hours
Suggestions:
Low Usage: Efficient usage, maintain current consumption
Medium Usage: Reduce usage during peak hours
High Usage: Use energy-efficient appliances or shift load
Example Output
Predicted Power: 1.75 kW
Category: High Usage
Suggestion: Reduce usage during peak hours to save energy
Key Takeaways
Electricity usage follows clear daily and weekly patterns
Evening hours are the most energy-intensive
Machine learning models can effectively predict trends
Clustering helps identify usage behavior patterns
Rule-based AI improves practical usability
Tech Stack
Python
Pandas, NumPy
Matplotlib / Seaborn
Scikit-learn
