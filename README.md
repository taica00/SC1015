# About

## Problem definition
You are a moderator for a job recruitment website and with many job postings being posted on the site daily, you have to sieve out the fraudulent job postings from the real postings. Therefore you are trying to use data science and machine learning in order to create an algorithm which identifies which job posting is fraudulent based on certain variables. 
## Models used
1. Random forest
2. K Nearest Neighbours
3. Logistics Regression
## Jupyter Notebook 1: Cleaning of Dataset
For the first notebook, we cleaned the dataset by removing any variables with high amounts of NaN values. Next, we converted text variables to their character count as we decided that numerical values were easier to analyse as compared to text data.
## Notebook 2: Exploratory Data Analysis
For exploratory analysis, we plotted a bargraph comparing the number of fraudulent job postings versus non-fraudulent ones and discovered that the dataset was very imbalanced. We then did exploratory data analysis of each variable by plotting each variable into two categories: fraudulent and non-fraudulent. 
## Notebook 3: Data preparation - Miss forest and SMOTE
## Notebook 4: Machine learning - Random forest, K nearest neighbours
## Contributions
## References





# Determine if a job posting is fraudulent. 
We want to perform data analysis on the dataset to identify interesting insights from this dataset.<br />
Create a classification model that uses text data features and meta-features to predict whether a job posting is fraudulant in nature.<br />
Dataset link: https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction?select=fake_job_postings.csv

# Dataset Headers
Variables: Job Title, Location, Department, Salary_range, Company_profile, Description, Requirements, Benefits, Telecommuting, Has_company_logo, Has_questions, 
Employment_type, Required_experience, Required_education, Industry, Function, Fraudulent

# Exploratory Data Analysis
* We cleaned the data and removed the variables that we think may not have a high relation to whether a job posting is fraudulent.
* After cleaning the data, we proceeded to find the correlation of the different data columns of the data to the response variable: fraudulent.
* salary_range, company_profile_length, requirements_length, telecommuting, has_company_logo, has_questions


