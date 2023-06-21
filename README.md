# Group4_Project1_DataAnalyticsproject-one

Data Analytics Bootcamp - Project 1 - Group 4

Group Members: Nancy Frye, Bharti Sharma, Katherine Okray, Barbara Kocurek

## Project Title:

Is College Worth It? 

## Project Description: 

### Overall: 
This project investigates if there is a relationship between the typical education level required for a job and the median average salary for that job in the U.S. Additionally, this project looks at predictors of college graduation rates to determine if school size, type, or selectivity make a difference in graduation rates.

The focus of this project is the United States, and the datasets analyzed are from 2015 to 2021.

#### Question 1 Description:

Is there a correlation between the typical education level required for a job and the salary for that job in the U.S.? We used a dataset from Bureau of labor statistics to find the correlation between the Level of Education and the Average annual salary. The data listed the information on 832 job categories. We used two variables from the dataset to study the relationship: Typical Entry level Education Median annual wage

#### Question 2 Description:

Is there a relationship between institutional characteristics (size, type, selectivity, and cost) on four- and six-year graduation rates of bachelor’s degree students who entered U.S. colleges in Aug 2015?

We used the dataset from 'Integrated Post Secondary Education Data System'(IPEDS).The data listed information on 1367 four year degree granting institutions in the United States. We used different variables for our analysis including:

- Percentage of students admitted in 2015 who had graduated by 2021.
- Type of institution(Public/Private).
- Total Cost.
- Total Enrollment.
- Percent Admitted

Major sources of the datasets: - Bureau of Labor Statistics - Integrated Post Secondary Education Data System (IPEDS)

#### GitHub:
https://github.com/katherineokray/project-one
Jupyter Notebook: https://github.com/katherineokray/project-one/blob/main/group_project1.ipynb

#### References: 

UTA-VIRT-DATA-PT-04-2023-U-LOLC

### Approach to Data Analysis 
#### Step 1: 

Read in raw data from Bureau of Labor Statistics (2021 wage data) Convert wage data to numeric Remove commas Replaced “>=208000” with “208000” in wage column. This affected 18 entries.

#### Step 2: 

Grouped data based on typical entry level education level Got the mean and median wages by education level Got information on quartiles to create a box plot Explored other ways to visualize data including Bar chart Pie chart Histogram Conducted an ANOVA to examine whether there were statistically significant differences in wages across education levels. The null hypothesis is rejected based on the low p-value.Median annual wage diffres significantly across Education level.The average salary for jobs that require the doctoral degree is the highest while it is lowest for the jobs that require no formal education.

#### Step 3: 

Read into the dataset from 'Integrated Post Secondary Education Data System'(IPEDS). The data listed information on 1,367 four year degree-granting institutions in the United States. We used different variables for our analysis including: Percentage of students admitted in 2015 who had graduated by 2021. Type of institution(Public/Private). Total Cost. Total Enrollment. Percent Admitted Dropped NAs and created a DataFrame that contained relevant information. Conducted descriptive statistics for 2015 graduation rates for both public and private institutions. Conducted an independent t-test on graduation rates for public and private institutions. Ran a Linear Regression models to predict graduation rates from(Overall, Public and Private): Cost Total Enrollment Percent Admitted

#### CONCLUSION:

There is a positive relationship between the typical education level required for a job and the wage for that job in the U.S.

a. Graduation rates were higher in private than public institutions 
b. The p-value is less than 0.05 (p < 0.05); however, there were several outliers for the private school data. 
c. Graduation rates were higher for more expensive institutions 
d. At public institutions, graduation rates were higher for larger institutions 
e. There was no relationship between graduation rates and selectivity

#### LIMITATIONS: 

1. BLS: 

- is survey data
- Median Wages do not indicate “entry-level” or more experience in the field. 

2. IPEDS:

- is survey data
- Not all schools report; school that do report do not always report all data.
- The reason is unknown for students not graduating from specific institutions.
   
#### NEXT STEPS/FUTURE IMPROVEMENTS:

1. Evaluate college retention rates 
2. Investigate wages and graduation by field of study 
3. Investigate amount of student debt
