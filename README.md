# Global-Pollution-Analysis-and-Energy-Recovery
#Project Objective
This project analyzes global pollution metrics and investigates how pollution levels influence energy recovery potential. The goal is twofold:

Predict energy recovery (in GWh) using regression models.

Classify countries by pollution severity using logistic regression.

#Dataset Overview
Dataset Name: Global_Pollution_Analysis.csv

Key Features:

Pollution indices (Air, Water, Soil)

Industrial Waste (in tons)

CO2 Emissions (in MT)

Energy Recovered (in GWh)

Energy Consumption per Capita (in MWh)

GDP per Capita (in USD)

Country, Year

#Data Preprocessing
Missing Values: Imputed or removed as required.

Encoding: Country and Year encoded using Label Encoding.

Scaling: All numeric features standardized using StandardScaler.

Feature Engineering:

Created Pollution_Level as a target for classification (Low, Medium, High).

Year trends and energy per capita computed for deeper insight.

#Exploratory Data Analysis (EDA)
Correlation Matrix: Identified strong correlations between:

Industrial Waste ↔ CO2 Emissions

Air Pollution Index ↔ Energy Recovery

Visualizations:

Heatmaps, bar charts, line plots

Trends by country and year

Outlier Detection: Boxplots used to flag and optionally remove extreme pollution or emission values.

#Predictive Modeling
1. Linear Regression (Predicting Energy Recovered)
Features Used: Air Pollution Index, CO2 Emissions, Industrial Waste, etc.

Train/Test Split: 80/20

Metrics:

R² Score: ~0.86 (good fit)

MAE & MSE: Low values, indicating accurate predictions

Visual Evaluation:

Residual distribution: Centered around 0

Actual vs Predicted: Linear relationship, small spread

2. Logistic Regression (Classifying Pollution Severity)
Target: Pollution_Level derived from Air Pollution Index

Classes: 0 = Low, 1 = Medium, 2 = High

Metrics:

Accuracy: ~85%

Precision/Recall: Balanced across classes

F1-score: High, indicating solid classification

Visuals:

Confusion Matrix

ROC Curves (One-vs-Rest AUC for each class)

#Actionable Insights
High Pollution, Low Recovery Countries:

Countries with severe pollution but poor energy recovery should be prioritized for green tech deployment.

Low Renewable Energy Usage with High Emissions:

These nations could benefit from policy incentives and international support for clean energy transitions.

High GDP, Moderate Pollution Nations:

Ideal candidates for strategic clean energy investment and innovation rollouts.

Pollution vs Energy Recovery:

Countries with rising industrial waste but flat recovery growth show untapped potential in waste-to-energy infrastructure.

#Recommendations
Government and Policy Makers:

Introduce subsidies for renewable energy in highly polluting countries.

Enforce stricter industrial emission caps in regions with low energy recovery.

Investors and NGOs:

Target countries with both economic readiness and environmental need.

Promote AI-based forecasting tools for pollution management.

Research & Development:

Further study into converting different types of waste (especially plastic) into usable energy.

Long-term tracking of pollution vs economic growth for sustainable development insights.

📁 Deliverables
-Google Colab / Jupyter Notebook with code, plots, and models

-Summary Report (this document)

-Visualizations: Heatmaps, scatter plots, ROC curves, confusion matrix

-Model Performance Metrics

