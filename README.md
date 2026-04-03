# UNICEF Donor Response Prediction

## Project Overview
This project develops a machine learning model to predict donor responses to direct mail (DM) fundraising campaigns for UNICEF Australia. The goal is to improve donor targeting by identifying individuals who are most likely to respond to fundraising appeals.

Using historical donor behaviour and campaign data, several predictive models were developed to estimate the probability that a donor will make a donation within three months after receiving a fundraising letter.

By applying predictive analytics, this project demonstrates how data-driven decision making can help nonprofit organisations improve fundraising efficiency and maximise campaign return on investment.

## Business Problem
UNICEF Australia relies heavily on direct mail fundraising campaigns to support humanitarian programs aimed at improving children's health, education, and welfare worldwide.

However, traditional mail fundraising faces several challenges:

- Declining donor response rates
- Increasing mailing and printing costs
- Competition from digital fundraising channels
- Donor fatigue due to repeated appeals

Sending letters to donors who are unlikely to respond leads to higher operational costs and lower campaign efficiency.

Therefore, UNICEF requires a data-driven donor targeting strategy to maximise campaign effectiveness.

## Project Objective
The objective of this project is to build a propensity model that predicts whether a donor will respond to a fundraising campaign within the next three months.

The model helps UNICEF:

- Improve donor targeting
- Reduce unnecessary mailing costs
- Increase response rates
- Optimise campaign return on investment

This problem is framed as a binary classification task, where donors are classified as either:

- Likely to respond
- Unlikely to respond

## Dataset
The dataset contains historical donor and campaign information provided by UNICEF.

Key characteristics of the data include:

- Donor behavioural history
- Campaign interaction data
- Donation frequency and amounts
- Demographic attributes

The analysis focuses on individual donors in Australia and New Zealand, using campaign data from 2020–2025 to capture recent fundraising trends.

## Exploratory Data Analysis (EDA)
Initial data exploration revealed several important patterns in donor behaviour.

### Donor Response Distribution
The dataset is highly imbalanced, with significantly fewer responding donors compared to non-responders.

This imbalance highlights the importance of using evaluation metrics that account for both precision and recall.

### Donation Behaviour
Donors who responded to campaigns tended to have:

- Higher historical donation frequency
- Shorter time since last donation
- Stronger engagement with previous campaigns

### Campaign Timing
Donation likelihood was influenced by campaign timing and previous donor engagement patterns.

These insights informed feature engineering and model development.

## Feature Engineering
Several features were engineered to capture donor behaviour and campaign engagement patterns.

Examples include:

### Recency Features
- Days since last donation
- Time since previous campaign response

These features capture donor engagement recency, which is often a strong predictor of future behaviour.

### Frequency Features
- Total number of historical donations
- Donation frequency within a given time period

These indicators reflect donor loyalty and engagement level.

### Campaign Interaction Features
- Previous campaign responses
- Historical response intervals

These features help identify donors who consistently engage with fundraising campaigns.

Feature engineering plays a critical role in improving model predictive performance.

## Machine Learning Models
Three machine learning models were implemented and compared.

### Logistic Regression
A baseline model that provides high interpretability and allows stakeholders to understand which features influence donor responses.

### Random Forest
A tree-based ensemble model capable of capturing non-linear relationships in donor behaviour.

### XGBoost
A gradient boosting algorithm designed for high predictive performance and complex feature interactions.

## Model Evaluation
Models were evaluated using the F1-score, which balances precision and recall.

This metric is particularly appropriate for imbalanced classification problems where both:

- correctly identifying responding donors
- avoiding false predictions

are important.

## Model Performance Comparison

| Model | Performance |
|-------|-------------|
| Logistic Regression | Best overall performance |
| Random Forest | Strong predictive accuracy |
| XGBoost | Competitive performance |

Although more complex models were evaluated, Logistic Regression produced the most effective and interpretable results for this dataset.

## Business Impact
The predictive model enables UNICEF to adopt a data-driven fundraising strategy.

By targeting donors who are most likely to respond, UNICEF can:

- Reduce unnecessary campaign costs
- Improve donor engagement
- Increase fundraising efficiency
- Allocate resources more effectively

These improvements help maximise the impact of fundraising campaigns and support UNICEF's humanitarian mission.

## Tools & Technologies
- Python
- Pandas
- Scikit-learn
- XGBoost
- Machine Learning

## Key Takeaways
- Machine learning can significantly improve donor targeting in fundraising campaigns.
- Donor behaviour patterns such as recency and frequency are strong predictors of response likelihood.
- Interpretable models such as Logistic Regression can provide both strong performance and transparency for stakeholders.
- Data-driven campaign optimisation can reduce operational costs while improving fundraising outcomes.
