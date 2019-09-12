# CAX Mortgage by CrowdANALYTIX: Yury Fedotov
**To see the code itself, please, open the notebook 'CAX_Notebook_Fedotov' in the repository! But I'd recommend you to read this file first**
## Introduction ##
CAX Mortgage by CrowdANALYTIX was my first ML competition (**May 2019**). Before participating in it, I had already studied 100+ hours of Python courses at DataCamp, created a Python-based model for valuation of M&A deals within my bachelor thesis, and created a minimum viable pipeline for the famous Titanic problem at Kaggle.

Here I share my experience and code from this competition! I didn't take any prizes on it, and my final score was around the 50th percentile among all participants, but I gained huge experience which will definetely support me in my future work.

## Objective ##
The objective of CAX Mortgage competition was to build a model that **predicts**, given mortgage application information (like applicant's income, age and credit score), **whether the mortgage will be funded or not**. Funded in a sense that a bank approves the application, not is a sense that a borrower succesfully repays principal and interest parts of the mortgage. The information regarging whether the mortgage was repaid is out of scope of this competition.
Let's conclude that it was a **binary classification task**.

## Data ##
There were 19 features in the original dataset, which represent a past customer’s mortgage application data. Here is a list of them:
1. Property value
1. Mortgage Payment, comprised of a principal portion, an interest portion, a property tax portion and a life insurance portion, calculated based on the interest rate, amortization period and payment frequency.
1. GDS: Annualized Housing Expenses / Annual Income
1. LTV: Mortgage Amount / Property Value
1. TDS: (Annualized Housing Expenses + Other Expenses) / Annual Income
1. Amortization, in month
1. Mortgage Amount requested, in dollars
1. Interest rate requested
1. Mortgage Purpose: purchase or refinance
1. Payment Frequency
1. Property Type
1. Term of the mortgage requested
1. FSA – the first three characters of the postal code, designating an area where the property is
1. Age Range of the main applicant
1. Gender
1. Income, in USD per year
1. Income type
1. NAICS code of the job category
1. Credit score

The target variable was called 'Result', and had a value of 1 for funded applications and 0 for declined.
Organizers provided the train (46k observations) and test (15k) sets, which allow this binary classification problem to be approached with **supervised learning** techniques.

During the feature engineering I used a table in **Notion.so** to control the process. Here I share a version of it, which is not final, but still allows to understand how I kept track of my work.
Link: https://drive.google.com/file/d/1mRdSCsd-zIHxNg1pNgbSwjFe9Dx1A7Qj/view?usp=sharing

## List of areas covered & instruments used ##
During this competition I managed to cover the following **areas**:
1. Deep analysis of the data: exploratory data analysis, statistical hypotheses tests
1. Preprocessing of features
1. New features engineering
1. Selection of features to be included in the model
1. Creating different ML models (supervised learning) in a binary classification task
1. Hyperparameters tuning (aka optimization) using the Grid Search algorithm
1. Valuation of model's performance using Cross Validation Scoring
1. Preparing a final submission file according to competition's requirements

**Packages employed:**
1. Pandas
1. Numpy
1. Matplotlib
1. Seaborn
1. Scikit learn
1. Scipy

## Conclusion
CAX Mortgage by CrowdANALYTIX was my first ML competition, and I'm very happy how it went. I didn't take any prizes on it, and my final score was around the 50th percentile among all participants, but I gained huge experience which will definetely support me in my future work. I would say that the following experience was the most valuable:
* Preprocessing features with many different techniques
* Choosing features to include into models
* Improving a score step-by-step, submitting a few solutions per day

After this competition I also understood which areas I need to focus on. The key of them are:
* Feature engineering, especially scaling and normalizing
* Feature selection
* Getting insights from data with weird distributions, outliers, missing values and errors
