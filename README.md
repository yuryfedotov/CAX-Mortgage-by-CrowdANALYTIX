# yf_caxmortgage
## Introduction ##
CAX Mortgage by CrowdANALYTIX was my first ML competition (**May 2019**). Before participating in it, I had already studied 100+ hours of Python courses at DataCamp, created a Python-based model for valuation of M&A deals within my bachelor thesis, and created a minimum viable pipeline for the famous Titanic problem at Kaggle.

Here I share my experience and code from this competition!

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
1. Income
1. Income type
1. NAICS code of the job category
1. Credit score

The target variable was called 'Result', and had a value of 1 for funded applications and 0 for declined.
Organizers provided the train (46k observations) and test (15k) sets, which allow this binary classification problem to be approached with **supervised learning** techniques.
