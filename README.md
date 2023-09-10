# HR-Analytics

## Problem Statement

Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.

For example, you may pay a premium of Rs. 5000 each year for a health insurance cover of Rs. 200,000/- so that if, God forbid, you fall ill and need to be hospitalised in that year, the insurance provider company will bear the cost of hospitalisation etc. for upto Rs. 200,000. Now if you are wondering how can company bear such high hospitalisation cost when it charges a premium of only Rs. 5000/-, that is where the concept of probabilities comes in picture. For example, like you, there may be 100 customers who would be paying a premium of Rs. 5000 every year, but only a few of them (say 2-3) would get hospitalised that year and not everyone. This way everyone shares the risk of everyone else.

Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

Now, in order to predict, whether the customer would be interested in Vehicle insurance, you have information about demographics (gender, age, region code type), Vehicles (Vehicle Age, Damage), Policy (Premium, sourcing channel) etc.


## The Data

Variable | Description
----------|--------------

- employee_id: Unique ID for employee
- department: Department of employee
- region: Region of employment (unordered)
- education: Education Level
- Gender: Gender of Employee
- recruitment_channel: Channel of recruitment for employee
- no_of_trainings: no of other trainings completed in previous year on soft skills, technical skills etc.
- age: Age of Employee
- previous_year_rating: Employee Rating for the previous year
- length_of_service: Length of service in years
- KPIs_met: >80% if Percent of KPIs(Key performance Indicators) >80% then 1 else 0
- awards_won?: if awards won during previous year then 1 else 0
- avg_training_score: Average score in current training evaluations
- is_promoted: (Target) Recommended for promotion


## Table of Content

- **Hypothesis Testing**

Hypothesis Testing is the first step we take towards understanding the data. Hypothesis Testing gives us the head-start towards understanding the problem.

- **EDA**
<!-- ![](/images/Wholedata.png) -->
![](/images/Heatmap.png)
![](/images/Dep_piechart.png)
![](/images/Education_barplot.png)
![](/images/Rating_violinplot.png)
![](/images/KPI_stackedplot.png)


**Feature Engineering**
![](/images/Age_label_plot.png)
![](/images/Length_service_label_plot.png)

- **Model Building**

![](/images/Logistic_Regression_Before_Balancing.png)
![](/images/model_comparison.png)
![](/images/Multi_model_ROC-AUC Curve.png)

- **Final Submission**

For Final Submission I choose Voting Classifier with soft voting which gave me f1-score of 0.93 as private score and 0.44 as public score.
