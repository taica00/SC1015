# Fraudulent Job Posting Detector
## About
This is our Mini-Project for Intro to Data Science and Artificial Intelligence (SC1015) that focuses on detecting fraudulent job postings from a [Kaggle dataset](https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction). 
## Problem definition
The COVID-19 pandemic has displaced millions of people from their jobs. In these desperate times, this has provided a perfect opportunity for online scammers to prey on their desperation. We are witnessing a daily rise in fake job postings and it is becoming increasingly difficult to differentiate between real and fraudulent job postings. Through this project, we aim to use data science and machine learning to create a classification model that uses text data features and meta-features to predict whether a job posting is fraudulent in nature.
## Contributors
[@leedz31](https://github.com/leedz31) Lee Ding Zheng: Cleaning of data, EDA and Presentation </br>
[@JeeinK](https://github.com/JeeinK) Qwek Jin Kee: Cleaning of data, EDA and Presentation </br>
[@taica00](https://github.com/taica00) Tai Chen An: Machine Learning 
## Models used
1. Random forest
2. K-Nearest Neighbours
3. XGBClassifier
## [Notebook 1: Cleaning of Dataset](https://github.com/taica00/SC1015/blob/main/Cleaning%20of%20Dataset.ipynb)
For the first notebook, we cleaned the dataset by removing any variables with high amounts of NaN values. Next, we converted text variables to their character count as we decided that numerical values were easier to analyse as compared to text data. We also omitted the cities from the location variable, so that we can generalise the locations and categorise them by countries instead.</br>
## [Notebook 2: Exploratory Data Analysis](https://github.com/taica00/SC1015/blob/main/Exploratory%20Data%20Analysis%20of%20Dataset.ipynb)
In this notebook, we first did some simple exploration of our cleaned data. From this, we discovered that our dataset was very imbalanced as the number of real job postings was much higher than fraudulent job postings. We then did exploratory data analysis of each variable by plotting each variable into two categories: fraudulent and non-fraudulent to find the correlation between the variables to the response variable: fraudulent. We then removed any variables that we think might not have a high relation to the response variable.
Variables: Job Title, Location, Telecommuting, has_company_logo, has_questions, employment_type, required_experience, required_education, industry, function, description_length, company_profile_length, requirements_length, benefits_length, fraudulent
## [Notebook 3: Data preparation - MissForest and SMOTENC](https://github.com/taica00/SC1015/blob/main/MissForest%20and%20SMOTENC.ipynb)
We first used the MissForest algorithm to impute all missing data. As mentioned in the previous notebook, we discovered that the dataset was very imbalanced. Hence, we decided to use SMOTENC(Synthetic Minority Over-sampling Technique for Nominal and Continuous), an oversampling technique to balance our dataset. 
## [Notebook 4: Machine learning - Random Forest, K-Nearest Neighbours, XGBClassifier](https://github.com/taica00/SC1015/blob/main/Machine%20Learning.ipynb)
We used 3 different classification models on our dataset. We used GridSearchCV to tune the hyperparameters for each model, aiming for the best F1 score. 
## Conclusion
- XGBClassifier was the best model for our dataset with a F1-score and recall of 0.83, and a precision of 0.82, for the positive class.
- This means that we are able to predict most fraudulent job postings, and most of the predictions are accurate.
## What did we learn from this project?
- Imputating missing data with algorithms such as MissForest.
- Creating synthetic examples of the minority class for an imbalanced dataset with SMOTE for training our classification models.
- How different classification models work and why some work better for our dataset.
- Cross validation with GridSearchCV to tune the hyperparameters for our classification models.
## References
- https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction
- https://medium.com/analytics-vidhya/smote-nc-in-ml-categorization-models-fo-imbalanced-datasets-8adbdcf08c25
- https://towardsdatascience.com/missforest-the-best-missing-data-imputation-algorithm-4d01182aed3
- https://www.kaggle.com/code/sociopath00/random-forest-using-gridsearchcv/notebook
- https://medium.datadriveninvestor.com/k-nearest-neighbors-in-python-hyperparameters-tuning-716734bc557f
- https://www.analyticsvidhya.com/blog/2016/03/complete-guide-parameter-tuning-xgboost-with-codes-python/
