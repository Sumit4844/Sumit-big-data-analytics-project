Project Overview
This project analyses global data science job salaries using the ds_salaries.csv dataset. The dataset provides detailed
information about salaries, job titles, experience levels, employment types, company sizes, and remote work ratios
for data-related roles across different countries and years.
The goal is to uncover salary trends, remote work impact, and other key insights that reflect the state of the data
science job market.
Dataset Description
File Name: ds_salaries.csv
Total Records: 607
Total Columns: 12
Features:
Column Name Description
work_year Year in which the salary data was recorded (2020–2022)
experience_level Level of experience (EN: Entry, MI: Mid, SE: Senior, EX: Executive)
employment_type Type of employment (FT: Full-time, PT: Part-time, CT: Contract, FL: Freelance)
job_title Specific job role/title
salary Raw salary amount in the local currency
salary_currency Currency type of the salary
salary_in_usd Salary converted into USD for standard comparison
employee_residence Country where the employee resides
remote_ratio Percentage of remote work (0 = On-site, 50 = Hybrid, 100 = Fully remote)
company_location Location of the employing company
company_size Size of the company (S = Small, M = Medium, L = Large)
Project Objectives
1. Analyze salary distribution and trends in data-related roles.
2. Compare salaries across experience levels, company sizes, and locations.
3. Study the effect of remote work on salaries.
4. Identify the most common and highest-paying job titles.
5. Provide insights useful for professionals entering or advancing in the data field.
Technologies Used
Tool Purpose
HiveQL (Apache Hive) Data querying and aggregation
HDFS / Local Storage Data storage
Python (Pandas, Matplotlib) Data analysis and visualization
Excel / CSV Raw data format
Jupyter Notebook (Optional) Interactive analysis and documentation
Steps Performed
1. Data Loading:
Imported ds_salaries.csv into Hive using a CREATE TABLE command with CSV SerDe.
2. Schema Validation:
Checked column names, data types, and total records.
3. Data Cleaning:
o Removed unnecessary columns (Unnamed: 0).
o Verified missing and inconsistent data.
o Converted salary to numeric type.
4. Exploratory Data Analysis (EDA):
o Used Hive queries to compute:
▪ Average salary by year, experience, and company size.
▪ Top-paying job titles and countries.
▪ Salary comparison between remote and on-site jobs.
▪ Job count distribution by title and employment type.
5. Visualization (Optional in Python):
o Created bar charts for average salary by experience level and remote ratio.
o Line charts for salary trends across years.
Key Insights
1. Salary Growth:
Average salary increased slightly from 2020 to 2022, showing steady growth in the data field.
2. Experience Level Impact:
Senior (SE) and Executive (EX) professionals earned significantly more than Entry (EN) or Mid (MI) levels.
3. Top Roles:
o Machine Learning Engineer and Data Scientist were among the highest-paying positions.
o Data Scientist was also the most common job title (143 occurrences).
4. Remote Work:
Fully remote (100%) jobs often paid higher than on-site roles, reflecting global flexibility.
5. Company Size:
Large companies offered slightly higher pay, but medium companies had the most employees.
6. Global Trends:
o The United States had the majority of employees and top salary ranges.
o USD was the most common currency used.
7. Employment Type:
Full-time roles dominated (≈97%), indicating stable, long-term employment trends in the data field.
Conclusion
The analysis of the Data Science Salaries dataset reveals a rapidly evolving industry with high-paying opportunities for
skilled professionals, particularly in machine learning and data engineering roles. Experience level, company size, and
remote flexibility significantly influence salaries.
