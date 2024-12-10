# Increasing Average Estimated Employee Value for IBM Employees

## Dataset
Dataset is a sample set of IBM employees including employees who have left the company as well as stayed with the company.

It contains important columns like:
1. PercentSalaryHike
2. PerformanceRating
3. YearsAtCompany
4. TotalWorkingYears
5. Attrition
6. DistanceFromHome

## Objectives
1. Design a metric Estimated Employee Value to quanitfy the performance, satisfaction and work experience of IBM employees.
2. Design retention strategies for IBM Employees by using Random Forest Classifier, incorporating Estimated Employee Value as a key metric.
3. Develop strategies for awarding transportation allowance incentives for high performers.
4. Estimate optimum promotion timeline using Survival Analysis and Satisfaction Score as a metric to improve job satisfaction.

## Methodology
### Employee Lifetime Value
Employee Lifetime Value(ELV) is a metric used to quantify the total value an employee brings to a company over the duration of their employment.
### Estimated Employee Value
Estimated Employee Value(EEV) is an adaption of Employee Lifetime Value(ELV). It is the ELV at a particular point of time for an employee.

This metric is designed based on a weighted average of following factors
1. Work Experience
2. Performance
3. Job Satisfaction

### Predicting Attrition
A Random Forest Classifier model was trained to predict attrition based on the given sample set. This model can be used to predict attrition of IBM Employees.

### Coupling EEV and Attrition
The employees can be segmented into three bands
1. High EEV
2. Medium EEV
3. Low EEV
Based on these the cost of attrition for each employee was calculated taking his monthly salary and an appropriate multiple inot account.

Employee Retention strategies can be designed based on the Cost of Attrition and business strategy.

### K-Means Clustering
K-Means Clustering was used to determine what separated the high performers from the low performers.

**Distance from Home** was found to be a key variable. A strategy was designed based on greedy and maximal approach to give transportation allowance as an incentive to improve the performance of low performers.

### Satisfaction Score and Optimum Promotion timeline
Satisfaction Score was derived as a metric to assess employee satisfaction. This satisfaction score was found to be inherently linked to promotion. Employee satisfaction decreased if promotions were not awarded at optimum time. 

Survival Analysis and Satisfaction score was used to determine optimum time of promotion.
