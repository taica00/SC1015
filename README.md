# Fraudulent Job Posting Detector
## About
This is our mini project for Intro to Data Science and Artificial Intelligence (SC1015) that focuses on detecting fraudulent job postings.
## Problem definition
The COVID-19 pandemic has displaced millions of people from their jobs. In these desperate times, this has provided a perfect opportunity for online scammers to prey on their desperation. We are witnessing a daily rise in fake job postings and it is becoming increasingly difficult to differentiate between real and fraudulent job postings. Through this project, we aim to use data science and machine learning to create a classification model that uses text data features and meta-features to predict whether a job posting is fraudulent in nature.
## Models used
1. Random forest
2. K Nearest Neighbours
3. Logistics Regression
## [Notebook 1: Cleaning of Dataset](https://github.com/taica00/SC1015/blob/main/Cleaning%20of%20Dataset%20.ipynb)
For the first notebook, we cleaned the dataset by removing any variables with high amounts of NaN values. Next, we converted text variables to their character count as we decided that numerical values were easier to analyse as compared to text data.</br>


## [Notebook 2: Exploratory Data Analysis](https://github.com/taica00/SC1015/blob/main/MissForest%20and%20SMOTENC.ipynb)
We then did exploratory data analysis of each variable by plotting each variable into two categories: fraudulent and non-fraudulent to find the correlation between the variables to the response variable: fraudulent. We then removed any variables that we think might not have a high relation to the response variable.
Variables: Job Title, Location, Department, Salary_range, Company_profile, Description, Requirements, Benefits, Telecommuting, Has_company_logo, Has_questions, 
Employment_type, Required_experience, Required_education, Industry, Function, Fraudulent
## [Notebook 3: Data preparation - Miss forest and SMOTENC]()
We plotted a bargraph comparing the number of fraudulent job postings versus non-fraudulent ones and discovered that the dataset was very imbalanced. Hence, we decided to use SMOTENC(Synthetic Minority Over-sampling Technique for Nominal and Continuous), an oversampling technique to balance our dataset. We also used MissForest, an algorithm that imputes all missing data using mean/mode for each variables with missing values. 
## [Notebook 4: Machine learning - Random forest, K nearest neighbours]()
We did machine learning. Then we compare the values to see which is the better model to use. To be elaborated more upon later.
## Contributions
Lee Ding Zheng: Cleaning of data, EDA and Presentation </br>
Qwek Jin Kee: Cleaning of data, EDA and Presentation </br>
Tai Chen An: Machine Learning 
## References
https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction
