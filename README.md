#     HR Analytics and Employee Attrition Insights at Wipro

![WhatsApp Image 2025-05-11 at 2 31 28 AM](https://github.com/user-attachments/assets/f2113469-d44e-441b-a377-0a572fcbf419)



The HR Wipro dataset includes information on 100 employees, detailing their department, tenure, age, and satisfaction ratings across key areas such as compensation, career growth, work-life balance, and job role. It also captures additional factors like location, remote work policies, market trends, and company performance. This dataset is instrumental in analyzing employee experiences and organizational patterns.

The project was completed in three phases:

1) Data Cleaning

2) Data Analysis

3) Visualization and Conclusion


Tools Used:

1) Microsoft Excel

2) MySQL

3) Power BI

# Data Cleaning:
![1  only Data set photo](https://github.com/user-attachments/assets/66265f53-cdf7-4ff6-8086-509656c93519)

![2  No duplicates](https://github.com/user-attachments/assets/69cf8635-f4e2-4d83-8e94-29df8bfe2afd)

* Implemented advanced data cleaning processes to identify and remove duplicate entries, standardizing the data.
* Employee ID is a unique value and observed no duplicate values entered .

* The dataset’s column headers were updated for better clarity and readability. Abbreviations and lowercase names were replaced with standardized, properly formatted titles like Employee ID, Start Date, Compensation & Benefits, and Company Performance to ensure consistency across the dataset.

![3  Start date end Date change ](https://github.com/user-attachments/assets/38a11407-d808-461a-9e06-97aebe1e5f3f)

![4  Start date end Date change ](https://github.com/user-attachments/assets/2fb0010a-afa3-4442-b57b-a441a414b76d)

* Updated Start date and end date data type from date time to only date 

![5  update teanur detail](https://github.com/user-attachments/assets/5c379d06-b6b8-48da-ae66-89e79e450673)

![6 rename and update tenure detal as round figure](https://github.com/user-attachments/assets/2c3ccf97-aef3-48b1-9ce2-6b5acc201304)


It was observed that the tenure was not accurately calculated based on the Start Date and End Date. A custom column should be created to correctly compute the tenure and replace the existing Tenure column.


## Data Analysis

Create date base as Wipro in my SQL and import the table as well.

![7 create wipro dtabase   insert tanle in SQL](https://github.com/user-attachments/assets/83a987ea-a2a2-4977-85fb-8aecbf9c4e36)


The dataset has 100 records and 14 columns, covering:
* Employee details: Employee ID, Department, Start_Date, End_Date, Tenure, Age, Location
* Work & satisfaction metrics: Compensation & Benefits, Career Growth & Promotions, Work Life Balance, Job & Work Role
* Policies and external factors: Remote Work Policy, Market Trends, Company Performance
All the rating columns (Compensation & Benefits, Career Growth & Promotions, etc.) seem numeric (likely 1–5 scale).

## Demographics 

* Age distribution

The dataset was analyzed based on employee ages, which ranged from 22 to 60 years. Employees were grouped into custom age brackets using a CASE structure: 22–31, 32–41, 42–51, and 52+, and employee counts were calculated for each group.

![7  Age groub distribution](https://github.com/user-attachments/assets/96bd5df2-3f57-4222-a0c9-8ebb698e043d)


* Department distribution

The employee distribution was analyzed across eight departments: Finance, HR, IT, Marketing, Operations, R&D, Sales, and Support. It was observed that the majority of employees work in the HR department. Additionally, the percentage of employees in each department was calculated to better understand departmental representation.

![8 0Deparment Distribution%](https://github.com/user-attachments/assets/68e978bf-9990-4e67-a0d4-bae2c57dd454)

![8 0Deparment Distribution](https://github.com/user-attachments/assets/26cdf865-a7f0-4633-91c9-9e3db3e4b699)

* Location distribution

Employee distribution was analyzed across seven locations: Hyderabad, Bangalore, Kolkata, Pune, Mumbai, Chennai, and Delhi. It was observed that the majority of employees are from Hyderabad and Bangalore, while Kolkata and Pune have an equal number of employees.

![9 0location Distribution](https://github.com/user-attachments/assets/f78fc92b-8913-41da-881d-e532ad91ca3e)


## Employee Retention

* Tenure analysis

The tenure of each employee was calculated along with the corresponding employee count. Among the 100 employees, the maximum tenure recorded is 9 years, with only one employee having this tenure, based in Pune.
On the other hand, employees with the least tenure (less than one year) are distributed across locations as follows:

Delhi: 1 employee

Hyderabad: 1 employee

Kolkata: 5 employees

Mumbai: 2 employees

Pune: 5 employees

![10  Tenure analysis ](https://github.com/user-attachments/assets/04ea7bdd-63da-48b5-9043-3bf33ee190a0)


## Employee Behavior and Satisfaction

* Compensation & Benefits

The dataset records salary-related information as ratings from 1 to 5. Analysis was primarily conducted by comparing salary ratings across departments and tenure. It was observed that only 17 employees achieved a salary rating of 5 or higher.

![12  Compensation   Benefits](https://github.com/user-attachments/assets/36540173-8760-406a-be34-9c2fae770ba4)


* Career Growth & Promotions Time to promotion. 

The dataset captures promotion timelines through a rating system ranging from 1 to 5. Analysis showed that only 14 employees achieved a promotion rating of 5 or higher, indicating faster career progression for this group.

![13  Career Growth   Promotions Time to promotion](https://github.com/user-attachments/assets/b95eb91f-6ba1-4daa-ae57-b517594b21ce)


* Work Life Balance

The dataset uses a rating scale from 1 to 5 to represent attrition-related factors. Analysis revealed that only 21 employees achieved an attrition-related rating of 5 or higher, suggesting strong retention among this group. Additionally, the average tenure was calculated to assess overall employee stability.

![14  Work Life Balance](https://github.com/user-attachments/assets/0c9290dd-2881-4731-b9a0-7d2cde71b2f9)

		
		
* Job & Work Role

Attrition was analyzed across different job roles using a rating scale from 1 to 5. It was found that only 17 employees achieved an attrition-related rating of 5 or higher, indicating lower attrition among certain roles.

![15  Job   Work Role](https://github.com/user-attachments/assets/fd449cfd-4523-4bc7-91b6-838fc61324eb)


* Correlations between satisfaction scores and tenure/attrition

0–1 Year Employees:

Moderate satisfaction across all areas, slightly positive about work-life balance and job roles.

2–3 Year Employees:

Growing dissatisfaction, especially with work-life balance and job roles, though career growth is seen as improving.
High attrition risk in this group.

4–6 Year Employees:
Low satisfaction with compensation and career growth, but a notable improvement in work-life balance.


New joiners are quite happy.
After 2–3 years, people feel a bit stuck (especially in career growth and pay).
Long-stayers (4–6 years) enjoy better work-life balance but are less happy with salary and promotion opportunities.

![16 Correlations between satisfaction scores and tenure,attrition](https://github.com/user-attachments/assets/f3ea35ab-0ae1-4b59-8ba2-ceb4bf80ebb3)



* Compare satisfaction/tenure between On-Site, Hybrid, and Remote workers

Fully Remote: 

Moderate variability, with a slight decline in the last value. It shows some instability compared to the others.

Hybrid: 

High performance at the start, with a minor drop towards the end, still relatively strong compared to others.

On-Site: 

High initial value that decreases steadily, suggesting decreasing performance or effectiveness in on-site environments.


![17  Compare satisfaction-tenure between On-Site, Hybrid, and Remote workers](https://github.com/user-attachments/assets/1ebf253c-5267-46a8-8e16-3a9db3d43e5f)



* Effect of Market Trends (Growing vs. Declining) on employee satisfaction and retention

Declining: 

This category has the lowest average and shows a decline, especially in the last value.

Growing: 

Shows an overall increase but with some fluctuations, peaking at 3.5588.

Stable: 

Consistently maintains values close to 3, representing steady or stable conditions.

Overall, "Growing" shows progress, "Declining" indicates deterioration, and "Stable" represents consistency.

![18 Effect of Market Trends (Growing vs  Declining) on employee satisfaction and retention](https://github.com/user-attachments/assets/a2a503bc-f384-45e3-848d-955ffbcdd145)

*	Company Performance perception vs. employee behaviour

Average: Shows a moderate trend with slight variability but no extreme highs or lows.

Below Average: Starts well but steadily declines, reflecting poorer performance.

Excellent: While showing potential excellence, the values fluctuate sharply, indicating inconsistent performance.

Good: Exhibits strong performance, especially in the middle, with only minor declines.

Poor: Starts well but ends with a sharp decline, indicating poor performance overall.

![18 Effect of Market Trends (Growing vs  Declining) on employee satisfaction and retention](https://github.com/user-attachments/assets/8f03053a-98d2-48d1-83bb-62b720962fca)


## Conclusions:-

This project provides a comprehensive analysis of Wipro's employee data, offering valuable insights into employee satisfaction, retention patterns, and organizational dynamics. By cleaning, analyzing, and visualizing the data, key trends and areas for improvement have been identified that can significantly contribute to enhancing employee engagement and retention within the company.



## Key Observations:

* Employee Demographics and Department Distribution:

The largest concentration of employees is within the HR department, highlighting the importance of HR practices in employee management and retention strategies.

Location-wise, the majority of employees are located in Hyderabad and Bangalore, suggesting that these locations may be strategic hubs for Wipro’s operations.

* Retention and Tenure:

Employees with less than 1 year of tenure are more likely to leave, suggesting that retention strategies should focus on improving the early employee experience.

Long-tenured employees (4–6 years) showed better work-life balance but were less satisfied with their compensation and career growth opportunities. This indicates a potential risk of dissatisfaction and turnover as employees stay longer.

Employees with 2–3 years of tenure exhibit growing dissatisfaction, particularly with work-life balance and job roles, highlighting a critical period where retention strategies need to be intensified.

* Work Environment Impact:

Hybrid Work: Hybrid employees demonstrated the highest levels of satisfaction, suggesting that flexibility is a key factor in boosting employee morale and retention. This could be a critical area for Wipro to expand and optimize.

Remote Work: Remote employees showed moderate satisfaction, with some instability in their ratings. This implies that remote work policies might need improvement in areas such as communication, career development, and employee engagement.

On-Site Work: On-site employees had a steady decline in satisfaction, indicating potential dissatisfaction with the on-site work environment. Wipro could explore ways to improve the on-site experience, particularly in the areas of compensation and career growth.

* Employee Satisfaction:

Compensation & Benefits: Only 17 employees were fully satisfied with their compensation. Wipro may need to reassess its compensation structures to ensure competitive salaries and benefits.

Career Growth: With only 14 employees rating career growth highly, there is a clear opportunity to invest in better career development programs and promotion opportunities.

Work-Life Balance: A significant portion of employees rated work-life balance highly, indicating that Wipro’s work-life balance policies are generally positive but may require ongoing adjustments to meet the needs of all employee groups.

Job Role Satisfaction: Employees seem to have lower satisfaction regarding their job roles, with only 17 employees rating it highly. Job design and role clarity could be areas for improvement.

* Market Trends and Company Performance:

Employees in a "growing" market generally had higher satisfaction levels, while those in "declining" markets showed lower satisfaction and increased attrition risk. Market conditions should be considered when developing retention and engagement strategies.

Employees’ perception of company performance directly impacted their satisfaction levels, suggesting that transparent communication about the company's direction and performance could positively affect employee morale.

* Recommendations:
Enhance Career Growth Opportunities: Addressing career stagnation (especially in the 2-3 year tenure group) by offering clearer growth paths, mentorship, and more frequent performance reviews can help boost retention.

Optimize Compensation & Benefits: A thorough review of compensation structures to ensure competitiveness within the industry can help retain top talent, particularly those dissatisfied with salary.

Invest in Hybrid and Remote Work: Strengthening remote and hybrid work policies to ensure effective communication, career development, and engagement will support employee satisfaction in these work environments.

Improve On-Site Employee Satisfaction: For on-site employees, improving job roles, compensation, and career growth opportunities could help reverse the declining satisfaction trends.


## Final Thoughts:

This project highlights that employee retention and satisfaction are multifaceted and require tailored approaches depending on tenure, work environment, and department. By focusing on the areas identified, Wipro can create a more engaged, satisfied, and productive workforce, which will ultimately contribute to long-term organizational success.

