# MegaLines Telecom Customer Analysis

**Table of Contents**
- [Introduction](#introduction)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Statistical Methods](#statistical-methods)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contact](#contact)

## Introduction

Welcome to the MegaLines Telecom Customer Analysis project! In this analysis, we delve into the usage and charges of 500 customers from 2018 to assist the marketing team in determining the profitability of MegaLines Telecom's two plans: 'Surf' and 'Ultimate.' Our goal is to uncover valuable insights into the effectiveness of each plan and guide future marketing decisions.

## Data Preprocessing

The data for this project was received in four tables: User data, Plan data, Call data, and Internet Data. While the data was mostly clean, some adjustments were necessary. Specifically, the 'churn_date' column had missing values for current customers without an end date. To address this, we assigned these customers an end date as the most recent date in the table. Additionally, we created two new columns: 'Month' extracted from the churn date and a 'State' column.

## Exploratory Data Analysis (EDA)

Our primary question in this analysis was, "Which of the two plans, 'Surf' or 'Ultimate,' is more profitable?" To answer this, we started by examining the average monthly costs: Surf ($72.04) and Ultimate ($71.68). Surprisingly, Surf customers pay, on average, 2.5 times more in overage fees than the base service cost ($20). To illustrate this finding, we created Figure 1.1 - Customer Vs. Revenue Shares.


![Figure 1.1 - Customer Vs. Revenue Shares](https://github.com/metanameEricRoss/MegaLines_Project/assets/89555796/bc987bfc-ede7-4cc0-b318-a08e3efb146d)

The above figure reaffirms our findings, with Surf contributing over half of the overall revenue (63.8%). To further understand the distribution of customer costs, we created a bar chart showing the average monthly cost for each plan (Figure 1.2 - Avg Monthly Cost).

![Figure 1.2 - Avg Monthly Cost](https://github.com/metanameEricRoss/MegaLines_Project/assets/89555796/a199bbb4-8a63-43df-9020-d32365018a54)

As shown in the chart, more than half of Surf customers pay more than the monthly cost, with some paying up to 10 times the base price. Ultimate customers, on the other hand, tend not to incur as many overage fees on average. We also analyzed the composition of overage fees, depicted in Figure 1.3 - Overage Fees.

![Figure 1.3 - SurfOverage Fees](https://github.com/metanameEricRoss/MegaLines_Project/assets/89555796/e6bb4f5b-2320-4b92-a889-fea8dd4a745f)

![Figure 1.4 - Ultimate Overage Fees](https://github.com/metanameEricRoss/MegaLines_Project/assets/89555796/cac1e684-ef8a-4e98-8400-cdeb92c17506)


The majority of overage fees are related to data usage for both plans, with Surf also incurring overage fees for minutes. Examining churn rates by plan (Figure 1.4 - Churn by Plan), we found that both plans have low churn percentages, with Surf at (~1.49%) and Ultimate at (~1.19%). However, Surf has a higher churn rate, indicating a slightly higher risk of losing customers despite higher profits.

## Statistical Methods

Following EDA, we conducted two statistical tests using a student-t test to determine if the two factors statistically vary based on mean and variance. Both tests used an alpha threshold of 0.05, the standard for a general test.

## Results

After thorough data analysis, we recommend focusing marketing efforts on the Ultimate plan, particularly for customers who heavily use data. This recommendation is based on two key factors:

1. **Customer Base**: The Surf customer base is more dispersed, making it less reliable when considering the addition of new customers. In contrast, the Ultimate plan brings in nearly the same average monthly charge per customer, making it easier to monitor and predict quarter to quarter.

2. **Churn Rate**: While both plans have low churn rates, Surf has a significantly higher churn rate than the Ultimate plan. This suggests that while Surf may generate slightly more revenue per user on average, it comes with a higher risk of customer churn.

## Conclusion

In summary, the Surf plan appears to generate similar revenue per user on average but carries a higher risk of churn and greater variability in user spending compared to the Ultimate plan. These insights can guide marketing efforts and help MegaLines Telecom optimize its advertising resources.

## Contact

For any questions or collaboration opportunities, please feel free to contact us at [08cire.eric99@gmail.com](mailto:08cire.eric99@gmail.com).
