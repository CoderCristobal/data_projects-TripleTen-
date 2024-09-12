Megaline Telecom Plan Revenue Analysis
Project Overview
This project aims to analyze the behavior of Megaline's clients and determine which of its two prepaid plans, Surf and Ultimate, generates more revenue. The company seeks to adjust its advertising budget based on the insights gathered from this analysis.

As an analyst, your task is to examine the data for 500 clients and assess their usage patterns across calls, text messages, and internet data. The goal is to provide a clear recommendation on which plan drives more revenue, both in total and on a per-user basis.

Project Structure
1. Introduction
The purpose of this analysis is to compare the two prepaid plans offered by Megaline, Surf and Ultimate, and determine which plan is more profitable for the company. This will allow the commercial department to allocate their advertising budget more effectively.

Key objectives:

Analyze customer behavior by studying usage patterns for calls, text messages, and data.
Calculate the monthly revenue generated from each user.
Compare the average revenue from the two plans and identify which plan brings in more revenue.
2. Data Preparation
The dataset used in this project consists of five files containing information on calls, internet usage, messages, and the plans for each user. The data was cleaned and transformed before analysis.

Key Steps:
Data Cleaning: Ensured all columns were in the correct format and handled any missing or erroneous data.
Feature Engineering:
Calculated the number of calls, messages, and data used by each customer on a monthly basis.
Computed the monthly revenue for each customer based on plan limits and additional charges for overages.
Files used:
megaline_calls.csv
megaline_internet.csv
megaline_messages.csv
megaline_plans.csv
megaline_users.csv
3. Data Analysis
In this section, we analyzed the usage data to understand client behavior and revenue generation for each plan.

Customer Usage Analysis:
Calculated the mean, variance, and standard deviation of calls, messages, and data volume for each plan.
Visualized the distributions using histograms and described key findings.
Revenue Comparison:
Calculated the total and average monthly revenue for each plan.
Analyzed the factors driving revenue, such as overage charges for Surf plan users who exceed their data limits.
Here are some visualizations that demonstrate the findings:

Figure 1: Histogram showing the distribution of calls made by Surf and Ultimate users

Figure 2: Bar chart comparing the average revenue per user for Surf and Ultimate plans

4. Hypothesis Testing
We tested two hypotheses using statistical methods to compare revenue differences:

Hypothesis 1:
Null Hypothesis (H₀): The average revenue of users from the Surf and Ultimate plans is the same.
Alternative Hypothesis (H₁): The average revenue of users from the Surf and Ultimate plans is different.
Hypothesis 2:
Null Hypothesis (H₀): The average revenue from users in the NY-NJ area is equal to the revenue from users in other regions.
Alternative Hypothesis (H₁): The average revenue from users in the NY-NJ area is different from other regions.
We used the t-test to evaluate these hypotheses and determined the significance level (alpha). The results showed statistically significant differences between the groups for both hypotheses.

5. Conclusion
From our analysis, we concluded that the Surf plan generates more total revenue due to its higher number of users. However, on a per-user basis, the Ultimate plan consistently brings in more revenue. The Surf plan’s revenue is largely driven by users exceeding their internet data limits, as minute and message overages are rare.

Recommendations for Business Improvement:
Focus advertising efforts on attracting users to the Ultimate plan, as it generates more revenue per user.
Consider restructuring the Surf plan's data package, since many users are regularly exceeding their limits, which suggests room for a more profitable data overage strategy.
Future Improvements
Here are a few ideas for future analysis and potential business improvements:

Plan Optimization: Analyze whether adjusting the data limits on the Surf plan would affect overall revenue or customer satisfaction.
Customer Retention: Investigate churn rates between Surf and Ultimate users to determine if plan features influence customer retention.
Marketing Strategy: Further segmentation of customer demographics to optimize targeted advertising for each plan.
