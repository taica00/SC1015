# About

## Problem definition
You are a moderator for a job recruitment website and with many job postings being posted on the site daily, you have to sieve out the fraudulent job postings from the real postings. Therefore you are trying to use data science and machine learning in order to create an algorithm which identifies which job posting is fraudulent based on certain variables. 
## Models used

## Jupyter Notebook 1: Cleaning of Dataset
## Notebook 2: Exploratory Data Analysis
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


